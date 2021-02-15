<script>
    let yes = false;

    window.addEventListener('DOMContentLoaded', function() {
	let formModule = document.querySelector('.form__send');

	formModule.addEventListener('submit', function(evt) {
		evt.preventDefault();

		let formData = {
			name: document.querySelector('input[name="name"]').value,
			phone: document.querySelector('input[name="phone"]').value,
			email: document.querySelector('input[name="email"]').value,
		};

		let request = new XMLHttpRequest();

		request.addEventListener('load', function() {
			console.log(request.response);
			formModule.innerHTML = '<p style="font-size: 18px; color: #FFFFFF">Спасибо! Мы обязательно свяжемся с вами!</p>';
		});

		request.open('POST', 'send.php', true);
		request.setRequestHeader('Content-Type', 'application/x-www-form-urlencoded; charset=UTF-8');
		request.send('name= ' + encodeURIComponent(formData.name) + ' &phone= ' + encodeURIComponent(formData.phone) + ' &email= ' + encodeURIComponent(formData.email));
	});

});

</script>

<div class="form-container form__footer" id="connect_form">
    <div class="container">
        <div class="row">
            <div class="col-xl-7">
                <div class="text-block">
                    <p class="text-block_content">
                        Получите временный доступ к личному кабинету, чтобы ознакомиться со всеми тонкостями процесса
                        обучения, образовательными программами и внутренним устройством
                    </p>
                </div>
            </div>
            <div class="col-xl-5">
                <form action="send.php" method='POST' id="form_ajax_2" class="form__send">
                    <div class="form-block">
                        <div class="row align-items-center">
                            <div class="col-xl-6">
                                <input type="text" name="name" class="form-control form__name" placeholder="Ваше имя" required>
                            </div>
                            <div class="col-xl-6">
                                <input name="phone" id="tel" class="form-control form__send__number"  placeholder="Ваш телефон"required>
                            </div>
                        </div>
                        <input type="email" class="form-control form_send__email" name="email" placeholder="Ваш электронный адрес"
                            required>
                        <label class="label">
                            <input type="checkbox" bind:checked={yes} class="checkbox">
                            <span class="fake"></span>
                            <span class="p">Я согласен с <a href="/img/politika_peda.pdf" target="_blank" class="link"> политикой конфиденциальности</a></span>
                        </label>
                    </div>
                    <button class="form__btn" disabled={!yes} type="submit">Отправить</button>
                </form>
            </div>
        </div>
    </div>
</div>




<style lang="scss">
    @import 'style/theme.scss';


    input:invalid {
        border-color: #ff6e5e;
    }

    input:valid {
        border-color: #76c27b;
    }

    input:invalid:not(:placeholder-shown) {
        border-color: #ff6e5e;
    }

    input:valid:not(:placeholder-shown) {
        border-color: #79d980;
    }


    .form-container {
        display: flex;
        align-items: center;
        background-color: #0C2967;
        padding-top: 100px;
        padding-bottom: 90px;
        padding-left: 80px;
        padding-right: 80px;


        .text-block_content {
            font-family: $fbck;
            font-size: 32px;
            color: $colorWhite;
        }



        .text-block {
            padding-right: 216px;


        }


        .form__name {

            margin-bottom: 39px;
        }

        .form__send__number {
            margin-bottom: 39px;
        }

        .form_send__email {
            margin-top: 0px;
            margin-bottom: 39px;

        }


        .checkbox {
            margin-bottom: 83px;
        }

        .form-control {
            padding: 22px 30px;
            background-color: #0C2967;

            border: 4px solid $colorWhite;

            font-size: 25px;
            color: $colorWhite;

        }

        .form-control::placeholder {
            color: #D3D3D3;
        }


        .form-control:focus,
        .form-control:active {
            color: $colorWhite;
            background-color: #081d4a;
        }




        .form-block {





            .p {
                color: $colorWhite;
                font-size: 18px;
                padding-left: 30px;
                padding-bottom: 91px;

            }

        }


        .link {
            color: $colorWhite;
            text-decoration: none;
            border-bottom: 3px solid $orange;
            transition: .3s
        }

        .link:hover {
            color: $orange;
            transition: .3s;
        }




        .label {
            display: flex;
            justify-content: start;
        }

        .checkbox {
            display: none;
        }

        .fake {
            display: inline-block;
            width: 40px;
            height: 40px;
            border: 5px solid $colorWhite;
            position: relative;



        }

        .fake::before {
            content: '';
            position: absolute;
            display: block;
            width: 15px;
            height: 15px;
            background-color: $orange;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            opacity: 0;
            transition: .2s;
        }


        .checkbox:checked+.fake::before {
            opacity: 1;
        }




        .form__btn {
            color: $colorWhite;
            background-color: $orange;
            line-height: 122.56%;
            letter-spacing: 0.06em;
            border-radius: 50px;
            border: none;
            font-size: $orangeButton;
            text-align: center;
            padding: 22px 65px 22px 65px;
            box-shadow: 0px 0px 20px $orange;
            transition: 0.6s;
            position: relative;
            left: 50%;
            transform: translate(-50%, 0);
        }

        .form__btn:disabled{
            opacity: 0.5;
        }

        .form__btn:disabled:hover{
            background-color: $orange;
            color: $colorWhite;
        }


        .form__btn:hover,
        .form__btn:active,
        .form__btn:focus {
            transition: 0.6s;
            box-shadow: 0px 0px 20px $colorWhite;
            color: $orange;
            background-color: $colorWhite;
            outline: 0;
            outline-offset: 0;
        }



        // убрал стрелочки input number

        input[type="number"]::-webkit-outer-spin-button,
        input[type="number"]::-webkit-inner-spin-button {
            -webkit-appearance: none;
            margin: 0;
        }


        input[type="number"] {
            -moz-appearance: textfield;
        }

        input[type="number"]:hover,
        input[type="number"]:focus {
            -moz-appearance: number-input;
        }


        input[type=number]::-webkit-inner-spin-button,
        input[type=number]::-webkit-outer-spin-button {
            -webkit-appearance: none;
            margin: 0;
        }

    }

    .form-container{
        margin-bottom: 0% !important;
        padding-top: 40px !important;
        padding-bottom: 40px !important;
    }

    .form-container .form-control{
        padding: 10px 30px !important;
        border-width: 1px !important;
        font-size: 12px !important;
        margin-bottom: 15px !important;
    }

    .form-container .fake{
        width: 20px !important;
        height: 20px !important;
        border-width: 2px !important;
    }

    .form-container .link{
        border-width: 1px !important;
    }

    .form-container .form-block .p{
        padding-bottom: 20px !important;
        font-size: 12px !important;
    }

    .form__btn {
        font-size: 24px !important;
    }

    .form-container .form__btn{
        padding: 10px 30px 10px 30px !important;
        font-size: 16px !important;
    }

    .text_block__content{
        font-size: 24px !important;
    }

    .form-container .text-block{
        padding-right: 0px !important;
    }

    .form-container .text-block_content{
        font-size: 24px;
    }

    .done_form{
        font-family: $fbck;
        color: $colorWhite;
        font-size: 18px;
    }

</style>