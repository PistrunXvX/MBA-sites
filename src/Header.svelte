<div class="main__container">
    <div class="mobile__nav">
        <div class="collapse" id="navbarToggleExternalContent">
            <div class="bg-light p-4">
                <nav class="mobile__nav__menu">
                    <ul>
                        <li><a href="#">Главная</a></li>
                        <li><a href="#">О нас</a></li>
                        <li><a href="#">Подключиться</a></li>
                        <li><a href="#">Тарифы</a></li>
                        <li><a href="#">Преимущества</a></li>
                        <li><a href="#">Лицензии</a></li>
                        <li><a href="#">Контакты</a></li>
                    </ul>
                </nav>
            </div>
          </div>
          <nav class="navbar navbar-light bg-light">
            <div class="container-fluid">
              <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarToggleExternalContent" aria-controls="navbarToggleExternalContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="phone__nav">
                <a href="tel:+88001000203">+8 800-100-02-03</a>
              </div>
            </div>
          </nav>
    </div>
    <div class="container-fluid" id="main">
        <div class="row dekstop__nav">
            <div class="col">
                <nav>
                    <a href="tel:+88001000203" class="desc_number">8 800-100-02-03</a>
                    <ul>
                        <li><a href="#main">Главная</a></li>
                        <li><a href="#about_Us">О нас</a></li>
                        <li><a href="#connect_us">Подключиться</a></li>
                        <li><a href="#price">Тарифы</a></li>
                        <li><a href="#advantage">Преимущества</a></li>
                        <li><a href="#sertificats">Лицензии</a></li>
                        <li><a href="#contacts">Контакты</a></li>
                    </ul>
                </nav>
            </div>
        </div>
        <div class="row ">
            <div class="col-3 remove__sm align-self-center">
                <ul class="social__icon">
                    <li><a class="fb__icon" href="https://www.facebook.com/uprav" target="_blank"></a></li>
                    <li><a class="vk__icon" href="https://vk.com/rusuprav" target="_blank"></a></li>
                    <li><a class="inst__icon" href="https://www.instagram.com/rusuprav/" target="_blank"></a></li>
                    <li><a class="yt__icon" href="https://www.youtube.com/user/TheRSManagement" target="_blank"></a></li>
                    <li><a class="tg__icon" href=" https://web.telegram.org/#/im?p=@rusuprav" target="_blank"></a></li>
                </ul>
            </div>
            <div class="col-9">
                <div class="main__text emergence">
                    <h1>
                        Корпоративный онлайн-университет <br> на <span class="underline">аутсорсинг</span>
                    </h1>
                    <div class="sub__text emergence">
                        <p>
                            Доступ к 35 направлениям и 5000 тем для успешного ведения бизнеса
                        </p>
                        <a type="button" class="emergence" data-toggle="modal" data-target="#first__modal__header">Подать заявку</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>


<style lang="scss" >
    @import 'style/theme.scss';


    .emergence{
        animation: 2.1s ease-in-out 0s 1 alternate opacity;
    }
    @keyframes opacity{
        from{
            opacity: 0;
        }
        to{
            opacity: 1;
        }
    }
    
    ul{
        text-align: right;
    }

    nav{

        padding-left: 5%;
        padding-bottom: 2%;
        margin-top: 1%;

        .desc_number {
        text-decoration: none;
        color: $colorWhite;
        border-bottom: 1px solid $orange;
        transition: .3s;

        margin-left: 7%;

        float: left;

        font-size: 20px;
        font-family: $fbck;

        }

        .desc_number:hover {
            color: $orange;
            transition: .3s;
        }

            li{
            display: inline;
            padding-right: 3%;

            a{
                font-size: $headerLi;
                font-family: $fbck;
                color: $colorWhite;

                text-transform: uppercase;
                text-decoration: none;

                animation: 0.2s ease-out nav_color_back;
            }
        }

        a:hover{
            animation: 0.2s ease-out 0s nav_color_to;
            color: $orange;
        }
    }

    .dekstop__nav{
        background-image: url(/img/Logo_RSHU.svg);
        background-repeat: no-repeat;
        background-size: contain;
        background-position: 5% 0;
    }

    .main__container{
        background-image: url(/img/header_img.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        // background-attachment: fixed;
    }

    .main__text{
        margin-top: 10%;
        margin-bottom: 10%;

        padding-left: 40%;

        h1{
            font-size: 41px;
            font-family: $fbck;
            color: $colorWhite;
            line-height: 127%;

            text-transform: uppercase;
        }

        .underline{
            border-bottom: solid 2px $orange;
        }

        p{
            font-size: $formInputSize;
            font-family: $fbck;
            color: $colorWhite;
            line-height: 164%;

            padding-bottom: 5%;
        }

        a{
            font-size: 18px;
            font-family: $fbck;
            color: $colorWhite;

            text-decoration: none;

            background-color: $orange;
            filter: drop-shadow(0px 0px 10px $orange);

            padding: 20px 40px;
            animation: 0.3s ease-in 0s button_color_back;
        }

        a:hover{
            animation: 0.3s ease-in 0s button_color_to;
            color: $orange;
            background-color: $colorWhite;
            filter: drop-shadow(0px 0px 10px $colorWhite);
        }
    }

    .social__icon{

        text-align: left;

        li{
            display: block;
            padding-top: 20px;
        }

        li:first-child{
            padding-top: 0;
        }

        a{
            text-decoration: none;
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;

            padding: 15px;
            opacity: 1;

            animation: 0.2s ease-in 0s social_icon_back;
        }

        a:hover{
            animation: 0.2s ease-in 0s social_icon_to;
            opacity: 0.5;
        }

        a:active{
            opacity: 0.7;
        }

        .fb__icon{
            background-image: url(/img/soc_icon_fb.svg);
        }

        .vk__icon{
            background-image: url(/img/soc_icon_vk.svg);
        }

        .inst__icon{
            background-image: url(/img/soc_icon_inst.svg);
        }

        .yt__icon{
            background-image: url(/img/soc_icon_yt.svg);
        }

        .tg__icon{
            background-image: url(/img/soc_icon_tg.svg);
        }
    }

    .mobile__nav{
        display: none;
    }

    .mobile__nav .navbar{
        margin-top: 0;
    }

    .phone__nav a{
        padding-right: 200px;
        color: $darkBlue;
        font-family: $fbck;

        font-size: 20px;
    }

    .main__container .navbar{
        background-repeat: no-repeat;
        background-size: contain;
    }

    //Animation

    @keyframes social_icon_to{
            from{
                opacity: 1; 
            }
            to{
                opacity: 0.5;
            }
        }

        @keyframes social_icon_back{
            from{
                opacity: 0.5; 
            }
            to{
                opacity: 1;
            }
        }
    
        @keyframes nav_color_to{
            from{
                color: $colorWhite;
            } 
            to{
                color: $orange;
            }
        }
    
    @keyframes nav_color_back{
        from{
            color: $orange;
        }
        to{
            color: $colorWhite;
        }
    }

    @keyframes button_color_to{
        from{
            background-color: $orange;
            color: $colorWhite;
            filter: drop-shadow(0px 0px 10px $orange);
        }
        to{
            background-color: $colorWhite;
            color: $orange;
            filter: drop-shadow(0px 0px 10px $colorWhite);
        }
    }

    @keyframes button_color_back{
        from{
            background-color: $colorWhite;
            color: $orange;
            filter: drop-shadow(0px 0px 10px $colorWhite);
        }
        to{
            background-color: $orange;
            color: $colorWhite;
            filter: drop-shadow(0px 0px 10px $orange);
        }
    }
    

</style>