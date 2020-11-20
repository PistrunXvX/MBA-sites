
    <div class="`">
        <div class="container-fluid">
        <div class="row justify-content-start">
            <div class="col-xl-7">

                <div class="about__block about__block-1 aboutUs">
                    <div class="about__block__title">
                        <h1 class="title__text">
                            Что это
                        </h1>
                    </div>
                    <div class="about__block_description ">
                        <p class="description__text">
                            Образовательный проект РШУ для компаний с <br> далекоидущими бизнес-планами. Вы сами
                            регулируете
                            процесс обучения своих сотрудников
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-fluid grey-color">
        <div class="row justify-content-end">
            <div class="col-xl-8">
                <div class="about__block about__block-2 aboutUs">
                    <div class="about__block__title">
                        <h1 class="title__text end">
                            Для чего 
                        </h1>
                    </div>
                </div>
            </div>
        </div>
        <div class="row justify-content-start">
            <div class="col-xl-7">

                <div class="about__block about__block-1 aboutUs">
                    <div class="about__block__title">
                        <h1 class="title__text">
                            Для кого
                        </h1>
                    </div>
                    <div class="about__block_description">
                        <p class="description__text">
                            Наши услуги ориентированы на собственников, топ-менеджмент, HR-специалистов и руководителей
                            функциональных подразделений
                        </p>
                    </div>
                </div>
            </div>
        </div>
        </div>
        </div>
        <div class="container-fluid grey-color">
        <div class="row justify-content-end">
            <div class="col-xl-6">
                <div class="container-fluid grey-color">
                <div class="about__block about__block-4 aboutUs">
                    <div class="about__block__title">
                        <h1 class="title__text end">
                            Выгода
                        </h1>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</div>





<style lang="scss">
    @import 'style/theme.scss';


    .container-fluid {
        padding: 0;
        margin: 0;
    }



    .aboutUs {
        color: $darkBlue;
        font-family: $fbck;
        padding: 78px 100px 61px 100px;




        .about__block {
            margin-bottom: 115px;
            position: relative;



        }

    }
        
    
    
    .about__block{
        margin-bottom:115px;
        position: relative;
    }

    .about__block-1::before{
        position: absolute;
        content:'';
        width:5px;
        height:60%;
        background-color: $orange;
        margin-left:-23px;
    }



    .about__block-2::before{
        position: absolute;
        content:'';
        width:5px;
        height:60%;
        background-color: $darkBlue;
       
        top: 25%;
        right: 5%;        
      
    }


    .about__block-4::before{
        position: absolute;
        content:'';
        width:5px;
        height:60%;
        background-color: $darkBlue;
       
        // margin-left: 102.5%;
        // top: 0;
        // left: 0;
        top: 25%;
        right: 5%;   
    }

           


    .end{
        text-align: right;
    }
            .des__link{
                color:$orange;
                text-decoration: none;
            }
</style>