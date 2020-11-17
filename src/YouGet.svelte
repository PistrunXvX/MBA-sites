<div class="container-fluid youGet__block">
    <h2>Что вы получаете</h2>
    <div class="container">
        <div class="row">
            <div class="col">
                <article class="first__block container__block">
                    <h3>Единый стандарт обучения</h3>
                    <p>
                        Ваши сотрудники формируют единый понятный аппарат, что позволяет сэкономить время
                        на неэффективных коммуникациях
                    </p>
                </article>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <article class="second__block container__block">
                    <h3>Широкая линейка программ</h3>
                    <p>
                        Благодаря большому количеству программ вы можете «закрыть» потребности обучения на
                        любом бизнес-направлении
                    </p>
                </article>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <article class="thirty__block container__block">
                    <h3>Эксперты-практики</h3>
                    <p>
                        Более 300 опытных преподавателей, прошедших внутреннюю сертификацию
                    </p>
                </article>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <article class="fouty__block container__block">
                    <h3>Гибкое расписание</h3>
                    <p>
                        Частота программ позволит обучать разных сотрудников 
                        по одной и той же тематике с регулярностью 
                        один раз в два месяца
                    </p>
                </article>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <article class="fifty__block container__block">
                    <h3>Экономия бюджета</h3>
                    <p>
                        Свыше 50% вашего бюджета может остаться на развитие важных бизнес-целей
                    </p>
                </article>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <article class="sixty__block container__block">
                    <h3>Багаж практических инструментов</h3>
                    <p>
                        Электронная версия презентаций и дополнительных материалов, с возможностью делиться и использовать в работе в постоянном режиме
                    </p>
                </article>
            </div>
        </div>
    </div>
</div>


<style lang="scss" >
    @import 'style/theme.scss';

    .youGet__block{

        h2{
            font-size: $blockTitleSize;
            font-family: $fbck;
            color: $darkBlue;
            text-align: center;
            text-transform: uppercase;

            margin-top: 5%;
        }

        article{
            
            font-family: $fbck;
            color: $darkBlue;

            margin-top: 20%;

            background-repeat: no-repeat;
            background-size: 150px;

            h3{
                font-size: 56px;
            }

            p{
                font-size: $description;
            }
        }

        .first__block, .thirty__block, .fifty__block{
            text-align: left;
            padding-right: 45%;
            background-position: 80% top;
        }

        .second__block, .fouty__block, .sixty__block{
            text-align: right;
            padding-left: 45%;
            background-position: 20% top;
        }

        .first__block{
            background-image: url(/img/education_icon_youGet.svg);
        }

        .second__block{
            background-image: url(/img/book_icon_youGet.svg);
        }
        
        .thirty__block{
            background-image: url(/img/atom_icon_youGet.svg);
        }

        .fouty__block{
            background-image: url(/img/research_icon_youGet.svg);
        }

        .fifty__block{
            background-image: url(/img/salary_icon_youGet.svg);
        }

        .sixty__block{
            background-image: url(/img/bag_icon_youGet.svg);
        }


        // .container__block{
        //     margin-right: 20%;
        // }
    }


</style>