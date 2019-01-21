---
layout: default
title: about
---
<style>
  @media screen and (max-width: 600px){

  }
  #container {
  	opacity: 1;
  width: 100%;
  }
   #visible-container {
    opacity: 1;
    transition: 1s;
  }
  body {
    /*background-color: #cbefdf;*/
    background-color: white;
    color: white;
    margin: auto;
  }

  .bottom {
  margin-top: 10vw;
  padding-left: 8vw;
  padding-bottom: 4vw;
background-color: white;
color: #696e77;
line-height: 2vw;
width: 40vw;

  }
  .bottombutton{

    padding: 15px 40px;
    font-size: 1vw;
    line-height: 1.8;
    color: white;
    background-color: #2ccc84;
    text-decoration: none;

    border-radius: 30px;
    border: 2px solid #2ccc84;
    padding: 10px;
  }

  .bottombutton:hover {
transition-duration:500ms;
        transition-timing-function: ease-out;
    color: #648aad;
    background-color: #d0dbed;
    border: 2px solid #d0dbed;
  }
  .article-submission {
font-size: 3vw;
margin-bottom: 2vw;

    }

  hr {
    display: block;
      height: 1px;
      border: 0;
      border-top: 2px solid #44a1ff;
      width: 21vw;

  }
  p {
  margin:0px 0px 0px 0px;
  font-size: 1.2vw;
  }
  .middlebutton{
    background-color: none;
    border-radius: 30px;
    border: 2px solid #2ccc84;
    padding: 10px;
    text-decoration: none;
    color: white;
    font-size: 1vw;
  }

  .middlebutton:hover {
    color: white;
    transition-duration:500ms;
        transition-timing-function: ease-out;
    border: 2px solid #4c525b;
    background-color: #4c525b;
  }
  .top {
  	padding-top: 8vw;
    padding-bottom: 0vw;
    padding-left: 8vw;
    color: white;
    background-color: #2ccc84;
    height: 20vw;
    margin:0;
  }
  .topa{
  font-size: 8vw;
  width: 80%;
  margin:0;
  }

  .topb{
font-size: 2.2vw;
  width: 60%;
  margin:0;

  }

.middle {
  padding-top: 4vw;
  background-color: #5b626d;
  color: white;
  height: 30vw;
}
  .b {
    margin-left: 8vw;
    display: inline-block;
    width: 40vw;
    height: 25vw;
    vertical-align: top;
}
.b1 {
  margin-top: 4vw;
font-size: 3vw;
margin-bottom: 2vw;
}
  </style>
  
 <div id= "container" >
  <div class = "top">
  	<div class = "topa">
    	<b>Verdant Articles</b>
    </div>
    <div class = "topb">
    	<i>Written | Created | Managed<br> by high school students</i>
    </div>
  </div>

  <div class = "middle">
  <div class = "b"> <div class = "b1">Our Mission</div>
<!--<hr width = "250px" style = "margin-left: 0;">-->
  <p>  is to give high schoolers a platform for their voices to be heard, help them gain recognition for their writing,
     and promote writing at a young age. 100% of The Verdant Leaf's articles are written by students in high school.</p>
<br>
  <a href = "index.php" class = "middlebutton"> Go Home</a>
</div>
</div>

<div class = "bottom">
<div class = "article-submission">
  Article Submission
  </div>

   <p>
    We welcome all writings. From poetry to theatrical scripts to breaking news to fictional stories to essays, just send it to us!
      After we evaluate your writing, it will be posted online within 2 days.</p>

 <br>
 <a href = "mailto:theverdantleaf@gmail.com?Subject=article-submission" class = "bottombutton"> Submit</a>

</div>
</div>
<script>
function fadein() {
	console.log("called");
  document.getElementById("container").setAttribute("id", 'visible-container');
}

	window.smoothScroll = function(target) {
	target = document.getElementById(target);
    var scrollContainer = target;
    if(scrollContainer == null) return;
    do { //find scroll container
        scrollContainer = scrollContainer.parentNode;
        if (!scrollContainer) return;
        scrollContainer.scrollTop += 1;
    } while (scrollContainer.scrollTop == 0);

    var targetY = 0;
    do { //find the top of target relatively to the container
        if (target == scrollContainer) break;
        targetY += target.offsetTop;
    } while (target = target.offsetParent);

    scroll = function(c, a, b, i) {
        i++; if (i > 50) return;
        c.scrollTop = a + (b - a) / 50 * i;
        setTimeout(function(){ scroll(c, a, b, i); }, 20);
    }
    // start scrolling
    scroll(scrollContainer, scrollContainer.scrollTop, targetY, 0);
    }
  
</script>
