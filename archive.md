---
layout: page
title: Archive
---

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