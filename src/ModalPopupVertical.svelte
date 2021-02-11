  <script>

    // window.addEventListener("DOMContentLoaded", function() {

    // let button = document.querySelector('.btn-modal-close');

    // button.addEventListener('click', function() {
    //   setTimeout(function () {
    //     window.scrollTo(0, 0);
    //   }, 500);
    // });

    function popupClose() {
      setTimeout(function () {
        window.scrollTo(0, 0);
      }, 500);
    };

    // });
  </script>
  
  <div class="modal fade style__popup" id="first__vertical__popup"  tabindex="-1" aria-labelledby="first__vertical__popupLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-scrollable modal-lg">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="first__vertical__popupLabel">Базовый тариф</h5>
          <button type="button" class="btn-close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true"></span>
          </button>
        </div>
        <div class="modal-body">
            <p>
              Данный тариф предусматривает подключение одновременно до 5 участников компании на разные модули в течении рабочего дня. 
              Участники должны быть зарегистрированы куратором в личном кабинете. Регламент обучения с 9.00 до 14.30 (2 кофе-паузы по 10 минут)
            </p>
            <p>
              Мы рекомендуем данный тариф для тех компаний, кто планирует обучение от 3 сотрудников. 
              В этом случае тариф «Базовый» позволит сэкономить на стоимости комплексных программ, выборе конкретного вопроса для изучения и организации выезда.
              Корпоративный онлайн Университет от Русской Школы Управления – выгодная инвестиция в развитие вашей компании. 
              Воспользуйтесь сервисом – и получите большее!
            </p>
        </div>
        <div class="modal-footer">
          <button type="button" on:click={popupClose} class="btn btn-modal-close" data-dismiss="modal">Выбираю</button>
        </div>
      </div>
    </div>
  </div>

  <div class="modal fade style__popup" id="second__vertical__popup"  tabindex="-1" aria-labelledby="second__vertical__popupLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-scrollable modal-lg">
      <div class="modal-content">
        <div class="modal-header">
          <h3 class="modal-title" id="second__vertical__popupLabel">Расширенный тариф</h3>
          <button type="button" class="btn-close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true"></span>
          </button>
        </div>
        <div class="modal-body">
          <p>
            Данный тариф предусматривает подключение одновременно до 10 участников компании на разные модули в течении рабочего дня. Участники должны быть зарегистрированы куратором в личном кабинете. 
            Регламент обучения с 9.00 до 14.30 (2 кофе-паузы по 10 минут)
          </p>
          <p>
            Мы рекомендуем данный тариф для тех компаний, кто планирует обучение от 5 сотрудников компании. В этом случае тариф «Расширенный» будет хорошей альтернативой корпоративному университету offline-формата и станет вашим планировщиков для реализации стратегических задач по обучению на 6 месяцев.
            Корпоративный онлайн Университет от Русской Школы Управления – выгодная инвестиция в развитие вашей компании. Воспользуйтесь сервисом – и получите большее!
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" on:click={popupClose} class="btn btn-modal-close" data-dismiss="modal">Выбираю</button>
        </div>
      </div>
    </div>
  </div>

  <div class="modal fade style__popup" id="third__vertical__popup"  tabindex="-1" aria-labelledby="third__vertical__popupLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-scrollable modal-lg">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="third__vertical__popupLabel">Безлимитный тариф</h5>
          <button type="button" class="btn-close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true"></span>
          </button>
        </div>
        <div class="modal-body">
          <p>
            Тариф, который позволит компании обучать неограниченное количество сотрудников в течении 1 года. 
            Регламент обучения с 9.00 до 14.30 (2 кофе-паузы по 10 минут)
          </p>
          <p>
            Обучение будет доступно, не только управленческому составу компании, но и линейному персоналу. 
            Тариф «Безлимитный» для тех компаний, которые заботятся о кадровом резерве, достигают стратегических целей и задач, готовы планировать 
            бюджет и вкладывать в создание положительного имиджа на рынке. 
          </p>
          <p>
            Корпоративный онлайн Университет от Русской Школы Управления – выгодная инвестиция в развитие вашей компании. Воспользуйтесь сервисом – и получите большее!
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" on:click={popupClose} class="button__good btn-modal-close" data-dismiss="modal">Выбираю</button>
        </div>
      </div>
    </div>
  </div>

  <style lang="scss">
      @import 'style/theme.scss';

      .modal-body{
        p{
          font-size: 20px;
        }
      }

        .style__popup{

            font-family: $fbck;
            color: $colorWhite;

            .modal-header, .modal-body,
            .modal-footer{
                background-color: $darkBlue;
                border-color: $orange;
            }

            .modal-footer{

                button{
                font-size: 20px;
                 color: $colorWhite;
                 transition: 0.3s;
                
                 text-transform: uppercase;

                 padding: 15px 30px;

                 background-color: $orange;
                 border-radius: 50px;
                 border: none;
                 box-shadow: none;

                 margin: auto;
                }

                
    .btn-close:hover{
        box-shadow: none;
        background-color: none;
        // color: $colorWhite;
    }

                button:hover{
                    background-color: $colorWhite;
                    box-shadow: 0px 0px 20px $colorWhite;
                    transition: 0.3s;
                    color: $orange;
                }
            }

        }

  </style>