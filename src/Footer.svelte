<div class="footer_container">
    <div class="container-fluid">
        <div class="row justify-content-between">
        <div class="col-xl-7">
            <nav class="nav_footer">
                <li class="nav_item"><a href="#">Главная</a></li>
                <li class="nav_item"><a href="#">О нас</a></li>
                <li class="nav_item"><a href="#">Подключиться</a></li>
                <li class="nav_item"><a href="#">Тарифы</a></li>
                <li class="nav_item"><a href="#">Преимущества</a></li>
                <li class="nav_item"><a href="#">Лицензии</a></li>
                <li class="nav_item"><a href="#">Контакты</a></li>
            </nav>
        </div>
            <div class="col-xl-3">
                <div class="contacts_block">
                    <span class="title">
                        Контакты
                    </span>
                    <span class="desc">г. Москва, м.Ботанический сад/м.ВДНХ,
                        ул. Сельскохозяйственная, д.17, к. 5
                        тел.: <a href="#" class="desc_number">+7(495) 980-57-28</a></span>
                </div>
            </div>
     </div>

    



        <div class="row justify-content-between">
            <div class="col-xl-6">
                <div class="about_block">
                    <img src="/img/Logo_RSHU_footer.png" alt="Logo" class="img-fluid logo" />
                            
                    <div class="about_block__content">

                        <div class="first__stroke">

                           <span class="first__stroke_text">© Русская Школа Управления, 2002-2020. Все права защищены и охраняются законом.
                                Все содержание курсов обучения, семинаров, тренингов, представленных на сайте www.uprav.ru, является уникальным и принадлежит РШУ.
                           </span> 

                        </div>


                        <div class="second-stroke">
                            <span class="licenses">
                                Лицензия на образовательную деятельность № 029045, № 040697 
                            </span>
                        </div>

                            <div class="politics">
                                <span class="politics_text"><a href="#"> Политика конфиденциальности</a></span>
                            </div>

                    </div>

                        

                </div>
            </div>

                    <div class="col-xl-3">
                        <div class="social">
                            <div class="social_title">
                                <span class="social_title__text">
                                    Мы в соцсетях
                                </span>
                            </div>

            
                            <ul class="social__icon">
                                <li><a class="fb__icon" href="#"></a></li>
                                <li><a class="vk__icon" href="#"></a></li>
                                <li><a class="inst__icon" href="#"></a></li>
                                <li><a class="yt__icon" href="#"></a></li>
                            </ul>
                            

                        </div>
                    </div>


        </div>

    </div>
</div>


























<style lang="scss" >
    @import 'style/theme.scss';


    .footer_container{
        font-family: $fbck;
        padding-top:74px;
        padding-left:3.5%;
        padding-right:3.5%;
        background-color:#EEF0F2;

    }

        .nav_footer{
            
            font-size: $headerLi;
            list-style:none;
            text-transform: uppercase;
            font-weight: normal;
            letter-spacing: 0.1em;
            color:$darkBlue;
            padding-bottom:129px;

        }


        li{
            display: inline;
        }

        .nav_footer a{
            text-decoration: none;
            color:$darkBlue;
            transition: .3s;

        }

        .nav_footer a:hover{
            transition: .3s;
            color:$orange;
        }


        .nav_item:not(:last-child){

            padding-right:4%;
            
        }

        .logo{
            padding-bottom:17px;
        }

        .first__stroke{
            padding-bottom: 20px;
        }
        .first__stroke_text{
            font-size: 12px;
            color: #818486;
            letter-spacing: 0.1em;
            font-weight: normal;
            
        }


        .second-stroke{
            padding-bottom: 13px;
        }

        .licenses{
            color:#9C9FA1;
            font-size: 12px;
            font-weight: normal;

        }


        .politics{
            padding-bottom: 30px;
        }

        .politics_text{
            color: #818486;
            font-size: 18px;
            line-height: 164.06%;
            

        }

        .politics_text a{
            color: #818486;
            text-decoration: none;
            transition: .3s;
            border-bottom: 2px solid #818486;
            

        }

        .politics_text a:hover{
            color:$orange;
            transition: .3s;
            border-bottom-color: $orange;

        }


        .contacts_block{
            display: flex;
            flex-direction: column;
        }

        .title{
            color:#0C2967;
            font-size: 39px;
            font-weight: normal;
            line-height: 109.6%;
            padding-bottom: 14px;

        }

        .desc{
            color:#2C467C;
            font-size: 20px;
            font-weight: 200;
            letter-spacing: 0.11em;
            line-height: 178.1%;
        }

        .desc_number{
            text-decoration: none;
            color:#2C467C;
            border-bottom:1px solid $orange;
            transition: .3s;

        }

        .desc_number:hover{
            color:$orange;
            transition: .3s;
        }


        

            .social{
                padding-top: 35px;
                display: flex;
                justify-content: center;
                flex-direction: column;
                text-align: center;
            }




            .social__icon{

                    
                    padding-top: 34px;

li{
    display: block;
    padding-top: 10%;
    display: inline;
}

li:first-child{
    padding-top: 0;
}

a{
    text-decoration: none;
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center;

    padding: 15px;
    opacity: 1;

    
}



.fb__icon{
   
    
}

.vk__icon{
    
}

.inst__icon{
    
}

.yt__icon{
   
}
}





        .social_title__text{
            color: #0C2967;
            font-size: 42px;
            line-height: 109.6%;
        }



        

</style>