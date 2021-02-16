<div id="thanksModal" class="modal">
        <div class="modal-content">
            <div class="modal-body">
                <h2>
                    Спасибо! Мы обязательно свяжемся с вами!
                </h2>
            </div>
        </div>
</div>

  <style lang="scss">
      @import './style/theme.scss';

      h2{
          color: $darkBlue;
          font-size: 24px;
          font-family: $fbck;
          font-weight: bold;

          text-align: center;
      }

      .thanksModal {
        display: none; /* Скрыто по умолчанию */
        background-color: rgb(0,0,0); /* Затемнение фона */
        background-color: rgba(0,0,0,0.5); /* Полупрозрачное затемнение */
        z-index: 1; /* Фон на нижнем слое */
        overflow: auto; /* При необходимости, то появиться прокрутка */
    }

    .modal-content {
        animation-name: animate;
        animation-duration: 0.5s;

        width: 50%;
        margin: auto;

        margin-top: 30vh;
    }

    .modal-body{
        padding: 10%;
    }

    @keyframes animate {
        from {top:-500px; opacity:0}
        to {top:0; opacity:1}
    }
  </style>