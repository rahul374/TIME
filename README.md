<html lang="en">
<head>
    <meta char set="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Create clock</title>
    <style>
        *{margin: 0;padding: 0;}
      
        .container{
            background: none;
        }
        .clock{
            width: 400px;
            height: 400px;
          background-image: url('c2.png');
          background-repeat: no-repeat;
          background-size: cover;
    
            margin-top: 30px;
            margin-left: 300px;
            border-radius: 50%;
            border: 50px solid rgb(238, 101, 101) ;
            position: relative;
            z-index: -3;
        }
        .sec{
            width: 10px;
        height: 150px;
    background-color:yellow;
        margin-top: -400px;
        margin-left: 500px;
        color:black    ;
        z-index: 1;
        position:relative;
        transform-origin: bottom;
        animation-name: sec;
        animation-duration: 60s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
        
        }
         .min{
            width: 10px;
        height: 130px;
       background-color: blue;
        margin-top: -130px;
         margin-left: 500px;
        color: white  ;
        z-index: 2; 
        position: relative;
        transform-origin: bottom;
        animation-name: min;
        animation-duration: 7200s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
        
         
        
        }
        .hour{
            width: 10px;
        height: 115px;
        background-color: lawngreen;
        margin-top: -110px;
        margin-left: 500px;
        color:black ; 
        transform-origin: bottom;
        animation-name: hour;
        animation-duration: 72000s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
          ;
        
        }  
        @keyframes sec{
            from{ transform: rotatez(0deg);}
            to{ transform: rotatez(360deg);}
        }
        @keyframes min{
            from{ transform: rotatez(0deg);}
            to{ transform: rotatez(360deg);}
        }
        @keyframes hour{
            from{ transform: rotatez(0deg);}
            to{ transform: rotatez(360deg);}
    
  }
  </style>
</head>
<body>
   
   
  <h1> TIME SEEN HERE </h1>
    <div class="container">
        <div class="clock"> </div>
        <div class="sec">S</div>
        <div class="min">M</div>
        <div class="hour">H</div>
   
    </div>
    
</body>
</html>
