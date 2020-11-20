<div class="aboutUs">
    <div class="container-fluid">
        <div class="row justify-content-start">
            <div class="col-xl-7">
                <div class="about__block about__block-1">
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
                    <div class="about__block about__block-2">
                        <div class="about__block__title">
                            <h1 class="title__text end">
                                Для чего
                            </h1>
                        </div>
                        <div class="about__block_description">
                            <p class="description__text end">
                                Вы создаете кадровый резерв для развития компании
                                Растет результативность каждого сотрудника и компании в целом
                                Обучение формирует корпоративную культуру и репутацию компании
                                Вы повышеаете стоимость и статус компании для привлечения инвестиций
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="row justify-content-start">
            <div class="col-xl-7">

                <div class="about__block about__block-1">
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
        <div class="container-fluid grey-color">
            <div class="row justify-content-end">
                <div class="col-xl-6">
                    <div class="container-fluid grey-color">
                        <div class="about__block about__block-4">
                            <div class="about__block__title">
                                <h1 class="title__text end">
                                    Выгода
                                </h1>
                            </div>
                            <div class="about__block_description">
                                <p class="description__text end">
                                    Покупать курсы отдельно не нужно: достаточно выбрать и оплатить подходящий тариф,
                                    чтобы
                                    <a href="#" class="des__link">получить доступ к более 1500 обучающих программ</a>
                                </p>
                            </div>
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

        .about__block-1::before {
            position: absolute;
            content: '';
            width: 5px;
            height: 100%;
            background-color: $orange;
            margin-left: -23px;





        }



        .about__block-2::after {
            position: absolute;
            content: '';
            width: 5px;
            height: 100%;
            background-color: $darkBlue;

            margin-left: 102.5%;
            top: 0;
            left: 0;




        }

        .grey-color {

            background-color: #EEF0F2;
        }

        .about__block-4::after {
            position: absolute;
            content: '';
            width: 5px;
            height: 100%;
            background-color: $darkBlue;

            margin-left: 102.5%;
            top: 0;
            left: 0;




        }

        .title__text {
            font-size: $blockTitleSize;




        }

        .description__text {
            font-size: $description;
        }

        .end {
            text-align: right;
        }

        .des__link {
            color: $orange;
            text-decoration: none;
        }
    }
</style>