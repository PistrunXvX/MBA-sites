<script>
	import Header from './Header.svelte';
	import About from './AboutUs.svelte';
	import YouCan from './YouCan.svelte';
	import YouGet from './YouGet.svelte';
	import Form from './FeedbackForm.svelte';
	import Slider from './Slider.svelte';
	import Price from './Price.svelte';
	import Advantage from './Advantage.svelte';
	import Cooperative from './Cooperative.svelte';
	import Sertificat from './Sertificat.svelte';
	import FormFooter from './FormFooter.svelte';
	import Footer from './Footer.svelte';
	import Modal from './ModalPopup.svelte';
	
	// Musk phone 


	
	window.addEventListener("DOMContentLoaded", function() {
    function setCursorPosition(pos, elem) {
        elem.focus();
        if (elem.setSelectionRange) elem.setSelectionRange(pos, pos);
        else if (elem.createTextRange) {
            let range = elem.createTextRange();
            range.collapse(true);
            range.moveEnd("character", pos);
            range.moveStart("character", pos);
            range.select()
        }
    }
    
    function mask(event) {
        let matrix = "+7 (___) ___ __ __",
            i = 0,
            def = matrix.replace(/\D/g, ""),
            val = this.value.replace(/\D/g, "");
        if (def.length >= val.length) val = def;
        this.value = matrix.replace(/./g, function(a) {
            return /[_\d]/.test(a) && i < val.length ? val.charAt(i++) : i >= val.length ? "" : a
        });
        if (event.type == "blur") {
            if (this.value.length == 2) this.value = ""
        } else setCursorPosition(this.value.length, this)
    };
        let input = document.querySelector("#tel");
        input.addEventListener("input", mask, false);
        input.addEventListener("focus", mask, false);
        input.addEventListener("blur", mask, false);
    });

    // /Маска телефона

// Создание анимаций

window.addEventListener('DOMContentLoaded', function() {

	// Двумерный массив
	// 1 - значение, блок к которму будет применяться класс анимации
	// 2 - значение, класс анимации
	let elemAnimation = [
		['.about__block-1', 'test_1'],
		['.about__block-2', 'test_2'],
		['.about__block-4', 'test_3'],
	];

	// Проверяет, если элемент в поле зрения - true, инчае - false
	function isVisible(elem) {
		let windowHeight = document.documentElement.clientHeight;

		let coords = elem.getBoundingClientRect();
		if (coords.top > 0 && coords.top < windowHeight) {
			return true;
		} else {
			return false;
		}
	};

	// Генерирует массив с выделенными элементами
	function makeDocumentArray(array) {
		let documentElemArray = [];
		for (let i = 0; i < array.length; i++) {
			let docTime = document.querySelector(array[i][0]);
			documentElemArray.push(docTime);
		}

		return documentElemArray;
	};

	let arrayElement = makeDocumentArray(elemAnimation);

	window.addEventListener('scroll', function() {

		// Проверяет массив с элементами при каждом скролле
		let i = 0;
		for (let elements of arrayElement) {
			if (isVisible(elements)) {
				elements.classList.add(elemAnimation[i][1]);
			}
			i++;
		}
	});
});

window.addEventListener('DOMContentLoaded', function() {
	let formModule = document.querySelector('.form__send__module');

	formModule.addEventListener('submit', function(evt) {
		evt.preventDefault();

		let formData = {
			name: document.querySelector('input[name="name"]').value,
			phone: document.querySelector('input[name="phone"]').value,
			email: document.querySelector('input[name="email"]').value,
		}

		let request = new XMLHttpRequest();

		request.addEventListener('load', function() {
			console.log(request.response);
		});

		request.open('POST', '/send.php', true);
		request.setRequestHeader('Content-Type', 'application/x-www-form-urlencoded; charset=UTF-8');
		request.send('name= ' + encodeURIComponent(formData.name) + ' phone= ' + encodeURIComponent(formData.phone) + ' email= ' + encodeURIComponent(formData.email));
	});

});

</script>



<Header/>
<About/>
<YouCan/>
<Form/>
<YouGet/>
<Slider/>
<Price/>
<Advantage/>
<Cooperative/>
<Sertificat/>
<FormFooter/>
<Footer/>
<Modal/>

<style>

</style>