<div class="footer_container" id="contacts">
    <div class="container-fluid">
        <div class="row justify-content-between">
            <div class="col-xl-7 col-xs-12 col-md-6 col-lg-8">
                <nav class="nav_footer navbar justify-content-center ">
                    <li class="nav_item"><a href="#main">Главная</a></li>
                    <li class="nav_item"><a href="#about_Us">О нас</a></li>
                    <li class="nav_item"><a href="#connect_us">Подключиться</a></li>
                    <li class="nav_item"><a href="#price">Тарифы</a></li>
                    <li class="nav_item"><a href="#advantage">Преимущества</a></li>
                    <li class="nav_item"><a href="#sertificats">Лицензии</a></li>
                    <li class="nav_item"><a href="#contacts">Контакты</a></li>
                </nav>
            </div>
            <div class="col-xl-3 col-xs-12 col-md-6 col-lg-4">
                <div class="contacts_block">
                    <span class="title">
                        Контакты
                    </span>
                    <span class="desc">г. Москва, м.Ботанический сад/м.ВДНХ, <br>
                        ул. Сельскохозяйственная, д.17/5 <br>
                        тел.: <a href="tel:+74959805728" class="desc_number">+7(495) 980-57-28</a></span>
                </div>
            </div>
        </div>
        <div class="row justify-content-between">
            <div class="col-xl-6">
                <div class="about_block">
                    <img src="/img/Logo_RSHU_footer.png" alt="Logo" class="img-fluid logo" />
                    <div class="about_block__content">
                        <div class="first__stroke">
                            <span class="first__stroke_text">© Русская Школа Управления, 2002-2020. Все права защищены и
                                охраняются законом.
                                Все содержание курсов обучения, семинаров, тренингов, представленных на сайте
                                www.uprav.ru, является уникальным и принадлежит РШУ.
                            </span>
                        </div>
                        <div class="second-stroke">
                            <span class="licenses">
                                Лицензия на образовательную деятельность № 029045, № 040697
                            </span>
                        </div>
                        <div class="politics">
                            <span class="politics_text"><a href="/img/politika_peda.pdf" target="_blank"> Политика конфиденциальности</a></span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-xl-3">
                <div class="social">
                    <div class="social_title">
                        <span class="social_title__text">
                            Мы в соцсетях
                        </span>
                    </div>
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


<style lang="scss">
    @import 'style/theme.scss';


    .footer_container {
        font-family: $fbck;
        padding-top: 74px;
        padding-left: 3.5%;
        padding-right: 3.5%;
        background-color: #EEF0F2;

    }

    .nav_footer {

        font-size: $headerLi;
        list-style: none;
        text-transform: uppercase;
        font-weight: normal;
        letter-spacing: 0.1em;
        color: $darkBlue;
        padding-bottom: 129px;

    }


    li {
        display: inline;
    }

    .nav_footer a {
        text-decoration: none;
        color: $darkBlue;
        transition: .3s;

    }

    .nav_footer a:hover {
        transition: .3s;
        color: $orange;
    }


    .nav_item:not(:last-child) {

        padding-right: 4%;

    }

    .logo {
        padding-bottom: 17px;
    }

    .first__stroke {
        padding-bottom: 20px;
    }

    .first__stroke_text {
        font-size: 12px;
        color: #818486;
        letter-spacing: 0.1em;
        font-weight: normal;

    }


    .second-stroke {
        padding-bottom: 13px;
    }

    .licenses {
        color: #9C9FA1;
        font-size: 12px;
        font-weight: normal;

    }


    .politics {
        padding-bottom: 30px;
    }

    .politics_text {
        color: #818486;
        font-size: 18px;
        line-height: 164.06%;


    }

    .politics_text a {
        color: #818486;
        text-decoration: none;
        transition: .3s;
        border-bottom: 2px solid #818486;


    }

    .politics_text a:hover {
        color: $orange;
        transition: .3s;
        border-bottom-color: $orange;

    }


    .contacts_block {
        display: flex;
        flex-direction: column;
    }

    .title {
        color: #0C2967;
        font-size: 39px;
        font-weight: normal;
        line-height: 109.6%;
        padding-bottom: 14px;

    }

    .desc {
        color: #2C467C;
        font-size: 20px;
        font-weight: 200;
        letter-spacing: 0.11em;
        line-height: 178.1%;
    }

    .desc_number {
        text-decoration: none;
        color: #2C467C;
        border-bottom: 1px solid $orange;
        transition: .3s;

    }

    .desc_number:hover {
        color: $orange;
        transition: .3s;
    }




    .social {
        padding-top: 35px;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
    }




    .social__icon {

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
            background-image: url(/img/soc_icon_blue_fb.svg);
        }

        .vk__icon {
            background-image: url(/img/soc_icon_blue_vk.png);
        }

        .inst__icon {
            background-image: url(/img/soc_icon_blue_inst.svg);
        }

        .yt__icon { 
            background-image: url(/img/soc_icon_blue_yt.png);
        }

        .tg__icon { 
            background-image: url(/img/soc_icon_blue_tg.svg);
        }
    }

    .social_title__text {
        color: #0C2967;
        font-size: 42px;
        line-height: 109.6%;
    }

    .social__icon a:hover{
        animation: 0.3s ease-in social_icon_to;
        opacity: 0.5;
    }

    .social__icon a:active{
        opacity: 0.7;
    }

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
</style>