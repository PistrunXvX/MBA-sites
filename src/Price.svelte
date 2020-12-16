<script>
    // window.addEventListener('DOMContentLoaded', function() {
    
    //     function setName(){
    //         buttonArray[0].textContent = 'Узнайте больше';
    //         console.log('test');
    //     };
    // });

    // let arrayButton = document.querySelectorAll('.month__price');

        function setName_1(){
            document.querySelector('.first__month').textContent = 'Подробнее';
        };

        function setName_2() {
            document.querySelector('.second__month').textContent = 'Подробнее';
        };

        function setName_3() {
            document.querySelector('.third__month').textContent = 'Подробнее';
        };

        
        function returnName_1(){
            document.querySelector('.first__month').textContent = '3 месяца';
        };

        function returnName_2() {
            document.querySelector('.second__month').textContent = '6 месяцев';
        };

        function returnName_3() {
            document.querySelector('.third__month').textContent = '12 месяцев';
        };

</script>

<div class="container-fluid price__block row-flex" id="price">
    <div class="container text-center">
        <h2>Три тарифа</h2>
    </div>
    <div class="row justify-content-evenly card_container">
        <div class="col-xxl-3 col-xl-4 col-lg-4 col-md-7 col-sm-8 wrapper__price">
            <article class="first__price price-card_animation" on:mouseover={setName_1} on:mouseout={returnName_1}>
                <h3>Базовый</h3>
                <p class="text__price">
                    5 подключений* в день
                    к платформе онлайн-
                    трансляции
                </p>
                <button type="button" data-toggle="modal" data-target="#first__vertical__popup" class="month__price first__month">
                    3 месяца
                </button>
                <p class="salary__price">
                    150 000 р.
                </p>
            </article>
        </div>
        <div class="col-xxl-3 col-xl-4 col-lg-4 col-md-7 col-sm-8 wrapper__price"> 
            <article class="second__price price-card_animation" on:mouseover={setName_2} on:mouseout={returnName_2}>
                <h3>Расширенный</h3>
                <p class="text__price">
                    10 подключений* в день
                    к платформе онлайн-
                    трансляции
                </p>
                <button type="button" data-toggle="modal" data-target="#second__vertical__popup" class="month__price second__month">
                    6 месяцев
                </button>
                <p class="salary__price">
                    300 000 р.
                </p>
            </article>
        </div>
        <div class="col-xxl-3 col-xl-4 col-lg-4 col-md-7 col-sm-8 wrapper__price">
            <article class="thirty__price price-card_animation" on:mouseover={setName_3} on:mouseout={returnName_3}>
                <h3>Безлимитный</h3>
                <p class="text__price">
                    неограниченное количество
                    подключений в день
                    <!-- к платформе онлайн-
                    трансляции -->
                </p>
                <button type="button" data-toggle="modal" data-target="#third__vertical__popup" class="month__price third__month">
                    12 месяцев
                </button>
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

        .price-card_animation{
            transition:transform 0.3s ease-in-out;
                
        }
        .price-card_animation:hover{
            fill:#EA8E02;
            transform:scale(1.05) translateY(-5%);
            transition:transform 0.3s ease-in-out;
        }


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
             background-size: 80px 80px;

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
                 transition: 0.3s;
                
                 text-transform: uppercase;

                 padding: 20px 50px;

                 background-color: $darkBlue;
                 border-radius: 50px;
                 border: none;
                 box-shadow: none;
             }

             
                .month__price:hover{
                    background-color: $orange;
                    box-shadow: 0px 0px 20px $orange;
                    transition: 0.3s;
                }

             .salary__price{
                 font-size: $description;
                 color: $darkBlue;

                 margin-top: 10%;
             }
         }

         .first__price{
             background-image: url(/img/star_icon_price.png);
             background-position: center 10%;
         }

         .second__price{
            background-image: url(/img/star_icon_price.png),
                              url(/img/star_icon_price.png);
            background-position: 40% 10%, 60% 10%;
         }

         .thirty__price{
            background-image: url(/img/star_icon_price.png),
                              url(/img/star_icon_price.png),
                              url(/img/star_icon_price.png);
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






