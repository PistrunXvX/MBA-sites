<div class="container-fluid coop__main">
    <h2>Мы сотрудничаем</h2>
    <div class="row justify-content-center">
        <div class="col">
            <div class="cooperative__container">
                <ul>
                    <li><img src="/img/cooperative_img_1.png" alt=""></li>
                    <li><img src="/img/cooperative_img_2.png" alt=""></li>
                    <li><img src="/img/cooperative_img_3.png" alt=""></li>
                    <li><img src="/img/cooperative_img_4.png" alt=""></li>
                </ul>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col">
            <div class="cooperative__container">
                <ul>
                    <li><img src="/img/cooperative_img_5.png" alt=""></li>
                    <li><img src="/img/cooperative_img_6.png" alt=""></li>
                    <li><img src="/img/cooperative_img_7.png" alt=""></li>
                    <li><img src="/img/cooperative_img_8.png" alt=""></li>
                </ul>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col">
            <div class="cooperative__container">
                <ul>
                    <li><img src="/img/cooperative_img_9.png" alt=""></li>
                    <li><img src="/img/cooperative_img_10.png" alt=""></li>
                    <li><img src="/img/cooperative_img_11.png" alt=""></li>
                    <li><img src="/img/cooperative_img_12.png" alt=""></li>
                </ul>
            </div>
        </div>
    </div>
</div>

<style lang="scss" >
    @import 'style/theme.scss';

    .coop__main{
        
        h2{
            font-size: $blockTitleSize;
            font-family: $fbck;
            color: $darkBlue;

            text-transform: uppercase;
            text-align: center;

            margin-top: 5%;
            margin-bottom: 5%;
        }
    }

    .cooperative__container{

        li{
            display: inline;
            list-style: none;

            margin-right: 10%;
        }

        img{
            width: 150px;
        }
    }

</style>