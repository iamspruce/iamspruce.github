---
layout: post
title: Create A Blog On Your Mobile Phone Part 3 
author: Spruce
author_link: spruce.emma
summary: >
   Creating a blog on your mobile phone final series, and in this series you are going to learn how to actually blog, and publish your first post as a blogger... 
tags: Mobile Blog Design
image: img/posts/mobile-blog-3/preview-web.png
sharing:
  twitter: Create A Blog On Your Mobile Phone Part 3
  facebook: Create A Blog On Your Mobile Phone Part 3
---

<p class="lead">
Sad to announce the end of this "how to create a blog on your mobile phone series", well i know we have learned a lot of new things in this web series
</p>
<h6>
Some things we have learned so far
</h6>
<ol>
<li>
what mobile blogging is
</li>
<li>
how to create a free website on github with jekyll
</li>
<li>
how to clone your website to your mobile phone
</li>
<li>
how to run some basic Git Commands in your mobile phone
</li>
<li>
and so many other things
</li>
</ol>
<p>
incase you missed the other series, don't worry you can always go back and read them up
</p>
<h6>
Link to previous series
</h6>
<p>
<a href="{{ site.baseurl }}/blog/create-a-blog-on-your-mobile-phone-with-jekyll-on-github.html">Create a blog on your mobile phone part 1</a>
 </p>
 <p>
<a href="{{ site.baseurl }}/blog/create-a-blog-on-your-mobile-phone-with-jekyll-on-github-part-2.html">Create a blog on your mobile phone part 2</a>
 </p>
 <p>
Now lets go back to what we are really here for, blogging from your mobile phone
 </p>

 <h1>
What is blogging
 </h1>
 <p>
 <b>Blogging</b> refers to writing, photography, and other media that is self-published online.
 </p>

 <p>
So basically you know what blogging is all about, its a way for a lot of people to express their feelings and share there ideas online.
 </p>

 <h2>
Blogging with jekyll
 </h2>
 <p>
your blog posts live in a directory called <b>_posts</b> in the root of your site, so basically thats where you will add all your blog posts
 </p>

 <p>
Your blog file names begin with "year-month-date-your-title.md" <br>
so when creating your post, always follow the order <b>Year</b>-<b>month</b>-<b>date</b>-<b>title</b>.md 
 </p>
 <p>
for a detailed on how to write blog posts on jekyll please refer to this jekyll guide below <br> <br>
<a href="https://jekyllrb.com/docs/posts">Learn more about jekyll post</a>
 </p>
 <h3>
Publishing your first post
 </h3>
 </p>
The first step is to open your spck editor, <a href="{{ site.baseurl }}/blog/create-a-blog-on-your-mobile-phone-with-jekyll-on-github.html">The editor you downloaded in the first part of this series</a>, open it and navigate to your _posts folder
 </p>
 <figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/mobile-blog-3/spck-preview.png" alt="Jekyll  _posts folder in spck editor" />

  <figcaption>
   _Posts folder looks like this
  </figcaption>
 </figure>
 <p>
Go ahead and delete the post found there and create another one with <br> <br>
YEAR-MONTH-DAY-TITLE.md format
 </p>
 <figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/mobile-blog-3/spck-post.png" alt="new post in jekyll spck editor" />

  <figcaption>
  Add new file
  </figcaption>
 </figure>
 <p>
After you created the post <br>
add your layout and title like this
 </p>

 <pre class="language-yml">
<code class="language-yml">
---
layout: post
title: welcome to my blog
---
</code>
 </pre>
 <figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/mobile-blog-3/spck-edited.png" alt="Edit jekyll config file in spck editor" />

  <figcaption>
  Modify jekyll site on spck editor
  </figcaption>
 </figure>

 <p>
Now you can add anything to your blog post, after all you are now a blogger, after you are done with writting your post, just go ahead and commit your changes and then push them online like we learned in our <a href="{{ site.baseurl }}/blog/create-a-blog-on-your-mobile-phone-with-jekyll-on-github-part-2.html">previous post</a>
 </p>

 <p>
and there you have it, you just created your first post, go ahead and preview your new post online
 </p>

 <figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/mobile-blog-3/preview-mobile.png" alt="Jekyll image folder in spck editor" />

  <figcaption>
  this is what your new website look like in a mobile view
  </figcaption>
 </figure>

 <p></p>
 <p></p>
 <figure class="p-article__img">
  <img src="{{ site.baseurl }}/assets/img/posts/mobile-blog-3/preview-web.png" alt="Jekyll image folder in spck editor" />

  <figcaption>
  this is what your new website look like in a pc view
  </figcaption>
 </figure>

 <h4>
 Previous posts from this series
 </h4>
 <p>
<a href="{{ site.baseurl }}/blog/create-a-blog-on-your-mobile-phone-with-jekyll-on-github.html">Create a blog on your mobile phone part 1</a>
 </p>
  <p>
<a href="{{ site.baseurl }}/blog/create-a-blog-on-your-mobile-phone-with-jekyll-on-github-part-2.html">Create a blog on your mobile phone part 2</a>
 </p>

 <h5>
Other resources to learn from
 </h5>
  <p>
<a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web"> Getting Started With The Web </a>
 </p>
  <p>
<a href="https://jekyllrb.com/tutorials/home/">Jekyll tutorials home</a>
 </p>
  <p>
<a href="https://jekyllrb.com/docs/step-by-step/08-blogging/">Blogging in jekyll</a>
 </p>

 <p>
thanks for reading.... 
 </p>