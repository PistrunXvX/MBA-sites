<script>
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
        let input = document.querySelector("#tel3");
        input.addEventListener("input", mask, false);
        input.addEventListener("focus", mask, false);
        input.addEventListener("blur", mask, false);
    });

    // /Маска телефона
    
        
      </script>

<div class="modal fade" id="modal__header" tabindex="-1" aria-labelledby="modal__header__label" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="modal__header__label">Заполните анкету</h5>
                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                    <span aria-hidden="true">&times;</span>
                </button>
            </div>
            <form action="post">
                <div class="modal-body">
                    <div class="row">
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="text" placeholder="Ваше имя" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="text" placeholder="Ваша фамилия" required>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="tel" id="tel3" placeholder="Ваш номер телефона" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="email" placeholder="Ваша электронная почта" required>
                        </div>
                    </div>
                </div>
                <div class="modal-footer">
                    <div class="row">
                        <div class="col-xl-12">
                            <button type="submit">Отправить заявку</button>
                        </div>
                    </div>
                </div>
            </form>
        </div>
    </div>
</div>

<style lang="scss">
    @import 'style/theme.scss';


    input:invalid {border-color: red;}
    input:valid {border-color: green;}
    input:invalid:not(:placeholder-shown) {border-color: red;}
    input:valid:not(:placeholder-shown) {border-color: green;}

    .modal-content {
        background-color: $darkBlue;

        .modal-title {
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




        .modal-dialog{
            max-width: 850px;
           
        }
  
            .modal-body{
                text-align: center;
                padding-top: 30px;
                padding-bottom: 30px;
            }

    //     @keyframes button_modal_color_to{
    //     from{
    //         background-color: $orange;
    //         color: $colorWhite;
    //         filter: drop-shadow(0px 0px 10px $orange);
    //     }
    //     to{
    //         background-color: $darkBlue;
    //         color: $orange;
    //         filter: drop-shadow(0px 0px 10px $darkBlue);
    //     }
    // }

    // @keyframes button_modal_color_back{
    //     from{
    //         background-color: $darkBlue;
    //         color: $orange;
    //         filter: drop-shadow(0px 0px 10px $darkBlue);
    //     }
    //     to{
    //         background-color: $orange;
    //         color: $colorWhite;
    //         filter: drop-shadow(0px 0px 10px $orange);
    //     }
    // }
</style>

<!-- <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body">
          ...
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
          <button type="button" class="btn btn-primary">Save changes</button>
        </div>
      </div>
    </div>
  </div> -->