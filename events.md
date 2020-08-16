---
layout: mypage
permalink: /events/
---

<style>
    .event-container{
        margin-top: 200px;
        display: grid;
        grid-template-columns: 1fr 1fr;
        max-width: 65%;
        column-gap: 50px;
        row-gap: 100px;
        margin-left: auto;
        margin-right: auto;
    }
    .event-container .box-event{
        grid-column: auto;
        width: 80%;
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
    .box-event:nth-child(1),
    .box-event:nth-child(4){
        background-color: #6200ee;
    }
    .box-event:nth-child(2),
    .box-event:nth-child(3){
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
        .event-container .box-event{
            width: 100%;
        }
        .box-event h1{
            font-size: 28px;
        }
        .box-event p{
            font-size: 20px;
        }
        .box-event:nth-child(odd){
            background-color: #6200ee;
        }
        .box-event:nth-child(even){
            background-color: #49aaa0;
        }
    }
</style>

<div class="event-container">
    <div class="box-event">
        <h1>Common</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum fugit assumenda ipsum temporibus reprehenderit corrupti?</p>
        <i class="fa fa-angle-right"></i><a href="/common-events/">View</a>
    </div>
    <div class="box-event">
        <h1>Machine Learning</h1>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint laboriosam amet est id facilis veritatis.</p>>
        <i class="fa fa-angle-right"></i><a href="/machine-learning-events/">View</a>
    </div>
    <div class="box-event">
        <h1>Web Development</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsum architecto corporis eum. Aspernatur rem ipsum, voluptatibus eius </p>
        <i class="fa fa-angle-right"></i><a href="/web-dev-events/">View</a>
    </div>
    <div class="box-event">
        <h1>Quantum Computing</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ullam consequuntur eaque tempora quae aut eos enim iusto est dolores .</p>>
        <i class="fa fa-angle-right"></i><a href="/quantum-computing-events/">View</a>
    </div>
</div>


<!-- |Date  	  |Event  	              |Time     |
|-	      |-	                  |-	    |
|26/8/2020|[Python Basics     ][a]|IEEE     |
|29/8/2020|[Games using python][b]|IEEE     |
|4/9/2020 |[Documentation     ][c]|IEEE     |
|5/9/2020 |[GIT               ][d]|IET      |
|6/9/2020 |[HTML/CSS          ][e]|ISTE     |
|7/9/2020 |[Open CV           ][f]|IET      |
|9/9/2020 |[ML 1              ][g]|ROBOCET  |
|10/9/2020|[JS                ][h]|         |
|11/9/2020|[ML 2              ][i]|ROBOCET  |
|13/9/2020|[React             ][j]|FOSS CELL|
|14/9/2020|[ML3               ][k]|ROBOCET  |
|16/9/2020|[Node              ][l]|FOSS CELL|
|17/9/2020|[Quantum Computing1][m]|COMMON   |
|18/9/2020|[Quantum Computing2][n]|COMMON   |
|20/9/2020|[Quantum Computing3][o]|COMMON   |
|22/9/2020|[Quantum Computing4][p]|COMMON   |

[a]: /events/python-basics
[b]: /events/gaming-using-python
[c]: /events/gaming-using-python
[d]: /events/gaming-using-python
[e]: /events/gaming-using-python
[f]: /events/gaming-using-python
[g]: /events/gaming-using-python
[h]: /events/gaming-using-python
[i]: /events/gaming-using-python
[j]: /events/gaming-using-python
[k]: /events/gaming-using-python
[l]: /events/gaming-using-python
[m]: /events/gaming-using-python
[n]: /events/gaming-using-python
[o]: /events/gaming-using-python
[p]: /events/gaming-using-python -->