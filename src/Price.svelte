<div class="container-fluid price__block row-flex">
    <div class="container text-center">
        <h2>Три тарифа</h2>
    </div>
    <div class="row justify-content-evenly">
        <div class="col-xl-3 col-lg-4 col-md-7 col-sm-8 price__wrapper">
            <article class="first__price ">
                <h3>Базовый</h3>
                <p class="text__price">
                    5 подключений* в день
                    к платформе онлайн-
                    трансляции
                </p>
                <span class="month__price">
                    3 месяца
                </span>
                <p class="salary__price">
                    150 000 р.
                </p>
            </article>
        </div>
        <div class="col-xl-3 col-lg-4 col-md-7 col-sm-8 price__wrapper"> 
            <article class="second__price">
                <h3>Расширенный</h3>
                <p class="text__price">
                    10 подключений* в день
                    к платформе онлайн-
                    трансляции
                </p>
                <span class="month__price">
                    6 месяцев
                </span>
                <p class="salary__price">
                    300 000 р.
                </p>
            </article>
        </div>
        <div class="col-xl-3 col-lg-4 col-md-7 col-sm-8 price__wrapper">
            <article class="thirty__price">
                <h3>Безлимитный</h3>
                <p class="text__price">
                    неограниченное количество
                    подключений в день
                    к платформе онлайн-
                    трансляции
                </p>
                <span class="month__price">
                    12 месяцев
                </span>
                <p class="salary__price">
                    1 500 000 р.
                </p>
            </article>
        </div>
        <p class="remark">
            *Всего 5 подключений в день к платформе онлайн-трансляции
        </p>
    </div>
</div>

<style lang="scss" >
    @import 'style/theme.scss';

    .price__block{
       
        
        flex-wrap: wrap;

         h2{
            font-size: $blockTitleSize;
            font-family: $fbck;
            color: $darkBlue;

            text-transform: uppercase;
            text-align: center;

            margin-top: 5%;
            margin-bottom:95px;
         }

         .first__price, .second__price, .thirty__price{
            height: 100%;

             background-repeat: no-repeat;
             background-size: 90px 90px;

             border: 10px solid $darkBlue;
             margin-top: 5%;
             padding-top: 200px;
                
             font-family: $fbck;
             text-align: center;

             h3{
                 font-size: $mainText;
                 color: $darkBlue;
             }

             .text__price{
                 font-size: $formInputSize;
                 color: $darkBlue;
                 margin-left: 20%;
                 margin-right: 20%;
                 margin-bottom: 10%;
                 margin-top: 10%;
             }

             .month__price{
                 font-size: $description;
                 color: $colorWhite;
                
                 text-transform: uppercase;

                 padding: 20px 50px;

                 background-color: $darkBlue;
                 border-radius: 50px;
             }

             .salary__price{
                 font-size: $description;
                 color: $darkBlue;

                 margin-top: 10%;
             }
         }

         .first__price{
             background-image: url(/img/star_icon_price.svg);
             background-position: center 10%;
         }

         .second__price{
            background-image: url(/img/star_icon_price.svg),
                              url(/img/star_icon_price.svg);
            background-position: 40% 10%, 60% 10%;
         }

         .thirty__price{
            background-image: url(/img/star_icon_price.svg),
                              url(/img/star_icon_price.svg),
                              url(/img/star_icon_price.svg);
            background-position: 35% 10%, 50% 5%, 65% 10%;
         }
    }

    .remark{
        font-size: $description;
        font-family: $fbck;
        color: $darkBlue;

        text-align: center;

        margin-top: 5%;
    }


       .row-flex {
         display: -webkit-box;
         display: -ms-flexbox;
            display: flex;
         -ms-flex-wrap: wrap;
            flex-wrap: wrap;
          }

    [class*=”col-”] {
    margin-bottom: 30px;
    }
    .content {
        height: 100%;
        padding: 20px 20px 10px;
        color: #fff;
    }

   
</style>






