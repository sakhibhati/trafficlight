# trafficlight
html and css code

><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    *{padding: 0; margin: 0;}
    .trafic{
        height: 200px;
        width: 80px;
        background-color: black;
        border-radius: 10px;
        margin: auto;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        padding: 10px 5px;


    }
    .trafic span{width: 50px; height: 50px; background-color: grey; border-radius: 100%; animation-duration: 8s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;}
    .red {
        animation-name: red;
      }
      .yellow {
        animation-name: yellow;
      }
      .green {
        animation-name: green;
      }
      
      @keyframes red {
        0%,
        33% { background-color: red;}
        34%,
        100% { background-color: gray;}
      }

      @keyframes yellow {
        0%,
        33% {background-color: gray;}
        34%,
        66% {background-color: yellow;}
        67%,
        100% {background-color: gray;}
      }

      @keyframes green {
        0%,
        66% {background-color: gray;}
        67%,
        100% {background-color: green;}
      }
      .pole{height: 150px; width: 20px; background-color: black;
    margin: auto;}
    
</style>
<body>
    <div class="trafic">
        <span class="red"></span>
        <span class="yellow"></span>
        <span class="green"></span>
    </div>
    <div class="pole"></div>
</body>
</html>
