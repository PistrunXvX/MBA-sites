 
    <div class="form-container">
    <div class="container-fluid">
        <div class="row">

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
                    <div class="row">
                    <div class="col-xl-6">

                    
                    <input type="text" class="form-control form__name" placeholder="Ваше имя" require>
                </div>
                <div class="col-xl-6">
                    <input type="email" class="form-control form__email" placeholder="Ваш телефон" require>
                </div>
                 </div>
                    <input type="email" class="form-control  form_send__email" placeholder="Ваш электронный адрес"
                        require>
                   <label class="label">
                    <input type="checkbox" class="checkbox">
                    <span class="fake"></span>
                    <span class="p">Я согласен с политикой конфиденциальности</span>
                   </label>
                   
                </div>
                <button class="btn form__btn" type="submit">Отправить</button>
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
        padding-top:211px;
        padding-bottom:260px;
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

        .form_send__email{
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

        }

        .form-control::placeholder{
            color:#D3D3D3;
        }

        .form-control::placeholder{
            color:#colorWhite;
        }

        .form-control:focus{
            color:$colorWhite;
        }




            .form-block{

                .p{
                    color:$colorWhite;
                    font-size: $formInputSize;
                }
            }


        
           
            
            .label{}
            
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
                background-image:url('../img/Vector 9.svg');
                background-size: 20px, 20px;
                background-repeat:no-repeat;
                background-position:center;
                
               
                transform:translate(-50%, -50%);
                opacity:0;
                transition: .2s;
            }
            
            
            .checkbox:checked + .fake::before{
                opacity:1;
            }

    }

    

    



</style>