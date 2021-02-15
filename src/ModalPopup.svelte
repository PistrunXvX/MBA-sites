<script>
window.addEventListener('DOMContentLoaded', function() {
	let formModule = document.querySelector('#first__modal__header');

	formModule.addEventListener('submit', function(evt) {
		evt.preventDefault();

		let formData = {
			name: document.querySelector('input[name="name"]').value,
            phone: document.querySelector('input[name="phone"]').value,
            secondName: document.querySelector('input[name="secondName"]').value,
			email: document.querySelector('input[name="email"]').value,
		};

		let request = new XMLHttpRequest();

		request.addEventListener('load', function() {
            console.log(request.response);
            let buttonClose = document.querySelector('.btn_popup_1');
            let modalBody = formModule.querySelector('.modal-body');
            modalBody.innerHTML = '<p style="font-size: 18px; color: #FFFFFF; text-align: center;">Спасибо! Мы обязательно свяжемся с вами!</p>'
            buttonClose.dataset.dismiss = 'modal';
            buttonClose.type = 'button';
            buttonClose.innerHTML = 'Закрыть';
		});

		request.open('POST', 'send_popup.php', true);
		request.setRequestHeader('Content-Type', 'application/x-www-form-urlencoded; charset=UTF-8');
		request.send('name= ' + encodeURIComponent(formData.name) + ' &secondName= ' + encodeURIComponent(formData.secondName) + ' &phone= ' + encodeURIComponent(formData.phone) + ' &email= ' + encodeURIComponent(formData.email));
	});

});

window.addEventListener('DOMContentLoaded', function() {
	let formModule = document.querySelector('#second__modal__header');

	formModule.addEventListener('submit', function(evt) {
		evt.preventDefault();

		let formData = {
			name: document.querySelector('input[name="name"]').value,
            phone: document.querySelector('input[name="phone"]').value,
            secondName: document.querySelector('input[name="secondName"]').value,
			email: document.querySelector('input[name="email"]').value,
		};

		let request = new XMLHttpRequest();

		request.addEventListener('load', function() {
			console.log(request.response);
            let buttonClose = document.querySelector('.btn_popup_2');
            let modalBody = formModule.querySelector('.modal-body');
            modalBody.innerHTML = '<p style="font-size: 18px; color: #FFFFFF; text-align: center;">Спасибо! Мы обязательно свяжемся с вами!</p>'
            buttonClose.dataset.dismiss = 'modal';
            buttonClose.type = 'button';
            buttonClose.innerHTML = 'Закрыть';
            
		});

		request.open('POST', 'send_popup.php', true);
		request.setRequestHeader('Content-Type', 'application/x-www-form-urlencoded; charset=UTF-8');
		request.send('name= ' + encodeURIComponent(formData.name) + ' &secondName= ' + encodeURIComponent(formData.secondName) + ' &phone= ' + encodeURIComponent(formData.phone) + ' &email= ' + encodeURIComponent(formData.email));
	});

});
</script>


<div class="modal fade" id="first__modal__header" tabindex="-1" aria-labelledby="modal__header__label" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="modal__header__label">Форма обратной свзяи</h5>
                <button type="button" class="btn-close" data-dismiss="modal" aria-label="Close">
                    <span aria-hidden="true"></span>
                </button>
            </div>
            <form action="send_popup.php" method="POST">
                <div class="modal-body">
                    <div class="row">
                        <div class="col">
                            <p class="modal__text">Мы свяжемся с вами в течении 15 минут! Ждите звонка</p>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="text" name="name" placeholder="Ваше имя" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="text" name="secondName" placeholder="Ваша фамилия" required>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="tel" name="phone" id="tel" placeholder="Ваш номер телефона" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="email" name="email" placeholder="Ваша электронная почта" required>
                        </div>
                    </div>
                </div>
                <div class="modal-footer">
                    <div class="row">
                        <div class="col-xl-12">
                            <button class="form_btn_popup btn_popup_1" data-dismiss="none" type="submit">Отправить заявку</button>
                        </div>
                    </div>
                </div>
            </form>
        </div>
    </div>
</div>

<div class="modal fade" id="second__modal__header" tabindex="-1" aria-labelledby="modal__header__label" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="modal__header__label">Форма обратной свзяи</h5>
                <button type="button" class="btn-close" data-dismiss="modal" aria-label="Close">
                    <span aria-hidden="true"></span>
                </button>
            </div>
            <form action="send_popup.php" method="POST">
                <div class="modal-body">
                    <div class="row">
                        <div class="col">
                            <p class="modal__text">Мы свяжемся с вами в течении 15 минут! Ждите звонка</p>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="text" name="name" placeholder="Ваше имя" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="text" name="secondName" placeholder="Ваша фамилия" required>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="tel" name="phone" id="tel" placeholder="Ваш номер телефона" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="email" name="email" placeholder="Ваша электронная почта" required>
                        </div>
                    </div>
                </div>
                <div class="modal-footer">
                    <div class="row">
                        <div class="col-xl-12">
                            <button class="form_btn_popup btn_popup_2" data-dismiss="none" type="submit">Отправить заявку</button>
                        </div>
                    </div>
                </div>
            </form>
        </div>
    </div>
</div>


<style lang="scss">
    @import 'style/theme.scss';

    input:invalid:not(:placeholder-shown) {
        border-color: #ff6e5e;
    }

    input:valid:not(:placeholder-shown) {
        border-color: #79d980;
    }

    .modal-content {
        
        .modal-title {
            font-family: $fbck;
            color: $colorWhite;
            font-size: 25px;
        }

        .modal__text{
            font-family: $fbck;
            color: $colorWhite;
            font-size: 25px;
        }

        .close {
            text-shadow: none;
        }  

        .modal-footer{
            text-align: center;
            
           
            
        }

        .modal-header,
        .modal-footer {
            border-color: $orange;
            padding-top: 20px;
            padding-bottom: 20px;
        }
    }

    .modal-footer button {
        font-size: 24px;
        font-family: $fbck;
        color: $colorWhite;
        text-decoration: none;
        background-color: $orange;
        filter: drop-shadow(0px 0px 10px $orange);
        padding: 20px 40px 20px 40px;
        animation: 0.3s ease-in 0s button_color_back;
        border: none;
        transition: 0.6s;
        
        

    }

    .modal-footer button:hover {
        animation: 0.3s ease-in 0s button_color_to;
        color: $orange;
        background-color: $colorWhite;
        filter: drop-shadow(0px 0px 10px $colorWhite);
    }

    input {
        padding: 20px 60px 20px 20px;
        background-color: #2C467C;
        border: 4px solid $colorWhite;
        font-size: 19px;
        color: $colorWhite;
        
    }

    input[type="text"] {
        margin-bottom: 40px;
    }

    input::placeholder {
        color: #D3D3D3;
    }

    input:focus,
    input:active {
        color: $colorWhite;
        outline: 0;
        outline-offset: 0;
        background-color: #223661;
    }

    button:hover,
    button:active,
    button:focus {
        transition: 0.6s;
        box-shadow: 0px 0px 20px $colorWhite;
        color: $orange;
        background-color: $colorWhite;
        outline: 0;
        outline-offset: 0;
    }

    .btn-close:hover{
        box-shadow: none;
        background-color: none;
    }

        .modal-dialog{
            max-width: 850px;
           
        }
  
            .modal-body{
                text-align: center;
                padding-top: 30px;
                padding-bottom: 30px;
            }

    #first__modal__header .modal-content{
        background-color: rgba(44, 70, 124, 0.8);
    }

    #second__modal__header .modal-content{
        background-color: $darkBlue;
    }
</style>