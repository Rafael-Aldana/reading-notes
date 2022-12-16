# Class 14 code-201d93

What does a CSS transform allow the developer to do to an element?
The transforms property trnasforms the element into 2-dimensianal or three-dimensional

Provide an example of a transform and how you could see that being used on a website. You can use this 2-dimensional code on something like an online video game.
HTML
1
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>
<figure class="box-3">Box 3</figure>
<figure class="box-4">Box 3</figure>

CSS
1
.box-1 {
  transform: rotate(15deg);
  transform-origin: 0 0;
}
.box-2 {
  transform: scale(.5);
  transform-origin: 100% 100%;
}
.box-3 {
  transform: skewX(20deg);
  transform-origin: top left;
}
.box-4 {
  transform: scale(.75) translate(-10px, -10px);
  transform-origin: 20px 50px;
}
[link-to-reding-notes](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
***************************************************************************************************************************************************
What does a CSS transition allow the developer to do to an element? Transitions provide a change from one state to another.
[link-to-reding-notes](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

How does a CSS animation differ from a CSS transition? Animations can set multiple points of transition upon different keyframes, as opposed to transitions they change one state to another.

***************************************************************************************************************************************************
What are some benefits to using CSS transitions on websites?
Adding transitions to websites will bring excitement in the users increase engagement and ultimately get people talking about your website.

How this topic fit in with your long-term goals? This is the path that the tech industry is headed down towards. Transitions and animations are that extra little bit of spice you need on top of having great CSS it attracts the users attention.
[link-to-reading-notes](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)
