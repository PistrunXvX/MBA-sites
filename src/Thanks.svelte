<script>

    function closePopup() {
        let popup = document.getElementById('thanksModal');

        popup.style.display = "none";
    };
</script>

<div id="thanksModal" class="modal">
        <div class="modal-content">
            <div class="row jutify-content-end">
                <div class="col">
                    <div class="modal-header">
                        <button type="button" on:click={closePopup} >&times</button>
                    </div>
                </div>
            </div>
            <div class="modal-body">
                <div class="row">
                    <div class="col">
                        <h2>
                            Спасибо за уделенное время! <br>
                            Совсем скоро Вам позвонит менеджер проекта!
                        </h2>
                    </div>
                </div>
                <hr>
                <div class="row">
                    <div class="col">
                        <div class="pop_up_bg">

                        </div>
                    </div>
                    <!-- <div class="col-4">

                    </div> -->
                </div>
                <div class="row">
                    <div class="col">
                        <p>
                            Вы можете воспользоваться скидкой сами или передарить ее коллегам, друзьям и партнерам <br>
                            На страницах наших социальных сетей, всегда есть актуальная и полезная игнформация для развития личных и бизнес компетенций <br>
                            Бизнес-лайфхаки, интересные статьи, рейтинги, аналитика и многое другое можно почитать на нашем <a href="https://uprav.ru/blog/">МЕДИАПОРТАЛЕ</a> 
                        </p>
                    </div>
                </div>
                <div class="row justify-content-center">
                    <div class="col">
                        <div class="wrapper_social">
                            <ul class="social__icon">
                                <li><a class="fb__icon" href="https://www.facebook.com/uprav" target="_blank"></a></li>
                                <li><a class="vk__icon" href="https://vk.com/rusuprav" target="_blank"></a></li>
                                <li><a class="inst__icon" href="https://www.instagram.com/rusuprav/" target="_blank"></a></li>
                                <li><a class="yt__icon" href="https://www.youtube.com/user/TheRSManagement" target="_blank"></a></li>
                                <li><a class="tg__icon" href=" https://web.telegram.org/#/im?p=@rusuprav" target="_blank"></a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</div>

  <style lang="scss">
      @import './style/theme.scss';

      h2{
          color: $colorWhite;
          font-size: 24px;
          font-family: $fbck;
          font-weight: bold;

          text-align: center;
      }

      #thanksModal {
        display: none; /* Скрыто по умолчанию */
        background-color: rgb(0,0,0); /* Затемнение фона */
        background-color: rgba(0,0,0,0.5); /* Полупрозрачное затемнение */
        z-index: 1; /* Фон на нижнем слое */
        overflow: auto; /* При необходимости, то появиться прокрутка */

        button{
            background-color: transparent;
            border: none;

            font-size: 20px;
        }
    }

    .modal-content {
        animation-name: animate;
        animation-duration: 0.5s;

        width: 50%;
        margin: auto;

        z-index: 2000;

        // margin-top: 5vh;
    }

    .modal-header{
        background-color: $darkBlue;
    }

    .modal-body{
        padding: 10%;
        background-color: $darkBlue;

        hr{
            height: 5px;
            color: $colorWhite;
            opacity: 1;
        }

        .pop_up_bg{
            background-image: url("/img/pop_up_bg.png");
            background-repeat: no-repeat;
            background-size: contain;

            height: 300px;
            width: 100%;
        }

        p{
            color: $colorWhite;
            font-size: 18px;
            font-family: $fbck;

            margin-top: 10px;

            a{
                color: $orange;
                text-decoration: none;
                transition: color .3s ease-in;
            }

            a:hover{
                color: #c27400;
            }
        }
    }

    .social__icon {

        text-align: center;

        padding-left: 0px;

        padding-top: 34px;

        li {
            display: block;
            padding-top: 10%;
            display: inline;

            padding-right: 30px;
        }

        li:first-child {
            padding-top: 0;
        }

        li:last-child{
            padding-right: 0px;
        }

        a {
            
            text-decoration: none;
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;

            padding: 15px;
            opacity: 1;

            animation: 0.3s ease-out social_icon_back;
        }



        .fb__icon {
            background-image: url(/img/soc_icon_fb.svg);
        }

        .vk__icon {
            background-image: url(/img/soc_icon_vk.svg);
        }

        .inst__icon {
            background-image: url(/img/soc_icon_inst.svg);
        }

        .yt__icon { 
            background-image: url(/img/soc_icon_yt.svg);
        }

        .tg__icon { 
            background-image: url(/img/soc_icon_tg.svg);
        }
    }

    .wrapper_social{
        margin: auto;
        display: block;
    }

    @keyframes animate {
        from {top:-300px; opacity:0}
        to {top:0; opacity:1}
    }
  </style>