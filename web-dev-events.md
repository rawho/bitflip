---
layout: mypage
permalink: /web-dev-events/
---

<style>
    .event-container{
        margin-top: 200px;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        max-width: 75%;
        column-gap: 50px;
        row-gap: 100px;
        margin-left: auto;
        margin-right: auto;
    }
    .event-container .box-event{
        grid-column: auto;
        width: 100%;
        height: 400px;
        border-radius: 20px;
        justify-content: center;
        position: relative;
    }
    .box-event h1{
        position: absolute;
        top: 50px;
        left: 20px;
        color: #ffffff;
        font-size: 30px;
    }
    .box-event p{
        position: absolute;
        bottom: 80px;
        left: 20px;
        color: #ffffff;
        font-weight: 600;
        font-size: 20px;
        font-family: Arial, Helvetica, sans-serif;
        padding-right: 20px;
    }
    .box-event i{
        position: absolute;
        bottom: 20px;
        right: 100px;
        color: #ffffff;
        font-size: 40px;
        animation: right 2s ease infinite;
    }

    @keyframes right{
        0%,20%,50%,80%,100%{
            transform: translateX(0);
        }
        40%{
            transform: translateX(-30px);
        }
        60%{
            transform: translateX(-15px);
        }
    }
    .box-event a{
        position: absolute;
        right: 30px;
        bottom: 20px;
        font-size: 20px;
        color: #ffffff;
        text-decoration: none;
        font-weight: 600;
    }
    .box-event:nth-child(odd){
        background-color: #6200ee;
    }
    .box-event:nth-child(even){
        background-color: #49aaa0;
    }

    @media(max-width: 767px){
        .event-container{
            margin-top: 150px;
            display: grid;
            grid-template-columns: 1fr;
            max-width: 80%;
            row-gap: 20px;
        }
        .box-event h1{
            font-size: 28px;
        }
        .box-event p{
            font-size: 20px;
        }
    }
</style>

<div class="event-container">
    <div class="box-event">
        <h1>HTML/CSS</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum fugit assumenda ipsum temporibus reprehenderit corrupti?</p>>
        <i class="fa fa-angle-right"></i><a href="/events/gaming-using-python">View</a>
    </div>
    <div class="box-event">
        <h1>Javascript</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum fugit assumenda ipsum temporibus reprehenderit corrupti?</p>>
        <i class="fa fa-angle-right"></i><a href="/events/gaming-using-python">View</a>
    </div>
    <div class="box-event">
        <h1>React</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum fugit assumenda ipsum temporibus reprehenderit corrupti?</p>
        <i class="fa fa-angle-right"></i><a href="/events/gaming-using-python">View</a>
    </div>
    <div class="box-event">
        <h1>Node</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum fugit assumenda ipsum temporibus reprehenderit corrupti?</p>
        <i class="fa fa-angle-right"></i><a href="/events/gaming-using-python">View</a>
    </div>
</div>
<p id="footer">&copy; Bitflip | Designed and developed by Rahul T</p> 