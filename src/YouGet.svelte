<script>
import { draw } from 'svelte/transition';

let duration = 3000;
let delay = 200;

// Размещать в строгом порядке с воспроизведением анимаций
let elemAnimation = [
    ['.blue__line__1', false],
    ['.yellow__line__1', false],
    ['.blue__line__2', false],
    ['.yellow__line__2', false],
    ['.blue__line__3', false],
];

window.addEventListener('DOMContentLoaded', function() {


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
				elemAnimation[i][1] = true;
			}
			i++;
		}
	});
});
</script>

<div class="container-fluid youGet__block">
    <h2>Что вы получаете</h2>
    <div class="container-fluid">
        <div class="row">
            <div class="col">
                <article class="first__block container__block">
                    <div class="icon__yellow">
                        <div class="bg__color first__block_anim">
                            <h3>Единый стандарт обучения</h3>
                            <p>
                                Ваши сотрудники формируют единый понятный аппарат, что позволяет сэкономить время
                                на неэффективных коммуникациях
                            </p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
        <div class="line__to blue__line__1">
            {#if elemAnimation[0][1]}
            <svg viewBox="0 0 100 3" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 3 H 34 Z" stroke="#2C467C" transition:draw="{{duration, delay}}"/>
            </svg>
            {/if}
        </div>
        <div class="row">
            <div class="col">
                <article class="second__block container__block">
                    <div class="icon__blue">
                        <div class="bg__color second__block_anim">
                            <h3>Широкая линейка программ</h3>
                            <p>
                                Благодаря большому количеству программ вы можете «закрыть» потребности обучения на
                                любом бизнес-направлении
                            </p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
        <div class="line__to yellow__line__1">
            {#if elemAnimation[1][1]}
            <svg viewBox="0 0 100 3" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 3 H 32.5 Z" stroke="#EA8E02" transition:draw="{{duration, delay}}"/>
            </svg>
            {/if}
        </div>
        <div class="row">
            <div class="col">
                <article class="thirty__block container__block">
                    <div class="icon__yellow">
                        <div class="bg__color thirty__block_anim">
                            <h3>Эксперты-практики</h3>
                            <p>
                                Более 300 опытных преподавателей, прошедших внутреннюю сертификацию
                            </p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
        <div class="line__to blue__line__2">
            {#if elemAnimation[2][1]}
            <svg viewBox="0 0 100 3" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 3 H 32 Z" stroke="#2C467C" transition:draw="{{duration, delay}}"/>
            </svg>
            {/if}
        </div>
        <div class="row">
            <div class="col">
                <article class="fouty__block container__block">
                    <div class="icon__blue">
                        <div class="bg__color fouty__block_anim">
                            <h3>Гибкое расписание</h3>
                            <p>
                                Частота программ позволит обучать разных сотрудников 
                                по одной и той же тематике с регулярностью 
                                один раз в два месяца
                            </p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
        <div class="line__to yellow__line__2">
            {#if elemAnimation[3][1]}
            <svg viewBox="0 0 100 3" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 3 H 32.6 Z" stroke="#EA8E02" transition:draw="{{duration, delay}}"/>
            </svg>
            {/if}
        </div>
        <div class="row">
            <div class="col">
                <article class="fifty__block container__block">
                    <div class="icon__yellow">
                        <div class="bg__color fifty__block_anim">
                            <h3>Экономия бюджета</h3>
                            <p>
                                Свыше 50% вашего бюджета может остаться на развитие важных бизнес-целей
                            </p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
        <div class="line__to blue__line__3">
            {#if elemAnimation[4][1]}
            <svg viewBox="0 0 100 3" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 3 H 34.6 Z" stroke="#2C467C" transition:draw="{{duration, delay}}"/>
            </svg>
            {/if}
        </div>
        <div class="row">
            <div class="col">
                <article class="sixty__block container__block">
                    <div class="icon__blue">
                        <div class="bg__color sixty__block_anim">
                            <h3>Багаж практических инструментов</h3>
                            <p>
                                Электронная версия презентаций и дополнительных материалов, с возможностью делиться и использовать в работе в постоянном режиме
                            </p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
    </div>
</div>


<style lang="scss" >
    @import 'style/theme.scss';

    .youGet__block{
        padding-bottom: 131px;
        position: relative;

        .bg__color{
            background-color: $grey;

            padding: 50px 30px;

            border-radius: 50px;
        }

        .icon__yellow:after{
            display: block;
            position: absolute;
            content: ' ';
            background-image: url(/img/yellow_elips.svg);
            background-size: 80px 80px;
            height: 80px;
            width: 80px;
            left: 45%;
            top: 40%;
        }

        .icon__blue:after{
            display: block;
            position: absolute;
            content: ' ';
            background-image: url(/img/blue_ellips.svg);
            background-size: 80px 80px;
            height: 80px;
            width: 80px;
            right: 45%;
            top: 40%;
        }
                
        h2{
            font-size: $blockTitleSize;
            font-family: $fbck;
            color: $darkBlue;
            text-align: center;
            text-transform: uppercase;

            margin-top: 5%;
        }

        article{
            
            font-family: $fbck;
            color: $darkBlue;

            margin-top: 20%;

            background-repeat: no-repeat;
            background-size: 150px;

            position: relative;

            h3{
                font-size: 56px;
            }

            p{
                font-size: $description;
            }
        }

        .first__block{
            margin-top: 10%;
        }

        .first__block, .thirty__block, .fifty__block{
            text-align: left;
            padding-right: 55%;
            background-position: 80% 50%;

            margin-left: 5%;
        }

        .second__block, .fouty__block, .sixty__block{
            text-align: right;
            padding-left: 55%;
            background-position: 20% 50%;

            margin-right: 5%;
        }

        .first__block{
            background-image: url(/img/education_icon_youGet.svg);
        }

        .second__block{
            background-image: url(/img/book_icon_youGet.svg);
        }
        
        .thirty__block{
            background-image: url(/img/atom_icon_youGet.svg);
        }

        .fouty__block{
            background-image: url(/img/research_icon_youGet.svg);
        }

        .fifty__block{
            background-image: url(/img/salary_icon_youGet.svg);
        }

        .sixty__block{
            background-image: url(/img/bag_icon_youGet.svg);
        }

        .line__to{
            position: absolute;
            width: 98%;
            transform: rotate(90deg);
        }

        .line__to svg{
            margin-bottom: 1%;
        }

        .blue__line__1{
            // position: fixed;
            top: 32.3%;
        }

        .yellow__line__1{
            top: 48.8%;
        }

        .blue__line__2{
            top: 64.8%;
        }

        .yellow__line__2{
            top: 80.5%;
        }

        .blue__line__3{
            top: calc(100% - (100% - 96.5%));
        }

    }
</style>