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
                    <input type="text" placeholder="Ваше имя" required>
                    <input type="text" placeholder="Ваша фамилия" required>
                    <input type="tel" placeholder="Ващ номер телефона" required>
                    <input type="email" placeholder="Ваша электронная почта" required>
                </div>
                <div class="modal-footer">
                    <button type="submit">Отправить заявку</button>
                </div>
            </form>
        </div>
    </div>
</div>

<style lang="scss" >
    @import 'style/theme.scss';

    .modal-content{
        background-color: $darkBlue;

        .modal-title{
            font-family: $fbck;
            color: $colorWhite;
        }

        .close{
            text-shadow: none;
        }

        .modal-header, .modal-footer{
            border-color: $orange;
        }
    }

   .modal-footer button{
            font-size: 18px;
            font-family: $fbck;
            color: $colorWhite;

            text-decoration: none;

            background-color: $orange;
            filter: drop-shadow(0px 0px 10px $orange);

            padding: 10px 20px;
            animation: 0.3s ease-in 0s button_color_back;

            border: none;

        }

    .modal-footer button:hover{
            animation: 0.3s ease-in 0s button_color_to;
            color: $orange;
            background-color: $colorWhite;
            filter: drop-shadow(0px 0px 10px $colorWhite);
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