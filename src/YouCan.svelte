<div class="container-fluid youCan__main">
    <h2>Вы сможете</h2>
    <div class="row">
        <div class="col-lg-4 col-md-12 col-sm-12 first__block youCan__block">
            <p>
                Не тратить время на поиск <br> провайдера образовательных <br> услуг
            </p>
        </div>
        <div class="col-lg-4 col-md-12 col-sm-12 second__block youCan__block">
            <p>
                Обеспечить непрерывное обучение
                и развитие персонала <br> самостоятельно составив график
            </p>
        </div>
        <div class="col-lg-4 col-md-12 col-sm-12 thirty__block youCan__block">
            <p>
                Всегда получать актуальные <br> знания, которые используют на <br> практике более 300 экспертов
            </p>
        </div>
    </div>
</div>

<style lang="scss" >
    @import 'style/theme.scss';
   

    .youCan__main{

        border-bottom:10px solid $orange;
        padding-bottom:100px;

        

        background-image: url(/img/linear_img_youCan.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        background-attachment: fixed;

        h2{
            font-size:$blockTitleSize;
            font-family: $fbck;
            color: $colorWhite;

            text-align: center;
            text-transform: uppercase;
            padding-top: 3%;
        }
        
        .youCan__block{
            font-size: $description;
            font-family: $fbck;
            color: $colorWhite;

            text-align: center;

            padding-top: 10%;
            margin-top: 5%;

            background-repeat: no-repeat;
            background-size: 170px;
            background-position: top center;

            p{
                padding-top: 50px;
            }
        }

        .youCan__block:last-child{
            margin-right: 0;
        }

        .first__block{
            background-image: url(/img/clock_icon_youCan.svg);
        }

        .second__block{
            background-image: url(/img/dekstop_icon_youCan.svg);
        }

        .thirty__block{
            background-image: url(/img/stonck_icon_youGet.svg);
        }
        
    }

</style>