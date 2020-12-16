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
	import ModalVertical from './ModalPopupVertical.svelte';
	
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
        let input = document.querySelectorAll("#tel");
		for (let elements of input) {
			elements.addEventListener("input", mask, false);
			elements.addEventListener("focus", mask, false);
			elements.addEventListener("blur", mask, false);
		}
    });

    // /Маска телефона

// Создание анимаций

window.addEventListener('DOMContentLoaded', function() {

	// Двумерный массив
	// 1 - значение, блок к которму будет применяться класс анимации
	// 2 - значение, класс анимации
	let elemAnimation = [
		['.about__block-1', 'animation-left_block'],
		['.about__block-2', 'animation-right_block'],
		['.about__animation-3', 'animation-left_block'],
		['.about__block-4', 'animation-right_block'],
		['.first__block', 'second_animation'],
		['.second__block', 'first_animation'],
		['.thirty__block', 'third_animation'],
		['.title_text_anim_1', 'anim_1'],
		['.title_text_anim_2', 'anim_2'],
		['.title_text_anim_3', 'anim_3'],
		['.title_text_anim_4', 'anim_4'],
		['.title_text_anim_5', 'anim_5'],
		['.first__block_anim', 'animation__youGet'],
		['.second__block_anim', 'animation__youGet'],
		['.thirty__block_anim', 'animation__youGet'],
		['.fouty__block_anim', 'animation__youGet'],
		['.fifty__block_anim', 'animation__youGet'],
		['.sixty__block_anim', 'animation__youGet'],
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

	// var tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-toggle="tooltip"]'))
	// var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
	// return new bootstrap.Tooltip(tooltipTriggerEl)
	// 	});
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

<div class="container__fixed__width">
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
	<ModalVertical/>
</div>

<style>
	.container__fixed__width{
		max-width: 1900px;
		min-width: 320px;
		margin: auto;
	}

</style>