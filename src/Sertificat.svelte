<div class="container-fluid sertificat__container" id="sertificats">
    <!-- <div class="container"> -->
        <h2>Лицензии и Сертификаты</h2>
        <div class="row justify-content-center">
            <div class="col-sm-12 col-md-12 col-lg-4">
                <div class="first__sertificat">
                    <a href="https://uprav.ru/about/#lg=1&slide=15"><img src="img/sertificat_img_1.jpg" class="img-fluid mx-auto d-block" alt="Лицензия на право ведения образовательной деятельности"></a>
                </div>
            </div>
            <div class="col-sm-12 col-md-12 col-lg-4">
                <div class="second__sertificat">
                    <a href="https://uprav.ru/about/#lg=1&slide=0"><img src="img/sertificat_img_2.jpg" class="img-fluid mx-auto d-block" alt="Сертификат соответсвия"></a>
                </div>
            </div>
            <div class="col-sm-12 col-md-12 col-lg-4">
                <div class="first__sertificat">
                    <a href="https://uprav.ru/about/#lg=1&slide=1"><img src="img/sertificat_img_3.jpg" class="img-fluid mx-auto d-block" alt="Сертификат соответсвия"></a>
                </div>
            </div>
        </div>
    <!-- </div> -->
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
            padding-top: 10%;
            width: 300px;

            animation: 0.3s ease-out animation__img__back;
        }
        
        img:hover{
            animation: 0.3s ease-in animation__img__to;
            transform: scale(1.1, 1.1);
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