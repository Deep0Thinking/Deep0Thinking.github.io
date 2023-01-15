---
layout: page
title: Archive
---

<head>

	<style>
		.Width
		{
			width: 100%;
		}

		.Group-Container-Full-Display
		{
			display: flex;
			justify-content: space-around;
			flex-direction: row;
			flex-wrap: wrap;
		}

		.Group-Container-Scrolling-Display
		{
			display: flex;
			flex-direction: row;
			overflow: auto;
		}

		.Single-Container
		{
			position: relative;
			width: 170px;
			min-width: 170px;
			margin: 11px;
			height: 100%;
			text-align: center;
			cursor: pointer;

			text-align: center;
			display: flex;
	    align-items: center;
		}

		.ImgBorder
		{
			transition: 0.3s;
			display: inline-block;
	    width: 100%;
	    height: 100%;
	    border: 4px solid;
	    border-color: black;
		}


		.Single-Container:hover .ImgBorder
		{
			border-color: DodgerBlue;
			transform: scale(1.1);
			transition: 0.3s;
		}

		.ImgOpacity
		{
			opacity: 1;
			width: 100%;
			transition: 0.3s;
		}

		.Single-Container:hover .ImgOpacity
		{
			opacity: 0.15;
			transition: 0.3s;
		}

		.Text
		{
			color: black;
			font-size: 20px;
			text-decoration: none;
			opacity: 0;
			transition: 0.3s;
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			width: 75%;
		}

		.Single-Container:hover .Text
		{
			opacity: 1;
			color: black;
			text-decoration: none;
		}

		.Text:visited
		{
			text-decoration: none;
			color: black;
		}

		.Selection
		{
			color: black;
			font-size: 20px;
			text-decoration: none;
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			width: 75%;
			height: 100%;
			display: none;
			opacity: 0;
			transition: 0.3s;
			flex-direction: column;
			justify-content: space-around;
			align-items: center;
			flex-wrap: wrap;
		}

		.Single-Container:hover .Selection
		{
			opacity: 1;
			transition: 0.3s;
		}

		.Option
		{
			position: relative;
			border: black solid 3px;
			padding: 3%;
			transition: 0.3s;
			color: black;
			text-decoration: none;
			width: auto;
		}

		.Option:hover
		{
			border-color: DodgerBlue;
			transform: scale(1.1);
			transition: 0.3s;
			color: black;
		}

	</style>

	<link href="https://cdn.jsdelivr.net/npm/remixicon@2.5.0/fonts/remixicon.css" rel="stylesheet">

</head>

### <i class="ri-book-fill"></i> Books written by me (you can scroll this part horizontally):

<!-- The whole display part for Scrolling-Display -->
<div class="Group-Container-Scrolling-Display">

	<div class="Single-Container">

		<div class="ImgBorder"><img class="ImgOpacity" src="https://thumbs.gfycat.com/FlickeringMeatyDuck-size_restricted.gif" alt="Intro To Elementary Number Theory"></div>

		<div class="Text">Intro To Elementary Number Theory</div>

		<div class="Selection">

			<a class="Width" href="https://www.bilibili.com/read/cv15974881?spm_id_from=333.999.0.0" target="_blank"><div class="Option">Chinese version</div></a>

			<a class="Width" href="https://www.bilibili.com/read/cv15974881?spm_id_from=333.999.0.0" target="_blank"><div class="Option">English version</div></a>

		</div>

	</div>

</div>

<hr>


<script>

	<!-- Toggle Display (none <-> block) -->
	var x = document.getElementsByClassName("Text");
	var y = document.getElementsByClassName("Selection");
	var z = document.getElementsByClassName("Single-Container");

	for (var i = 0, len = x.length; i < len; i++)
	{
		(function(index){
			z[i].onclick = function(){

			  if (x[index].style.display === "none")
				{
			    x[index].style.display = "flex";
	        y[index].style.display = "none";
			  }

				else
				{
			    x[index].style.display = "none";
	        y[index].style.display = "flex";
			  }

			}

		})(i);

	}

</script>



<script src="https://giscus.app/client.js"
        data-repo="Deep0Thinking/Deep0thinking.github.io"
        data-repo-id="R_kgDOHLLlWQ"
        data-category="General"
        data-category-id="DIC_kwDOHLLlWc4CShS4"
        data-mapping="pathname"
        data-strict="0"
        data-reactions-enabled="1"
        data-emit-metadata="0"
        data-input-position="top"
        data-theme="light"
        data-lang="en"
        data-loading="lazy"
        crossorigin="anonymous"
        async>
</script>
