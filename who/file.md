<h2>你好</h2>
<style>
    .logos {
        width: 980px;
        margin: 0 auto;
        padding: 20px;
        overflow: hidden;
        *zoom: 1;
    }

    .logos li{
        float: left;
        width: 140px;
        height: 140px;
        line-height: 140px;
        overflow: hidden;
        margin: 24px;
        text-align:center;
        background: #fff;
        border-radius: 10px;
    }

    .logos li:after,.logos li span{
        display:inline-block;
        *display:inline;
        *zoom:1;
        width:0;
        height:100%;
        vertical-align:middle;
    }
    .logos li:after{
        content:'';
    }

    .logos li img{
        display:inline-block;
        *display:inline;
        *zoom:1;
        vertical-align:middle;
        font-size:16px;
        width: 120px;
    }
    .logos li a{
        display: inline-block;
        width: 100%;
        height: 100%;
    }
    .container {
        padding-right: 15px;
        padding-left: 15px;
        margin-right: auto;
        margin-left: auto;
    }
    .jumbotron{
        border-radius: 6px;

        position: relative;
        padding: 30px 0;
        color: rgba(255, 255, 255, 0.6);
        text-shadow: 0 1px 0 rgba(0, 0, 0, 0.1);
        background-color: #1ba9ba;
        background-image: -webkit-gradient(linear, left top, left bottom, from(#0088a4), to(#1ba9ba));
        background-image: -webkit-linear-gradient(top, #0088a4 0, #1ba9ba 100%);
        background-image: -o-linear-gradient(top, #0088a4 0, #1ba9ba 100%);
        background-image: linear-gradient(to bottom, #0088a4 0, #1ba9ba 100%);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#0088a4', endColorstr='#1ba9ba', GradientType=0);
        background-repeat: repeat-x;

    }
    .jumbotron:after{
        position: static;
    }
    .projects-header {

        text-align: center;
        margin: 60px 0 10px;
        font-weight: 200;
        margin-bottom: 40px;
        display: block;
        margin-left: auto;
        margin-right: auto;
    }
    .projects-header h2{
        color:#1ba9ba;
    }
    .projects-header p{
        color:#ccc;
    }
    .page-header {
        padding-bottom: 9px;
        margin: 40px 0 20px;
        border-bottom: 1px solid #eee;
    }
</style>
<div class="row jumbotron">
    <ul class="logos" ms-controller="logos">

        <li ms-for="el in @logos">
            <a ms-attr="{href: el.link}" target="_blank" >
                <img ms-attr="{src: 'http://avalonjs.coding.me/share/img/logos/'+el.src}"/>
                <!--[if lt IE 8]><span></span><![endif]-->
            </a>
        </li>

    </ul>
</div>