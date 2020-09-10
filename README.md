 <?php require 'conn.php'; ?>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="port.css">
    <!-- <link rel="stylesheet" href="css/ps.css"> -->
    <title>Bipin Portfolio</title>
    <style>
     *{
    margin: 0;padding: 0;box-sizing: border-box;
}
body{

}
header{
 background-image: url("img/iii.jpg");
 width: 100%;
 height: 300px;
}
#head{
    top: 60px;
    /* position: sticky; */
    width: 100%;
    height: 50px;
    background: #000;
    display: flex;
}
#head #logo h4{
    width: 250px;
  padding: 10px;
  color: #fff;
  font-size: 25px;

}
#head #menu ul li{
    position: absolute;
    left: 40%;
    display: flex;
    /* margin-left: 20px; */
}
#head #menu ul li a{
    text-decoration: none;
    margin-left: 20px;
    line-height: 50px;
    font-size: 20px;
    color: #fff;
}
#head #icon img{
    width: 50px;
    height: 50px;
    border-radius: 50%;
    border: 2px solid red;
    padding: 5px;
    margin-left: 10px;
}
#head #icon{
    position: absolute;
    left: 80%;

}
section #main{
margin-top: 100px;
margin-left: 380px;
}
#main li{
    list-style: none;
}
#main li a{
    text-decoration: none;
    font-size: 20px;
    margin-left: 3px;
    background: #000;
  padding: 5px 10px;
  color: #fff;
}


#main li a.active{
    background: red;
}#main li a:hover{
    background: red;
}
 section #box{
    display: none;

}
      
        .imagecontainer{
          
            margin-left:180px;
            width:1000px;
            height:500px;
            z-index:111;
          
            /* overflow:hidden; */
            /* border:2px solid red; */
        }
        
      .imagecontainer div{
          display:inline-block;
          margin-top:20px;
      }  
      .imagecontainer img{
          padding:5px;
        border-radius:20px;
        border:2px solid gray;
          width:300px;
          height:200px;
          margin:5px;


      }
      #container{
          border:2px solid red;
    position: relative;
    width: 1280px;
    height:610px;
    display: block;
    margin-left:40px;
    margin-bottom:60px;
    /* justify-content: space-around; */

}
#container #card{
    position: relative;
    width: 250px;
    /* margin-right:10px; */
    margin-bottom:5px;
    background: linear-gradient(0deg,#1b1b1b,#222,#1b1b1b);
    display: inline-flex;
    justify-content: center;
    align-items: center;
    height: 300px;
    border-radius: 4px;
    text-align: center;
    overflow: hidden;
   transition: 0.5;
}
#container #card:hover{
    transform: translateY(-10px);
    box-shadow: 0 15px 35px rgba(0,0,0,.5); 
}
#container #card:before{
    content: "";
    position: absolute;
    top: 0;
    left: -60px;
    width: 100%;
    height: 100%;
    background: rgba(255,255,255,.03);
    pointer-events: none;
    z-index: 1;
}
#persent{
    position: relative;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    box-shadow: inset 0 0 50px #000;
    background: #222;
    z-index: 1000;
}
#persent #number{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
}
#persent #number h2{
    color: #777;
    font-size: 30px;
    font-weight: 700;
    transition: 0.5s;
}
#card:hover #persent #number h2{
    color: #fff;
    font-size: 40px;
}
#persent #number h2 span{
    font-size: 24px;
    color: #777;
    transition: 0.5s;
}
#card:hover #persent #number h2 span{
    color: #fff;
}
.text{
    position: relative;
    color: #777;
    margin: 20px;
    font-weight: 700;
    font-size: 18px;
    letter-spacing: 1px;
    transition:0.5s ;
}
#card:hover .text{
    color: #ffff;
}
svg{
    position: relative;
    width: 150px;
    height: 150px;
    z-index: 1000;
}
svg circle{
  width: 150px;
  height: 150px;
  fill: none;
  stroke: #191919;
  stroke-width: 10;
  stroke-linecap: round;
  transform: translate(5px,5px);

}
svg circle:nth-child(2){
     stroke-dasharray: 400;
    stroke-dashoffset: 400; 
}
#card:nth-child(1) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 50)/ 100); 
    stroke:#00ff43
}
#card:nth-child(2) svg circle:nth-child(2){
    stroke:yellow;
}
#card:nth-child(3) svg circle:nth-child(2){
    stroke:green;
}
#card:nth-child(4) svg circle:nth-child(2){
    stroke:red;
}
#card:nth-child(5) svg circle:nth-child(2){
    stroke:gold;
}
#card:nth-child(6) svg circle:nth-child(2){
    stroke:blue;
}
#card:nth-child(7) svg circle:nth-child(2){
    stroke:lightcyan;
}

      #card:nth-child(1) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 95)/ 100); 
    stroke:#00ff43
}

#card:nth-child(2) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 90)/ 100); 
    stroke:yellow;
}
#card:nth-child(3) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 80)/ 100); 
    stroke:green;
}
#card:nth-child(4) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 90)/ 100); 
    stroke:red;
}
#card:nth-child(5) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 70)/ 100); 
    stroke:gold;
}
#card:nth-child(6) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 80)/ 100); 
    stroke:blue;
}
#card:nth-child(7) svg circle:nth-child(2){
    stroke-dashoffset: calc(440 - (440 * 90)/ 100); 
    stroke:lightcyan;
}
    </style>
</head>
<body>
    <header>
        <div id="head">
            <div id="logo">
               <h4> Devloper Bipin</h4>
            </div>
            <div id="menu">
                <ul>
                    <li>
                        <a href="">Home</a>
                        <a href="">About</a>
                        <a href="">Portfolio</a>
                        <a href="">Contact</a>
                    </li>
                </ul>
            </div>
            <div id="icon">
                <img src="img/icon/f2.png" alt="" srcset="">
                <img src="img/icon/ty.png" alt="" srcset="">
                <img src="img/icon/ins.png" alt="" srcset="">
            </div>
        </div>
    </header>
<!-- <div>Devloper Bipin kumar</div>
<img src="img/J.png" alt="" width="80%" height="100px"> -->
    <section>
        <div id="main" >
            <ul>
                <li>
                    <a href="#" data-filter="all" class="button active">All</a>
                    <a href="#" data-filter="Educational" class="button">Educational</a>
                    <a href="#" data-filter="Portfolio" class="button">Portfolio</a>
                    <a href="#" data-filter="Web design" class="button">Web design</a>
                    <a href="#" data-filter="E commerse" class="button">E commerse</a>
                    <a href="#" data-filter="Business" class="button">Business</a>
                </li>
            </ul>
        </div>
    
        <div class="imagecontainer">
            <?php
        $selectquery = "SELECT * FROM `image`";
  $query = mysqli_query($con,$selectquery);
 
 
 if( $countdata = mysqli_num_rows($query)>0){
   while ( $fetchdata = mysqli_fetch_assoc($query)) {
       ?>
    
   
 
            <div class="filter <?php echo $fetchdata['filter']; ?>">
            <img src="img/ecom/<?php echo $fetchdata['file']; ?>" alt="" srcset="">
            </div>
<?php 
   }
}
   ?>
</div>

</section>

<div id="container">
    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>95<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">HTML</h2>
    </div>
    </div>

    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>90<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">CSS</h2>
    </div>
    </div>

    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>80<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">JAVASCRIPT</h2>
    </div>
    </div>
  
    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>90<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">JQUERY</h2>
    </div>
    </div>
   
    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>70<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">AJEX</h2>
    </div>
    </div>

    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>80<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">PHP</h2>
    </div>
    </div>
  
    <div id="card">
    <div id="box">
    <div id="persent">
    <svg>
    <circle cx="70"  cy="70" r="70"></circle>
    <circle cx="70"  cy="70" r="70"></circle>
    </svg>
    <div id="number">
    <h2>90<span>%</span></h2>
    </div>
    </div>
    <h2 class="text">BOOTSTROP</h2>
    </div>
    </div>

    </div>
    
   <script src="jquery/jquery-3.5.1.min.js"></script>
  <script>
      $(document).ready(function(){
   $('.button').click(function(){
  var name = $(this).attr("data-filter");
  if(name == "all"){
      $(".filter").show("2000");
  }else{
      $(".filter").not("."+name).hide("2000");
      $(".filter").filter("."+name).show("2000");
  }
   });
      });
  </script>
 
  
</body>
</html>
