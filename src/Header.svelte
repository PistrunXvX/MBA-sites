<div class="main__container">
    <div class="container-fluid">
        <div class="row">
            <div class="col">
                <nav>
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
        <div class="row">
            <div class="col-2">
                <ul class="social__icon">
                    <li><a class="fb__icon" href="#"></a></li>
                    <li><a class="vk__icon" href="#"></a></li>
                    <li><a class="inst__icon" href="#"></a></li>
                    <li><a class="yt__icon" href="#"></a></li>
                </ul>
            </div>
            <div class="col-10">
                <div class="main__text">
                    <h1>
                        Корпоративный онлайн-университет <br> на <span class="underline">аутсорсинг</span>
                    </h1>
                    <div class="sub__text">
                        <p>
                            Доступ к 35 направлениям и 5000 тем для успешного ведения бизнеса
                        </p>
                        <a href="#">Подать заявку</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>


<style lang="scss" >
    @import 'style/theme.scss';
    
    ul{
        text-align: right;
    }

    nav{
        background-image: url(/img/Logo_RSHU.svg);
        background-repeat: no-repeat;
        background-size: contain;
        background-position: 5% 0;

        padding-left: 5%;
        padding-bottom: 2%;
        margin-top: 1%;

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

    .main__container{
        background-image: url(/img/header_img.jpg);
        background-size: cover;
        background-repeat: no-repeat;
    }

    .main__text{
        margin-top: 10%;
        margin-bottom: 10%;

        padding-left: 40%;

        h1{
            font-size: $mainText;
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
        margin-top: 50%;

        li{
            display: block;
            padding-top: 10%;
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