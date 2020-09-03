---
layout: mypage
permalink: /non-technical/valorant/
---
<style>

body{
    color: #ffffff;
}

.container-ideathon{
    margin-top: 200px;
    margin-left: auto;
    margin-right: auto;
    display: grid;
    grid-template-columns: 1fr 1fr;
    max-width: 80%;
    column-gap: 20px;
    margin-bottom: 100px;
}

.boxes img{
    max-width: 80%;
    justify-self: center;
}
.boxes p{
    font-size: 25px;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-weight: 100;
}
.boxes h4{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    color: #ecdddd;
    font-size: 30px;
    margin-bottom: 20px;
    padding-top: 30px;
    font-weight: 400;
}
.boxes h5{
    color: #ffffff;
    font-size: 20px;
    font-weight: 300;
    padding-top: 30px;
}
#prize{
    font-family: Arial, Helvetica, sans-serif;
    background-color: #ff8900;
    padding:5px 15px;
    color: #ffffff;
}
.date-sub{
    color: #ff8900;
    font-family: monospace;
    letter-spacing: .0001rem;
}
.boxes:nth-child(3){
    margin-top: 80px;
    margin-bottom: 200px;
    
    justify-self: center;
}

.ab{
    color: #ff8900;
    font-size: 25px;
    font-weight: 200;
}
.c{
    font-size: 35px;
}
@media(max-width: 767px){
    .container-ideathon{
        grid-template-columns: 1fr;

    }
    .boxes img{
        max-width: 100%;
    }

    .boxes h4{
        font-size: 22px;
        font-weight: 200;
        color: #ffffff;
    }
    .container-ideathon .boxes:nth-child(1){
        display: block;
    }
    .c{
        font-size: 30px;
    }
}

.btn-01{
    margin-right: 50px;
}
</style>


<div class="container-ideathon">
    <div class="boxes">
        <img src="/static/images/bitflip_nontech_val_final1 (1).jpg" alt="poster">
    </div>
    <div class="boxes">
        <h4><span class="ab c">VALORANT TOURNEY</span></h4>
        <p>Enroll as teams of 5 and embark on this lethal combat where precise gunplay meets unique agent abilities!</p>
        <h4><span id="prize">PRIZE POOL: INR 2000/-</span></h4>
        <h4>Reg fee : <span class="ab">₹200 </span> <br><br>
            Open to all <br><br>
            </h4><br>
            <a href="https://rzp.io/l/bitflipgaming"><button class="btn-01">Register Now</button></a>
            <a href="/static/BITFLIP_VALORANT TOURNEY_ RULES AND REGULATIONS.pdf"><button class="btn-01">Rules & Regulations</button></a>
    </div>
</div>

