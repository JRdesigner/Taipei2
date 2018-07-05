
<html>
<head>
	<title>Card 3D</title>
	<meta charset="utf-8">
  <link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
  <style>
    @import url('https://fonts.googleapis.com/css?family=Josefin+Sans:400,700');
body {
	margin: 0;
	padding: 0;
	font-family: 'Josefin Sans', sans-serif;
}
.card {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%,-50%);
	width: 300px;
	height: 400px;
	transform-style: preserve-3d;
	perspective: 600px;
	transition: 0.5s;
}
.card .front {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background: #000;
	backface-visibility: hidden;
	transform: rotateX(0deg);
	transition: 0.5s;
}
.card:hover .front {
	transform: rotateX(-180deg);
}
.card .back {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background: #000;
	backface-visibility: hidden;
	transform: rotateX(180deg);
	transition: 0.5s;
}
.card .back:before {
	content: '';
	position: absolute;
	top: 0;
	left: -50%;
	width: 100%;
	height: 100%;
	background: rgba(255,255,255,0.1);
}
.card:hover .back {
	transform: rotateX(0deg);
}
.card .back .details {
	position: absolute;
	top: 50%;
	left: 0;
	transform: translateY(-50%);
	width: 100%;
	text-align: center;
	box-sizing: border-box;
	padding: 20px;
}
.card .back .details h2 {
	margin: 0;
	padding: 0;
	font-size: 20px;
	color: #fff;
}
.card .back .details h2 span {
	font-size: 16px;
	color: #a7a7a7;
}
.social-icons {
	padding: 10px 0;
}
.social-icons a {
	text-align: center;
	width: 36px;
	height: 36px;
	display: inline-block;
	background: #262626;
	color: #fff;
	text-decoration: none;
	border-radius: 50%;
	transition: 0.5s;
}
.social-icons a .fa {
	line-height: 36px;
}
.social-icons a:hover {
	background: #e91e63;
}
  </style>
</head>
<body>
	<div class="card">
		<div class="front"><img src="fan-mu-3.jpg"></div>
		<div class="back">
			<div class="details">
				<h2>Tony Tèo<br> <span>Junior Designer</span></h2>
				<div class="social-icons">
					<a href="#"><i class="fa fa-facebook-official" aria-hidden="true"></i></a>
					<a href="#"><i class="fa fa-twitter" aria-hidden="true"></i></a>
					<a href="#"><i class="fa fa-google-plus-official" aria-hidden="true"></i></a>
					<a href="#"><i class="fa fa-instagram" aria-hidden="true"></i></a>
					<a href="#"><i class="fa fa-camera-retro" aria-hidden="true"></i></a>	
				</div>
			</div>
		</div>

	</div>
</body>
</html>
