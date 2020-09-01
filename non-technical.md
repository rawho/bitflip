---
layout: construction
driveId: 1yvh0vhIFDP2QkG_zurGqd8j3JH7ctC5z/preview
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
        grid-column: auto;
        width: 100%;
        height: 500px;
        border-radius: 20px;
        justify-content: center;
        position: relative;
        background-color: #000000;
        
    }
    .event-container .box-event .poster img{    
        position: absolute;
        top: 0;
        height: 500px;
    }
    .event-container .box-event .poster button{    
        position: absolute;
        top: 40%;
        left: 20px;
        opacity: 0;
    }
    .event-container .box-event:hover .poster button{
        opacity: 1;
    }
    .event-container .box-event:hover .poster img{
        opacity: .5;
    }
    .box-event img{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        opacity: 1;
        
    }

    video{
        margin-top: 200px;
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
        #mob-btn{
            opacity: .5;

        }

    }
</style>
<!-- {% include googleDrivePlayer.html id=page.driveId %} -->
<div class="event-container">
    <div class="box-event">
        <div class="poster">
            <img src="/static/images/non-tech1.jpg" alt="">        
            <button id="mob-btn" class="btn-01">Coming soon ..</button>
        </div>
    </div>
    <div class="box-event">
        <div class="poster">
            <img src="/static/images/non-tech2.jpg" alt="">       
            <button id="mob-btn" class="btn-01">Coming soon ..</button> 
        </div>
    </div>
    <div class="box-event">
        <div class="poster">
            <img src="/static/images/non-tech3.png" alt="">        
            <button id="mob-btn" class="btn-01">Coming soon ..</button>
        </div>
    </div>

</div>
<p id="footer">&copy; Bitflip | Designed and developed by <a href="https://github.com/rawho">Rahul T</a> </p> 