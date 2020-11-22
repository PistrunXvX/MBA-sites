<div class="advantage" id="advantage">
    <div class="container-fluid">
        <h2 class="title title__one">Преимущества</h2>
        <p class="title title__two">Корпоративного онлайн-университета</p>
        <div class="container">
            <div class="advantage__list">
                <div class="row justify-content-between">
                    <div class="col-xl-4 col-xs-10 col-sm-6 ">
                        <div class="advantage__list-item first_block">
                            <div class="list-item_title ">
                                <p class="title_text first_number">Работаем с 2002 года</p>
                            </div>
                            <div class="list-item_desc">
                                <p class="desc_text">У нас более 150 000 выпускников, мы сотрудничали более, чем с 15
                                    000 компаний, что
                                    показывает доверие клиентов к нам и профессионализм наших педагогов</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-xl-4  col-xs-10 col-sm-6 ">
                        <div class="advantage__list-item second_block">
                            <div class="list-item_title">
                                <p class="title_text second_number">Широкая линейка программ</p>
                            </div>
                            <div class="list-item_desc">
                                <ul class="item-desc_content">
                                    <li class="desc_text"> - Более 30 направлений</li>
                                    <li class="desc_text"> - 1500 программ обучения
                                    <li class="desc_text"> - Постоянное развитие знаний и навыков</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row justify-content-center">
                    <div class="col-xl-4 col-xs-10 col-sm-6">
                        <div class="advantage__list-item third_block">
                            <div class="list-item_title">
                                <p class="title_text five_number">Гибкое расписание</p>
                            </div>
                            <div class="list-item_desc">
                                <p class="desc_text">Частота программ позволит обучать разных
                                    сотрудников по одной и той же тематике
                                    с регулярностью один раз в два месяца</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row justify-content-between">
                    <div class="col-xl-4 col-xs-10 col-sm-6 ">
                        <div class="advantage__list-item four_block">
                            <div class="list-item_title">
                                <p class="title_text third_number">Гарантия качества</p>
                            </div>
                            <div class="list-item_desc">
                                <ul class="item-desc_content third_item-desc_content">
                                    <li class="desc_text"> - Более 30 направлений</li>
                                    <li class="desc_text"> - 1500 программ обучения
                                    <li class="desc_text"> - Постоянное развитие знаний и навыков</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-xl-4 col-xs-10 col-sm-6 ">
                        <div class="advantage__list-item five_block">
                            <div class="list-item_title">
                                <p class="title_text four_number">Экономия бюджета</p>
                            </div>
                            <div class="list-item_desc ">
                                <p class="desc_text">
                                    Наши цены за тарифы значительно ниже,
                                    чем цены на курсы в образовательных центрах, при этом вы получаете в разы больше
                                    информации
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




    .advantage {
        background-image: url("/img/main_img_advantage.jpg");
        background-repeat: no-repeat;
        background-size: auto;
        background-position: center;
        width: 100%;
        height: 100%;
        font-family: $fbck;
        color: $darkBlue;
        margin-top: 257px;
        margin-bottom: 187px;



    }


    // .container{

    //     margin-top:260px;


    // }






    .title_text {
        font-size: $description;
        font-weight: normal;
        line-height: 99.56%;
        letter-spacing: -0.045em;
        position: relative;
    }



    .title_text::before {
        content: "05";

        font-weight: 800;
        font-size: 54px;
        line-height: 99.56%;
        padding-right: 13px;

        border-top: 3px solid $darkBlue;

    }

    .first_number::before {

        content: "01";
    }

    .second_number::before {
        content: "02";
    }

    .third_number::before {
        content: "03";
    }

    .four_number::before {
        content: "04";
    }

    .five_number::before {
        content: "05";
    }











    .desc_text {
        font-size: 24px;
        font-weight: normal;
        letter-spacing: -0.045em;
        line-height: 137.6%;
    }

    li {
        list-style-type: none;
    }

    .title {
        text-transform: uppercase;
        line-height: 200.06%;
        font-weight: normal;
        text-align: center;

        margin-right: 10%;
        margin-left: 10%;
        

        font-size: 70px;
    }

    .title__one {
        font-size: $blockTitleSize;
        padding-bottom: 13px;

    }

    .title__two {
        font-size: 60px;
        margin-bottom: 520px;

    }
    
</style>