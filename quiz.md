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
#canvas {
        width: 100%;
        min-height: 500vh;
        background: #121212;
        background-image: url('/static/images/quiz.jpg');
        background-size: contain;
        position:absolute;
        left:0;
        top:0;
        position: fixed;
        z-index:-1;
        opacity: .2;
    }
@media(max-width: 767px){
    #canvas {
        width: 100%;
        min-height: 500vh;
        background: #121212;
        background-image: url('/static/images/game-back.jpg');
        background-size: contain;
        position:absolute;
        left:0;
        top:0;
        position: fixed;
        z-index:-1;
        opacity: .4;
    }
}
</style>

<canvas id="canvas"></canvas>
<div class="container-ideathon">
    <div class="boxes">
        <img src="/static/images/quiz.jpeg" alt="poster">
    </div>
    <div class="boxes">
        <h4><span class="ab c">MELA QUIZ</span></h4>
        <p>Rack your brains out as only the best can excel as you explore the fields of <span class="ab">'Music Entertainment Literature and Arts'</span>  in this quiz!</p>
        <h4>Quiz Master : <span class="ab">Mahendra Balu P</span></h4>
        <h4><span id="prize">Prizes worth INR 1500</span></h4>
        <h4>Reg fee : <span class="ab">₹30/head </span> <br><br>
            Open to all <br><br>
            Teams of 4 or less</h4><br>
            <button class="btn-01" style="background-color: red">Registration Closed</button>
            <br>
            <br>
            <a href="/static/BITFLIP_MELA_FAQ (1).pdf"><button class="btn-01">Rules & Regulations</button></a>
    </div>
</div>
<p id="footer">&copy; Bitflip | Designed and developed by <a href="https://github.com/rawho">Rahul T</a> </p>
<script>
    var Canvas = document.getElementById('canvas');
var ctx = Canvas.getContext('2d');

var resize = function() {
    Canvas.width = Canvas.clientWidth;
    Canvas.height = Canvas.clientHeight;
};
window.addEventListener('resize', resize);
resize();

var elements = [];
var presets = {};

presets.o = function (x, y, s, dx, dy) {
    return {
        x: x,
        y: y,
        r: 12 * s,
        w: 5 * s,
        dx: dx,
        dy: dy,
        draw: function(ctx, t) {
            this.x += this.dx;
            this.y += this.dy;
            
            ctx.beginPath();
            ctx.arc(this.x + + Math.sin((50 + x + (t / 10)) / 100) * 3, this.y + + Math.sin((45 + x + (t / 10)) / 100) * 4, this.r, 0, 2 * Math.PI, false);
            ctx.lineWidth = this.w;
            ctx.strokeStyle = '#fff';
            ctx.stroke();
        }
    }
};

presets.x = function (x, y, s, dx, dy, dr, r) {
    r = r || 0;
    return {
        x: x,
        y: y,
        s: 20 * s,
        w: 5 * s,
        r: r,
        dx: dx,
        dy: dy,
        dr: dr,
        draw: function(ctx, t) {
            this.x += this.dx;
            this.y += this.dy;
            this.r += this.dr;
            
            var _this = this;
            var line = function(x, y, tx, ty, c, o) {
                o = o || 0;
                ctx.beginPath();
                ctx.moveTo(-o + ((_this.s / 2) * x), o + ((_this.s / 2) * y));
                ctx.lineTo(-o + ((_this.s / 2) * tx), o + ((_this.s / 2) * ty));
                ctx.lineWidth = _this.w;
                ctx.strokeStyle = c;
                ctx.stroke();
            };
            
            ctx.save();
            
            ctx.translate(this.x + Math.sin((x + (t / 10)) / 100) * 5, this.y + Math.sin((10 + x + (t / 10)) / 100) * 2);
            ctx.rotate(this.r * Math.PI / 180);
            
            line(-1, -1, 1, 1, '#fff');
            line(1, -1, -1, 1, '#fff');
            
            ctx.restore();
        }
    }
};

for(var x = 0; x < Canvas.width; x++) {
    for(var y = 0; y < Canvas.height; y++) {
        if(Math.round(Math.random() * 8000) == 1) {
            var s = ((Math.random() * 5) + 1) / 10;
            if(Math.round(Math.random()) == 1)
                elements.push(presets.o(x, y, s, 0, 0));
            else
                elements.push(presets.x(x, y, s, 0, 0, ((Math.random() * 3) - 1) / 10, (Math.random() * 360)));
        }
    }
}

setInterval(function() {
    ctx.clearRect(0, 0, Canvas.width, Canvas.height);

    var time = new Date().getTime();
    for (var e in elements)
		elements[e].draw(ctx, time);
}, 10);
</script>