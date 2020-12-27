---
layout: post
title: Top 5 Css Methodologies In 2021 
author: Spruce
author_link: spruce.emma
summary: >
   See the top 5 css methodologies in 2021 
tags: css methodologies
image: img/posts/red-button.png
sharing:
  twitter: Top 5 Css Methodologies In 2021
  facebook: Top 5 Css Methodologies In 2021
---

Css is very difficult to manage when you are dealing with a large system, this is because Everything in css is <b>Global</b>

<pre class="language-css">
  <code class="language-css">

&lt;button class="button button-action"&gt;
    Load More
  &lt;/button&gt;

  &lt;!-- css --&gt;

  .button {
    background: blue;
  }
  .button-action {
    background: pink;
  }

  // then maybe after 3 months on line 1299...
  // another developer wants a call to action button
  // and he declares another class with button-action with background color red

  .button-action {
    background: red;
  }

  </code>
</pre>

<p>
  you might be wondering what will be the background color of the button, well like i said earlier everything in css is Global, what will happen is that all three background properties will move to the top of the <b>Scope</b> like this...
</p>
<ol>
<li>
background: blue;
</li>
<li>
background: pink;
</li>
<li>
background: red;
</li>
</ol>
<p>
Then the browser will go through the code and apply all of them. Yeah all of them, and then decide to use the last one
</p>
<pre class="language-css">
  <code class="language-css">
 
 // the browser will read the code like this from top to bottom

  &lt;!-- css --&gt;

   <span style="color: yellow;">background: blue</span>; // oh here is a background with color of blue, use this.

   <span style="color: yellow;">background: pink</span>; // wait, don't use that, here is another background with color pink, definately use this.

   <span style="color: yellow;">background: red;</span> // what's wrong with this developer, here is another background with color red, jeez, is there another one?. nope, then use this.

    &lt;!-- Html --&gt;

    &lt;button class="button button-action"&gt;
    Load More
  &gt;/button&gt;

  </code>
</pre>

<figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/red-button.png" alt="Css red background" />
 
 <figcaption>
Browser will use the red background
 </figcaption>
 </figure>
<p>
The problem of managing css is what every developer must face one way or the other, not to mention (one of the hardest thing in css) naming classes, along the line you are going to run out of class names, that's where css methodologies comes in play(sticking to a particular naming convention)... 
</p>

<h1>
What are css methodologies?
</h1>
<p>
css methodologies are systems that are formaly documented down that help us to auhor/write css as isolated modules, rather than just some long indivisible code.
</p>

<h2>
Top 5 Css Methodologies in 2021
</h2>
<h4>
<a href="https://acss.io">1. Atomic Css</a>
</h4>
<p>
Atomic Css is a collection of single purpose styling units that fits well with components in templated framewoks...
</p>
<p></p>
<h6>
Benefits of using Atomic Css
</h6>
<ol>
<li>
Moves specifity out of the way
</li>
<li>
Improves performance
</li>
<li>
Allows to share content and assets easily
</li>
</ol>
<p></p>
<h6>
Further reading 
</h6>
<ol>
<li>
<a href="https://acss.io/frequently-asked-questions.html">Atomic css frequently asked questions</a>
</li>
<li>
<a href="https://acss.io/quick-start.html">Atomic Css Quick Start</a>
</li>
</ol>

<p></p>

<h4>
<a href="https://getbem.com">2. BEM</a>
</h4>
<p>
BEM stands for - <b>BLOCKS, ELEMENTS and MODIFIERS</b>
</p>
<p>
<b>Block:</b><br>
This are standalone entity that is meaningful on its own <br><br>
<b>Element:</b><br>
A part of a block that has no standalone meaning (it must be used within a block)  <br><br>
<b>Modifier:</b><br>
A flag on a block or element, basically we use this to change the appearance or state of an element.
</p>
<h6>
Benefits of using BEM
</h6>
<ol>
<li>
Modularity
</li>
<li>
Reusability
</li>
<li>
Structure
</li>
</ol>
<p></p>
<h6>
Further reading 
</h6>
<ol>
<li>
<a href="https://getbem.com/introduction/">Intro to BEM</a>
</li>
<li>
<a href="https://www.integralist.co.uk/posts/bem.html">BEM</a>
</li>
<li>
<a href="https://getbem.com/naming/">BEM naming convention</a>
</li>
</ol>
<p></p>

<h4>
<a href="https://getbem.com">3. ITCSS</a>
</h4>
<p>
ITCSS - stands for <b>INVERTED TRIANGLE CSS</b>
</p>
<p>
This is a methodolgy for structuring your css files in the best and stress free way as possible.
</p>
<h6>
Benefits of using ITCSS
</h6>
<ol>
<li>
Less thinking on naming things
</li>
<li>
Reusability
</li>
<li>
Flexibility
</li>
</ol>
<p></p>

<h6>
Further reading 
</h6>
<ol>
<li>
<a href="https://xfive.co/blog/itcss-scalable-maintainable-css-architecture">ITCSS: Scalable and Maintainable Css Architecture</a>
</li>
<li>
<a href="https://hongkiat.com/blog/inverted-triangle-css-web-development/">Intro to ITCSS for web developers</a>
</li>
</ol>
<p></p>


<h4>
<a href="https://smacss.com">4. SMACSS</a>
</h4>
<p>
SMACSS stands for - <b>SCALABLE and MODULAR ARCHITECTURE for CSS</b>
</p>
<p>

<h6>
Benefits of using SMACSS
</h6>
<ol>
<li>
Scalable
</li>
<li>
Ease of Reading
</li>
</ol>

<p></p>

<h6>
Further reading 
</h6>
<ol>
<li>
<a href="https://smacss.com">Smacss guide</a>
</li>
</ol>
<p></p>

<h4>
<a href="https://oocss.org">5. OOCSS</a>
</h4>
<p>
OOCSS stands for - <b>OBJECT ORIENTED CSS</b>
</p>
<h6>
Two main principles of OOCSS
</h6>
<ol>
<li>
Separating Structure From Skin
</li>
<li>
Separating Container And Content
</li>
</ol>

<p></p>
<h6>
Benefits of using OOCSS
</h6>
<ol>
<li>
Maintainable stylesheets
</li>
<li>
Faster websites
</li>
<li>
Easier to modify common styles
</li>
</ol>
<p></p>
<h6>
Further reading 
</h6>
<ol>
<li>
<a href="https://oocss.org">Object oriented Css</a>
</li>
<li>
<a href="https://www.smashingmagazine.com/2011/12/an-introduction-to-object-oriented-css-oocss">Intro to object oriented css on smashingmagazine</a>
</li>
</ol>
<p></p>


<p>
This list is based on the survey from <a href="https://2020.stateofcss.com/en-US/technologies/methodologies/">The state of css 2020</a>, and it is intended to show you the css methodologies that would probably be used in 2021 
</p>

<p>
Another css methodology that is currently on a fast rise is the <a href="https://piccalil.li/blog/cube-css/">Cube Css</a>
</p>

<div class="info info--note">
   <div class="info__content">
       <strong>Note:</strong> There is no best css methodology, the one you decide to use depends on you and the type of your project...
                </div>
          </div>

<p>
Thanks for reading
</p>