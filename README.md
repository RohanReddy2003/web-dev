<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elastic</title>
    <link rel="stylesheet" href="elastic.css">
</head>
<body>
    <div class="frame">
        <div class="top"></div>
        <div class="bottom"></div>
        <div class="ellipse">
            <div class="black"></div>
            <div class="blue"></div>
        </div>
    </div>
</body>
</html>


.frame{
    position: absolute;
    top: 50%;
    left: 50%;
    width: 400px;
    height: 400px;
    margin-top: -200px;
    margin-left: -200px;
    border-radius: 5px;
    box-shadow: 1px 2px 10px 0px ;
    -webkit-front-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    overflow: hidden;
}
.top{
    position: absolute;
    width: 100%;
    height: 200px;
    top: 0;
    left: 0;
    background: black;
}
.bottom{
    position: absolute;
    width: 100%;
    height: 200px;
    top: 50%;
    left: 0;
    background: rgb(0, 0, 222);
}
.ellipse {
	position: absolute;
	z-index: 2;
	width: 420px;
	height: 400px;
	top: 0;
	left: -10px;
	transform-style: preserve-3d;
	animation: elastic 5s ease-in-out infinite;
}
.black{
    position: absolute;
    width: 420px;
    height: 400px;
    background: black;
    backface-visibility: hidden;
    border-radius: 50%;
    z-index: 2;
    transform: rotateX(0);
}
.blue{
    position: absolute;
    width: 420px;
    height: 400px;
    background: rgb(0, 0, 222);
    backface-visibility: hidden;
    border-radius: 50%;
    z-index: 1;
    transform: rotateX(180deg);
}
@keyframes elastic{
	0% {
		transform: rotateX(90deg);
	}
	15% {
		transform: rotateX(150deg);
	}
	20% {
		transform: rotateX(50deg);
	}
	25% {
		transform: rotateX(120deg);
	}
	30% {
		transform: rotateX(70deg);
	}
	35% {
		transform: rotateX(100deg);
	}
	40% {
		transform: rotateX(83deg);
	} 
	45% {
		transform: rotateX(93deg);
	}
	50% {
		transform: rotateX(90deg);
	}
	
	65% {
		transform: rotateX(30deg);
	}
	70% {
		transform: rotateX(130deg);
	}
	75% {
		transform: rotateX(60deg);
	}
	80% {
		transform: rotateX(110deg);
	}
	85% {
		transform: rotateX(80deg);
	}
	90% {
		transform: rotateX(97deg);
	} 
	95% {
		transform: rotateX(87deg);
	}
	100% {
		transform: rotateX(90deg);
	}
}
