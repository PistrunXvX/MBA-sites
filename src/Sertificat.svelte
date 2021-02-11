<div class="container-fluid sertificat__container" id="sertificats">
    <div class="container">
        <h2>Лицензии и Сертификаты</h2>
        <div class="row justify-content-center">
            <div class="col-sm-12 col-md-12 col-lg-4">
                <div class="first__sertificat sertificat">
                    <a href="https://uprav.ru/about/#lg=1&slide=15">
                        <picture>
                            <source srcset="img/sertificat_img_1.webp" type="image/webp">
                            <img src="img/sertificat_img_1.jpg" class="img-fluid mx-auto d-block" alt="Лицензия на право ведения образовательной деятельности">
                        </picture>
                    </a>
                    <p>
                        Лицензия на право ведения образовательной деятельности
                    </p>
                </div>
            </div>
            <div class="col-sm-12 col-md-12 col-lg-4">
                <div class="second__sertificat sertificat">
                    <a href="https://uprav.ru/about/#lg=1&slide=0">
                        <picture>
                            <source srcset="img/sertificat_img_2.webp" type="image/webp">
                            <img src="img/sertificat_img_2.jpg" class="img-fluid mx-auto d-block" alt="Сертификат соответсвия">
                        </picture>
                    </a>
                    <p>
                        Сертификат соответсвия
                    </p>
                </div>
            </div>
            <div class="col-sm-12 col-md-12 col-lg-4">
                <div class="first__sertificat sertificat">
                    <a href="https://uprav.ru/about/#lg=1&slide=1">
                        <picture>
                            <source srcset="img/sertificat_img_3.webp" type="image/webp">
                            <img src="img/sertificat_img_3.jpg" class="img-fluid mx-auto d-block" alt="Сертификат соответсвия">
                        </picture>
                    </a>
                    <p>
                        Сертификат соответсвия
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>

<style lang="scss" >
    @import 'style/theme.scss';

    .sertificat__container{

        background-color: $grey;

        padding-bottom: 5%;
        
        h2{
            font-size: $blockTitleSize;
            font-family: $fbck;
            color: $darkBlue;

            text-align: center;
            text-transform: uppercase;

            padding-top: 5%;
            margin-bottom: 57px;
        }

        img{
            width: 300px;

            animation: 0.3s ease-out animation__img__back;

            border-style: solid;
            border-width: 20px 20px 20px 20px;
            -moz-border-image: url(/img/border_sertificat.png) 15 15 15 15;
            -webkit-border-image: url(/img/border_sertificat.png) 15 15 15 15;
            -o-border-image: url(/img/border_sertificat.png) 15 15 15 15;
            border-image: url(/img/border_sertificat.png) 15 15 15 15;
        }
        
        img:hover{
            animation: 0.3s ease-in animation__img__to;
            transform: scale(1.1, 1.1);
        }

        .sertificat{
            padding-top: 10%;

            p{
                font-size: 18px;
                color: $darkBlue;
                font-family: $fbck;

                text-align: center;

                padding-top: 50px;
            }
        }
    }

    @keyframes animation__img__to{
        from{
            transform: scale(1,1);
        }
        to{
            transform: scale(1.1, 1.1);
        }
    }

    @keyframes animation__img__back{
        from{
            transform: scale(1.1,1.1);
        }
        to{
            transform: scale(1, 1);
        }
    }

</style>