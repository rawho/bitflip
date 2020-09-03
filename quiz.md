---
layout: mypage
permalink: /non-technical/mela-Quiz/
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
}

</style>


<div class="container-ideathon">
    <div class="boxes">
        <img src="/static/images/quiz.jpeg" alt="poster">
    </div>
    <div class="boxes">
        <h4>Quiz Topic : <br> <span class="ab">Music Entertainment Literature Arts</span></h4>
        <h4>Quiz Master : <span class="ab">Mahendra Balu P</span></h4>
        <h4><span id="prize">Prizes worth INR 1500</span></h4>
        <h4>Reg fee : <span class="ab">₹30/head </span> <br><br>
            Open to all <br><br>
            Teams of 4 or less</h4><br>
            <form><script src="https://cdn.razorpay.com/static/widget/payment-button.js" data-payment_button_id="pl_FUfWXmCZeInEni"> </script> </form>
    </div>
</div>

