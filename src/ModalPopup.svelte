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
                            <input type="tel" placeholder="Ваш номер телефона" required>
                        </div>
                        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-6">
                            <input type="email" placeholder="Ваша электронная почта" required>
                        </div>
                    </div>
                </div>
                <div class="modal-footer">
                    <div class="row">
                        <button type="submit">Отправить заявку</button>
                    </div>
                </div>
            </form>
        </div>
    </div>
</div>

<style lang="scss">
    @import 'style/theme.scss';

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

        .modal-header,
        .modal-footer {
            border-color: $orange;
            padding-top: 20px;
            padding-bottom: 20px;
        }
    }

    .modal-footer button {
        font-size: 20px;
        font-family: $fbck;
        color: $colorWhite;
        text-decoration: none;
        background-color: $orange;
        filter: drop-shadow(0px 0px 10px $orange);
        padding: 20px 20px;
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
        margin-bottom: 30px;
    }

    input::placeholder {
        color: #D3D3D3;
    }

    input:focus,
    input:active {
        color: $colorWhite;
        outline: 0;
        outline-offset: 0;
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