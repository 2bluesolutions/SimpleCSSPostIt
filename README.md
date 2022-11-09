# Simple CSS Post-It Note
A simple post-it note in CSS

![post-it](https://user-images.githubusercontent.com/21087449/200914625-44dbdfa9-23dd-4735-ae29-667f3967d555.jpg)


Create a simple block of text for what you want to appear:

```
<div class="postit">
	<p>sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </p> 
	<p>MORE TEXT!!!</p>
	<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit  </p>
	<p style="font-size:30px;">Brian</p>

</div>
```

Relatively simple style for the post-it.  You can change the colours as you see fit as well as the widths and heights.  Use absolute positioning to place the post-it on top of other HTML elements.   Add a bit of rotation with transform:rotate to adjust the look and feel.
```

	<style>
		@import 'https://fonts.googleapis.com/css?family=Reenie+Beanie';
		.postit {
			line-height: 1;
			text-align: center;
			width: 250px;
			margin: 25px;
			min-height: 300px;
			max-height: 150px;
			position: relative;
			border: 1px solid #E8E8E8;
			padding: 0 30px 20px;
			border-top: 0 solid #fdfd86!important;
			font-family: 'Reenie Beanie'!important;
			font-size: 22px;
			border-bottom-right-radius: 60px 5px;
			display: inline-block;
			background: #ffff88;
			background: -moz-linear-gradient(-45deg, #ffff88 81%, #ffff88 82%, #ffff88 82%, #ffffc6 100%);
			background: -webkit-gradient(linear, left top, right bottom, color-stop(81%,#ffff88), color-stop(82%,#ffff88), color-stop(82%,#ffff88), color-stop(100%,#ffffc6));
			background: -webkit-linear-gradient(-45deg, #ffff88 81%,#ffff88 82%,#ffff88 82%,#ffffc6 100%);
			background: -o-linear-gradient(-45deg, #ffff88 81%,#ffff88 82%,#ffff88 82%,#ffffc6 100%);
			background: -ms-linear-gradient(-45deg, #ffff88 81%,#ffff88 82%,#ffff88 82%,#ffffc6 100%);
			background: linear-gradient(135deg, #ffff88 81%,#ffff88 82%,#ffff88 82%,#ffffc6 100%);
			filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ffff88', endColorstr='#ffffc6',GradientType=1 );
		}

		.postit:after {
			content: "";
			position: absolute;
			z-index: -1;
			right: 0px;
			bottom: 20px;
			width: 200px;
			height: 25px;
			background: rgba(0, 0, 0, 0.2);
			box-shadow: 2px 15px 5px rgb(0 0 0 / 40%);
			-moz-transform: matrix(-1, -0.1, 0, 1, 0, 0);
			-webkit-transform: matrix(-1, -0.1, 0, 1, 0, 0);
			-o-transform: matrix(-1, -0.1, 0, 1, 0, 0);
			-ms-transform: matrix(-1, -0.1, 0, 1, 0, 0);
			transform: matrix(-1, -0.1, 0, 1, 0, 0);
		}

	</style>
