---
layout: post
title: How to create 5 Cool Css only line effect
author: Spruce
author_link: spruce.emma
summary: 'Who said css lines has to be boring? Or just a straight line'
tags: css effects lines
image: img/posts/lines.jpg
sharing:
  twitter: How to create 5 Cool Css only line effect
  facebook: How to create 5 Cool Css only line effect
---

<p class="lead">
When we talk about css lines we shouldn't always think about ordinary "one way straight lines"
</p>

<p>
Lines can be used to style up our web pages in a lot of ways. That is, just <b>5 effects</b> are just a few things you could do with Lines
</p>

<p>
What would make this effects fun is that you only get to use <b>CSS</b>, no images are used here
</p>

<p class="mark-text">
Note: Some of this effect can be achieved using images too
</p>

<h1>
Css only Line effects
</h1>
<ol>
<li>
 <a href="#highlight-text">
Highlight Text
</a>
</li>
<li>
 <a href="#line-both-side">
Lines on both side of an Element
</a>
</li>
<li>
 <a href="#wavy-line">
Css Wavy line
</a>
</li>
<li>
 <a href="#line-hover">
Line Hover Effect
</a>
</li>
<li>
 <a href="#line-one-side">
Add line in the middle of a word
</a>
</li>
</ol>
<p></p>
<p>
Let's jump right into actually creating this stuff
</p>

<h3 id="highlight-text">
Highlight Text
</h3>
<p>
Now you might be surprised how easy it is to highlight a whole paragraph of text with one line of css...
</p>
<pre class="language-html">
<code class="language-html">
 // HTML code
 &lt;p class="highlight-text"&gt;
  Lorem ipsum dolor sit amet consectetur adipisicing elit. At nam dignissimos nemo nihil iure illo nisi nobis voluptatum sit architecto reprehenderit, quibusdam molestiae, sunt, distinctio ea vero? Error, minus excepturi?
 &lt;p&gt;

// Css 
// Only trick here is to make sure the element is <b>inline</b>

 .highlight-text {
 display: inline; // enforce inline
background: linear-gradient(180deg, rgba(225,225,225,0) 50%, #00bb00 50%);
}
</code>
</pre>
<p></p>
<p>
And that's it, preview should look like this
</p>
<p class="mark-text" style="border: 2px solid #ccx; font-size: 18px">
 Lorem ipsum dolor sit amet consectetur adipisicing elit. At nam dignissimos nemo nihil iure illo nisi nobis voluptatum sit architecto reprehenderit, quibusdam molestiae, sunt, distinctio ea vero? Error, minus excepturi? 
</p>

<h3 id="line-both-side">
Lines on both side of an Element
</h3>
<p>
You might be wondering, how do I place lines on both side of an Element in the most less messy way. It's actually kind of a breeze with css <b>LINEAR-GRADIENT</b>
</p>

<pre class="language-html">
<code class="language-html">
 // HTML code
  &lt;div class="lines"&gt;
    &lt;input type="submit" class="btn btn--small btn--primary" value="button"&gt;
    &lt;/div&gt;

// Css 

 .lines {
    text-align: center;
    background-image: linear-gradient(#ddd,#ddd);
    background-size: 100% .1em;
    background-repeat: no-repeat;
    background-position: center center;
    margin: 2em 0;
}
.llines .btn
 {
 display:inline-block;
 box-shadow:0 0 0 1em #fff;
} 
</code>
</pre>
<p></p>
<p> that's it, the preview should look like this
</p>
<div style="border: 2px solid #ccx; font-size: 18px">
 <div class="lines">
        <input type="submit" class="btn btn--small btn--primary" value="button">
    </div> 
</div>
<p></p>

<h3 id="wavy-line">
Css Wavy lines
</h3>
<p>
With just a single <b>div</b> you can create a Wavy effect with pure css
</p>

 <pre class="language-html">
<code class="language-html">
 // HTML code
 &lt;div class="wavy-line"&gt;&lt;div&gt;

// Css

.wavy-line {
    position: relative;
    width: 100vw;
    height: 50px;
}
.wavy-line::before, .line::after {
    content: "";
    display: block;
    position: absolute;
    width: 100vw; /*same width as container*/
    height: 26px;
}
.wavy-line::after {
    background: linear-gradient(45deg, transparent, transparent 49%, green 49%, transparent 51%);
}
.wavy-line::before {
    background: linear-gradient(-45deg, transparent, transparent 49%, green 49%, transparent 51%);
}
.wavy-line::before, .line::after {
    background-size: 50px 50px;
}

</code>
</pre>
<p></p>

<p>
There you go, and the preview should look like the one below
</p>
<div style="border: 2px solid #ccx; font-size: 18px">
 <div class="wavy-line"></div>
    </div> 


<h3 id="line-hover">
Animate line on hover
</h3>
<p>
Another cool thing you can do with css lines is animating them....
</p>

 <pre class="language-html">
<code class="language-html">
 // HTML code
     &lt;a href="#0" class="line-animate"&gt;
        hover me
    &lt;/a&gt;

// Css

.line-animate {
    display: inline-block;
    text-decoration: none;
    font-size: 26px;
    color: green;
    position: relative;
}
.line-animate:hover.line-animate::after {
    content: "";
    display: block;
    width: 100%;
    height: 4px;
    position: absolute;
    top: 100%;
    background-image: linear-gradient(#ddd,#ddd);
    background-size: 100% .1em;
    animation: animate .5s linear;

}

@keyframes animate {
    0% {
        width: 0;
    }
    50% {
        width: 100%;
    }
    0% {
        width: 0;
    }
}

</code>
</pre>
<p></p>

 <div style="border: 2px solid #ccx; font-size: 18px">
 <a href="#0" class="line-animate">
        hover me
    </a> 
    </div>
<p>
And there you have it, a cool hover line effect created with css
</p>

<h3 id="line-one-side">
Add line in the middle of a word
</h3>

<p>
Have you ever wanted create a header like the one below?
</p>
 <figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/line-article.jpg" alt="image of header text with Line from smashingmagazine" />

<figcaption>
Image of header with line from smashingmagazine
</figcaption>
 </figure>

<p>
What if I told you it is quite easy to do with CSS 
</p>

 <pre class="language-html">
<code class="language-html">
 // HTML code
   &lt;div class="line-before"&gt;
     &lt;span class="line-before__inner"&gt;
     Latest posts
    &lt;/span&gt;
    &lt;/div&gt;

// Css 
.line-before__inner {
 position:relative;
 display:block;
 width:100%;
 color:#333;
 background-position:center;
 z-index:2;
 padding-left:calc(100px + 1em);
}

.line-before__inner::before {
 content:'';
 position:absolute;
 display:block;
 width:100px;
 height:1px;
 background-color:currentColor;
 left:0;
 top:50%
} 

</code>
</pre>
<p></p> 

 <div style="border: 2px solid #ccx; font-size: 18px">
 <div class="line-before">
        <span class="line-before__inner">
   Latest posts
    </span>
    </div> 
    </div> 
<p></p>
<p>
The CSS above is self explanatory, so that's how to add a line in the middle of a text item
</p>

<p>
Thanks for reading
</p>
