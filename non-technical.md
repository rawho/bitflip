---
layout: mypage
permalink: /non-technical/
---

<style>
    .event-container{
        margin-top: 200px;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        max-width: 90%;
        margin-left: auto;
        margin-right: auto;
    }
    .event-container .box-event{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
        grid-column: auto;
        width: 100%;
        height: 500px;
        border-radius: 20px;
        justify-content: center;
        position: relative;
        background-color: #000000;
        
    }
    .box-event img{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        opacity: 1;
        
    }
    .event-container .box-event .poster{
        
    }



    

    @media(max-width: 767px){
        .event-container{
            margin-top: 150px;
            display: grid;
            grid-template-columns: 1fr;
            max-width: 90%;
            row-gap: 20px;
        }
        .event-container .box-event{
            width: 100%;
        }

    }
</style>

<div class="event-container">
    <div class="box-event">
        <div class="poster">
            <img src="/static/images/non-tech1.jpg" alt="">        
        </div>
    </div>
    <div class="box-event">
        <div class="poster">
            <img src="/static/images/non-tech2.jpg" alt="">        
        </div>
    </div>
    <div class="box-event">
        <div class="poster">
            <img src="/static/images/non-tech3.png" alt="">        
        </div>
    </div>

</div>
<p id="footer">&copy; Bitflip | Designed and developed by Rahul T</p> 