<!DOCTYPE html>
<html>
<head>
    <title>자기소개 홈페이지</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <style>
        body {
            margin: 0;
            padding: 0;
        }

        header {
            position: fixed;
            width: 100%;
            top: 0px;
            margin: 0;
            padding: 0;
            text-align: center;
            z-index: 100;
            background-color: white;
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            width: 100%;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin-top: 15px;
            padding: 10px;
            margin-right: 30px;
            font-size: large;
        }

        nav ul li a {
            text-decoration: none;
            color: #333;
        }

        .profile-image {
        display: block;
        margin: 0 auto;
        margin-left: 50px;
        float: left;
        width: 100%;
        max-width: 570px;
        height: auto;
        }

        #about {
            margin-top: 100px;
            display: block;
        }

        #hobby {
            margin-top: 150px;
        }

        #study {
            margin-top: 100px;
        }

        .hobby-images {
        display: flex;
        justify-content: center;
        margin-top: 30px;
        flex-wrap: wrap;
        }

        .hobby-images img {
        width: 200px;
        height: 200px;
        }

        .hobby-images figcaption {
        text-align: center;
        margin-top: 10px;
        }

        .title {
            text-align: center;
        }

        .baekjun {
        display: block;
        margin: 0 auto;
        float: left;
        width: 30%;
        height: 30%;
        }

        @media  (max-width: 499px) {
        .baekjun {
        display: block;
        margin: 0 auto;
        float: left;
        width: 100%;
        height: 100%;
        max-width: 500px;
        }
        }


        @media (min-width: 500px) and (max-width: 799px) {
        .profile-image {
        display: block;
        margin: 0 auto;
        margin-left: 50px;
        float: left;
        width: 200%;
        max-width: 800px;
        height: auto;
        }

        .baekjun {
        display: block;
        margin: 0 auto;
        float: left;
        width: 150%;
        height: 150%;
        max-width: 800px;
        }
        }


    </style>
    
    <script>
        $(document).ready(function() {
            $('nav a').on('click', function(e) {
                e.preventDefault();
                var target = $(this).attr('href');
                $('div').hide();
                $(target).show();
            });
        });
    </script>

    
    
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#about">Introduction</a></li>
                <li><a href="#hobby">Hobby</a></li>
                <li><a href="#study">Study</a></li>
            </ul>
        </nav>
    </header>


    <div id="about">
        <img class="profile-image" src="https://img.hankyung.com/photo/202112/AA.28229717.1.jpg"></a>
        <h1>자기소개</h1>
        <p>안녕하세요. 저는 현재 강원대학교 컴퓨터공학과에 재학중인 2학년 권제후입니다.</p>
        <p>저는 학창시절에 남양주에서 살았으며 도농중학교, 동화고등학교를 졸업하여 강원대학교에 오게되었고, 현재는 안산에 거주 중입니다.</p>
        <p>가족관계로는 형과 동생이 있으며 나이차이가 많이나서 형과는 5살차이, 동생과는 7살로 형과 동생이 띠동갑입니다.</p>
        <p>1학년은 자율전공학부에 있다가 현재 2학년에 컴퓨터공학과에 오게 되었으며, 파이썬을 주력으로 해서 알고리즘을 공부 중입니다.</p>
        <p>모두 반갑습니다!</p>
    </div>


    <div id="hobby" class="hobby-images" style="display: none;">
        <h1>취미</h1>
            <figure>
                <img class="game" src="https://www.leagueoflegends.com/static/open-graph-2e582ae9fae8b0b396ca46ff21fd47a8.jpg">
                <figcaption>게임</figcaption>
            </figure>
            <figure>
                <img class="bike" src="https://pds.joongang.co.kr/news/component/htmlphoto_mmdata/202003/02/625c670a-04f1-4ae3-8468-35ac5fafb79b.jpg">
                <figcaption>자전거타기</figcaption>
            </figure>
            <figure>
                <img class="music" src="https://image.utoimage.com/preview/cp921217/2021/03/202103010565_500.jpg">
                <figcaption>음악듣기</figcaption>
            </figure>
            <figure>
                <img class="WebToon" src="https://cdn.aitimes.kr/news/photo/202212/26708_40154_3921.jpg">
                <figcaption>웹툰감상</figcaption>
            </figure>
    </div>

    <div id="study" style="display: none;">
        <h1 class="title">공부 계획</h1>
        <img class="baekjun" src="https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/images/boj-og.png">
        <br>
        <p>지금까지 배운 언어로는 C, JAVA, PYTHON에 대해 조금씩 배웠습니다.</p>
        <p>요즘은 파이썬으로 주로 백준 사이트에서 알고리즘을 공부하고 있습니다.</p>
        <p>하지만 곧 군대를 가야해서 군대를 다녀온 후 공부를 이어가야 하지 않을까 싶습니다 ㅎㅎ.</p>
        <p>나중에 배워보고 싶은 언어로는 매우 빠른 속도를 자랑하는 c++을 배우고 싶으며 추후에는 백엔드 개발자가 되는 것을 희망하고 있습니다.</p>
    </div>

</body>
</html>
