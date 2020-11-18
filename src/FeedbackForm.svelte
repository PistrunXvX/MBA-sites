



    
   
 
    <div class="form-container">
    <div class="container-fluid">
        <div class="row align-items-center">

            <div class="col-xl-7">

                <div class="text-block">

                    <h2 class="text-block_content">
                        Всегда важно понять, кто ведёт обучение и как проходят занятия - с радостью пришлём
                        вам один из модулей

                    </h2>

                </div>

            </div>



            <div class="col-xl-5">
                <div class="form-block">
                    <div class="row align-items-center">
                    <div class="col-xl-6">

                    
                    <input type="text" class="form-control form__name" placeholder="Ваше имя" require>
                </div>
                <div class="col-xl-6">
                    <input type="text" class="form-control form__send__number" id="tel" placeholder="Ваш телефон" require>
                </div>
                 </div>

                 
                    <input type="email" class="form-control  form_send__email" placeholder="Ваш электронный адрес" require>
                   <label class="label">
                    <input type="checkbox" class="checkbox">
                    <span class="fake"></span>
                    <span class="p">Я согласен с <a href="#" class="link"> политикой конфиденциальности</a></span>
                   </label>
                   
                </div>
                <button class=" form__btn" type="submit">Отправить</button>
            </div>
        </div>
    </div>
</div>




<style lang="scss">
    @import 'style/theme.scss';



    .form-container{
        display: flex;
        align-items:center;
        background-color:$darkBlue;
        padding-top:100px;
        padding-bottom:90px;
        padding-left:80px;
        padding-right:80px;


        .text-block_content{
            font-family: $fbck;
            font-size: 39px;
            color:$colorWhite;
        }

     
        
        .text-block{
             padding-right:216px;
             
            
        }


        .form__name{
           
            margin-bottom:39px;
        }

        .form__send__number{
            margin-bottom:39px;
        }

        .form_send__email{
            margin-top:0px;
            margin-bottom:39px;
            
        }


        .checkbox{
            margin-bottom: 83px;
        }

        .form-control{
            padding:22px 30px;
            background-color:$darkBlue;
           
            border: 4px solid $colorWhite;
           
            font-size: 25px;
            color:$colorWhite;

        }

        .form-control::placeholder{
            color:#D3D3D3;
        }


        .form-control:focus, .form-control:active{
            color:$colorWhite;
        }


        

            .form-block{

                



                .p{
                    color:$colorWhite;
                    font-size: $formInputSize;
                    padding-left:30px;
                    padding-bottom:91px;
                    
                }

            }


            .link{
                color:$colorWhite;
                text-decoration: none;
                border-bottom: 3px solid $orange;
            }

           
           
            
            .label{
                display: flex;
                justify-content: start;
            }
            
            .checkbox{
                display:none;
            }

            .fake{
                display:inline-block;
                width:40px;
                height:40px;
                border:5px solid $colorWhite;
                position: relative;
                
                

            }

            .fake::before{
                content:'';
                position: absolute;
                display:block;
                width:15px;
                height:15px;
                background-color:$orange;
                top:50%;
                left:50%;
                transform:translate(-50%, -50%);
                opacity:0;
                transition: .2s;
            }
            
            
            .checkbox:checked + .fake::before{
                opacity:1;
            }




                .form__btn{
                    color:$colorWhite;
                    background-color:$orange;
                    line-height: 122.56%;
                    letter-spacing: 0.06em;
                    border-radius:50px;
                    border:none;
                    font-size: $orangeButton;
                    text-align: center;
                    padding:14px 65px 22px 65px;
                    box-shadow: 0px 0px 20px $orange;
                    transition: 0.6s;
                    position: relative;
                    left: 50%;
                    transform: translate(-50%, 0);
                    
                    
                
                    
                }

                .form__btn:hover,.form__btn:active, .form__btn:focus{
                    transition: 0.6s;
                    box-shadow:0px 0px 20px $colorWhite;;
                    color:$orange;
                    background-color:$colorWhite;
                    
                }



                        // убрал стрелочки input number

                input[type="number"]::-webkit-outer-spin-button,
               input[type="number"]::-webkit-inner-spin-button {
               -webkit-appearance: none;
                margin: 0;
           }


             input[type="number"] {
  -moz-appearance: textfield;
}
                input[type="number"]:hover,
               input[type="number"]:focus {
               -moz-appearance: number-input;
}


                    input[type=number]::-webkit-inner-spin-button,
                input[type=number]::-webkit-outer-spin-button {
                    -webkit-appearance: none;
                   margin: 0;
}

    }

    

   



</style>