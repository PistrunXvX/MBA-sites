<div class="main__container">
    <div class="container-fluid">
        <div class="row">
            <div class="col">
                <nav>
                    <ul>
                        <li><a href="">Главная</a></li>
                        <li><a href="">О нас</a></li>
                        <li><a href="">Подключиться</a></li>
                        <li><a href="">Тарифы</a></li>
                        <li><a href="">Преимущества</a></li>
                        <li><a href="">Лицензии</a></li>
                        <li><a href="">Контакты</a></li>
                    </ul>
                </nav>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <div class="main-text">
                    <h1>
                        Корпоративный онлайн-университет на <span class="underline">аутсорсинг</span>
                    </h1>
                    <p>
                        Доступ к 35 направлениям и 5000 тем для успешного ведения бизнеса
                    </p>
                    <a href="#">Начать обучение</a>
                </div>
            </div>
        </div>
    </div>
</div>


<style lang="scss" >
    @import 'style/theme.scss';
    
    li{
        display: inline;

        a{
            font-size: $headerLi;
            font-family: $fbck;
            color: $colorWhite;

            text-transform: uppercase;
            text-decoration: none;
        }
    }

    .main__container{
        background-image: url(/img/header_img.jpg);
        background-size: cover;
        background-repeat: no-repeat;
    }

</style>