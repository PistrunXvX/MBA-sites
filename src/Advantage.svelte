<script>
    window.addEventListener('DOMContentLoaded', function() {
        let widthWindow = window.innerWidth;
        console.log(typeof(widthWindow));

        let numberTo3 = document.querySelector('.title_text_anim_5');
        let numberTo4 = document.querySelector('.title_text_anim_3');
        let numberTo5 = document.querySelector('.title_text_anim_4');

        if (widthWindow < 960) {
            numberTo3.textContent = "03";
            numberTo4.textContent = "04";
            numberTo5.textContent = "05";
        }

    
        let windowHWidth = document.documentElement.clientWidth;
    console.log(windowHWidth);
    if (windowHWidth < 1400 ) {
        let elem = document.querySelector('.advantage');
        elem.classList.add('container');
    } else {
        elem.classList.remove('container');
    }
    });

</script>

<div class="advantage" id="advantage">
    <div class="container-fluid">
        <h2 class="title title__one">Преимущества</h2>
        <p class="title title__two">Корпоративного онлайн-университета</p>
        <div class="container">
            <div class="advantage__list">
                <div class="row justify-content-between">
                    <div class="col-xl-4 col-xs-10 col-sm-10 ">
                        <div class="advantage__list-item first_block">
                            <div class="list-item_title ">
                                <p class="title_text"><span class="title_text_number title_text_anim_1">01</span>Работаем с 2002 года</p>
                            </div>
                            <div class="list-item_desc">
                                <p class="desc_text">
                                    <!-- У нас более 150 000 выпускников, мы сотрудничали более, чем с 15
                                    000 компаний, что
                                    показывает доверие клиентов к нам и профессионализм наших педагогов -->
                                    Более 150 000 выпускников и 15 000 компаний
                                    доверяют нам и профессионализму наших экспертов

                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="col-xl-4  col-xs-10 col-sm-10 ">
                        <div class="advantage__list-item second_block">
                            <div class="list-item_title">
                                <p class="title_text"><span class="title_text_number title_text_anim_2">02</span>Системный подход</p>
                            </div> 
                            <div class="list-item_desc">
                                <!-- <ul class="item-desc_content">
                                    <li class="desc_text"> Более 30 направлений</li>
                                    <li class="desc_text"> 1500 программ обучения
                                    <li class="desc_text"> Постоянное развитие знаний и навыков</li>
                                </ul> -->
                                <p class="desc_text">
                                    Планирование, организация и контроль
                                    - определяющие факторы эффективности обучения
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row justify-content-center">
                    <div class="col-xl-4 col-xs-10 col-sm-10 ">
                        <div class="advantage__list-item third_block">
                            <div class="list-item_title">
                                <p class="title_text five_number"><span class="title_text_number title_text_anim_5">05</span>Стабильность обучения</p>
                            </div>
                            <div class="list-item_desc">
                                <p class="desc_text">
                                    <!-- Частота программ позволит обучать разных
                                    сотрудников по одной и той же тематике
                                    с регулярностью один раз в два месяца -->
                                    Непрерывное обучение в течение 
                                    календарного года 
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row justify-content-between">
                    <div class="col-xl-4 col-xs-10 col-sm-10 ">
                        <div class="advantage__list-item four_block">
                            <div class="list-item_title">
                                <p class="title_text third_number"><span class="title_text_number title_text_anim_3">03</span>Гарантия качества</p>
                            </div>
                            <div class="list-item_desc">
                                <ul class="item-desc_content third_item-desc_content">
                                    <li class="desc_text">Сертификат ГОСТ Р ИСО 9001-2015</li>
                                    <li class="desc_text"> Лицензия на образовательную деятельность</li>
                                    <li class="desc_text">Постоянная актуализация информации</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-xl-4 col-xs-10 col-sm-10  ">
                        <div class="advantage__list-item five_block">
                            <div class="list-item_title">
                                <p class="title_text four_number"><span class="title_text_number title_text_anim_4">04</span>Доступность обучения</p>
                            </div>
                            <div class="list-item_desc ">
                                <p class="desc_text">
                                    <!-- Наши цены за тарифы значительно ниже,
                                    чем цены на курсы в образовательных центрах, при этом вы получаете в разы больше
                                    информации -->
                                    Линейка программ для всех уровней и 
                                    категорий сотрудников компании
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
        background-image: url("/img/main_img_advantage.webp");
        background-repeat: no-repeat;
        background-size: auto;
        background-position: center;
        width: 100%;
        height: 100%;
        font-family: $fbck;
        color: $darkBlue;
        // margin-top: 157px;
        margin-bottom: 50px;



    }

    .title_text {
        font-size: $description;
        font-weight: normal;
        line-height: 99.56%;
        letter-spacing: -0.045em;
        position: relative;
    }



    .title_text_number{
        font-weight: 800;
        font-size: 54px;
        line-height: 99.56%;
        padding-right: 13px;

        border-top: 3px solid $darkBlue;

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
        padding-top: 100px;

    }

    .title__two {
        font-size: 55px;
        margin-bottom: 420px;

    }
    
</style>