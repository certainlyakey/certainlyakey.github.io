---
layout: page
title: An educational interactive demo
excerpt: An interactive demonstration of CSS box model
sampleno: 5
---

##An interactive demonstration of CSS box model 

###_November 2014_, [view on separate page](http://codepen.io/certainlyakey/full/uLrdj)

<p data-height="800" data-theme-id="5749" data-slug-hash="uLrdj" data-default-tab="result" data-user="certainlyakey" class='codepen'>See the Pen <a href='http://codepen.io/certainlyakey/pen/uLrdj/'>Box model and box-sizing live demo</a> by certainlyakey (<a href='http://codepen.io/certainlyakey'>@certainlyakey</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

####Description

This interactive demo was created for a CSS class. It's intended to play a role in learning two important things about CSS: the box model and `box-sizing` property (which effectively toggles the box model). It's based on a useful idea and several tricks that allow to deliver the concept the in a clear and comprehensible, practical-oriented way.

The box model is one of the hardest to explain concepts in CSS, along with specificity, float, and animations. There's a whole bucket of factors that make it difficult to comprehend and teach. 

The first one is that its purpose may not be immediately clear. Compare it to other, easily graspable components of CSS (it's a declarative language, after all) such as properties — mostly, you just set them to any value and see the results right away.  The box model — the system that predicts how padding, margin, border, and given dimensions of a block element will combine visually in browser — is a fairly complex concept, not something you can just type in. Box model dictates whether or not an element’s width and height include padding and border. It is an essential part of CSS in a practical sense for two reasons: the possibility to facilitate the design and development process and importance for compatibility with legacy browsers. Furthermore, it's completely possible to advance in CSS knowing nothing about box model, but chances that such a student will become stuck with its difficulties at a later stage are very high, so learning about box model behavior is necessary.

I decided then to approach the problem visualizing the box model. Visualizing it and not explaining verbally is the right thing to do because it might make even most complex notions accessible to human mind. There are a lot of interactive demos I've made that utilize many free online services related to frontend development such as [JSBin](http://www.jsbin.com), [Codepen](http://www.codepen.io), [Dabblet](http://dabblet.com/) etc. They do a good job regarding learning process because they allow anybody to tinker with code, and web development is all about tinkering (considering what an indispensable part of any web designer toolkit browsers' developer tools are). Another convenient feature is that demos made in these services are embeddable, they are easy to include into class presentations. I'm myself more a man of code and decided to do the visualization in browser, coding it with the same HTML, CSS, Javascript the class was about.

From a visual stand the most obvious solution is to show box model as a scheme (as done in [this article on the matter](https://css-tricks.com/the-css-box-model/), for example). To begin with something, I just coded this scheme into a CSS based graphic in Codepen. Most graphics showing CSS box model do not show how background relates to it because it does not count when model is calculated, but I found that the concept is easier to grasp if you mention how background expands onto padding, so I included background in the scheme too.

It's always optimal when the implementation of a demo is done in such a way that the code itself is a demonstration too, not just the picture rendered by browser. But the markup and CSS code for such a scheme would be too dirty and difficult for students to comprehend at this stage — the box model part of my class went pretty early and most of students wouldn't be able to figure out everything that would appear in the code of the demo. 

Still, it was tempting to make a demonstration that would allow, at least, the code to represent a typical block element to which box model applies — and at most, to be changed by students and show how box model affects the appearance of this element. Therefore, the question is, how to hide one part of the code from students and at the same time show another part? And furthermore, allow it to be tinkered with? That's when I stumbled upon a helpful trick shown earlier by Enrique Moreno Tent [here](http://codepen.io/dbugger/pen/IstHx). More precisely, two tricks — the `<style>` HTML tag is actually styleable itself, and with the help of `contenteditable` attribute it will become interactive. 

That leads us to the desired results — the students see only the CSS that takes part in forming the box model of the displayed element, and they are able to change this CSS code and see how the element box is affected visually. For example, they may change `padding` property, and the appropriate part of the scheme changes. Thus the demo follows the principle of direct manipulation — students may change the demo and immediately see the result, faster and more profoundly getting the idea of box model. As a small bonus, the usual refresh speed of reloading the result screen on services is a little slow, and the `style` tag trick makes refreshing the graphic instant. I also like the technical elegancy of this solution in that it does not require any additional scripts or hacks, relying on already presented browser possibilities.

Still, box model is important not only as a inner browser mechanics. It may be changed by developer. There are several types of box model, and the default one (it's called `content-box`) is not the most design friendly to use because the actual width of an element in browser is not equal the width declared in CSS by a developer, and it may result in misunderstandings (this is just one example of how a mental model and conceptual model do not conform with each other). Another type, called `border-box`, on the other hand, is easily comprehensible — the rendered width and CSS width are the same — and even recommended by web design "rock star" Paul Irish (here's [a link to post in his blog](http://paulirish.com/2012/box-sizing-border-box-ftw/)). (There's a less known third alternative, which is called `padding-box`.)

The `box-sizing` CSS property allows to apply different box model modes, and the demo serves to demonstrate how it actually works. All a student needs to do is just to type in the value. To assist with the visual explanation I added a ruler centered above the box that shows how the width value in CSS (by default 400 pixels) corresponds to the actual width of the box. This is also a good moment to explain how legacy browsers (IE6/IE7) worked this way by default and what problems it created for web designers who had the same block having different sizes in different browsers.

So, to sum up, the advantages of this work as a learning aid in terms of teaching benefits, usability and technical value are these:

- it explains visually (and thus much faster and more clearly) how CSS box model looks, what components it consists of;
- its interactive features allow to show how box model works;
- it represents a good visual guide on `padding`, `border`, 'margin', `width` and `height` properties;
- it follows the principle of direct manipulation in that the changes students make are reflected instantly on the scheme graphic and are very easy to relate in mind;
- `box-sizing` property is covered with the interactive features too, so there's no need to explain it separately;
- it shows in an obvious way the benefit of caring about compatibility — the visual changes in the box provoked by students themselves demonstrate what could happen with it in browsers having different box model modes set by default;
- the demo shows the relationship between box model and an element's background;
- the demo stays interactive even when it's embedded — for example, students can play around with it even in a presentation without need for opening it in a new tab;
- the actual code the demo is made with is still accessible — students may open the page on Codepen and play with it (though it's more for an advanced part of student audience).

But, there's still some room for work left. The current disadvantages are:

- the demo is not self-contained, that is, it has to be consumed with some additional information (it may not be clear what to do with it, so the interactive feature would not be used), for example, in a web-based presentation or in class with verbal explanations of a teacher;
- to follow the previous point, the demo lacks affordances, for example, the changeable box behind the scheme could indicate more clearly that it is interactive;
- the possibility to enter anything into the box may prevent part of the students from guessing what actually should be there. It's not a huge problem for numeric properties, such as `width` and `height` — it's easy to assume that if they already contain numbers you just change the digits. But `box-sizing` property is keyword-based, and students may hesitate to touch it if not told to do so and what to enter. A better decision, for instance, could be to introduce a menu containing all three `box-sizing` values, following the "recognition rather than recall" principle. But that would contradict the mental model of changeable textarea that assumes that you are able to play around with code in any way; 
- the interactive box moves without any warning if a change introduced within the box by a student forces browser to increase or decrease the height of the scheme. This undesired effect may startle the user and breaks the feeling that the page is under his control;
- `margin` property may not be easily understandable — it's not that clear how it works (it pushes the element from boundaries of neighbouring elements) and whether it plays a role in box model or not (it's not).