--- 
layout: post
date: "2008-06-06"
title: Skipping Photoshop for web design
comments: true
categories: css
---

Occasionally the folks at 37signals write a blog post that seems to channel thoughts that I've just never put to paper [blog]. This week they did it twice, with <a href="http://www.37signals.com/svn/posts/1061-why-we-skip-photoshop">two</a> <a href="http://www.37signals.com/svn/posts/1066-web-designers-should-do-their-own-htmlcss">posts</a> about how they prefer to skip Photoshop and work with HTML and CSS when it comes to designing a web site.

I've found it incredibly pleasant to work with designers who have demonstrated knowledge and skill when it comes to CSS and HTML -- at my last job, our lead designer was also the guy you went to if you were stumped by a CSS issue. Knowing the tools means that production considerations become an active part of the design process: you don't create an element without giving some thought to how it will be built. In the best of worlds, you weigh the cost of building the element -- in time, in HTTP requests, in excessive markup -- against the benefit of having it on the site, and make educated decisions about what is "worth it."

I've never found Photoshop to be an adequate tool for mocking up a design -- it just doesn't "think" the way the web does, it just doesn't observe the constraints that the web imposes, and it just doesn't make accessible the parts of CSS that are truly powerful.

While I am no designer, I play one sometimes for freelance clients. When I haven't wanted to go straight to code, I've found that another Adobe product, InDesign, can be incredibly powerful. It's an application intended for print layout (and some of its related assumptions can be a little frustrating, such as its lack of a hex-based color picker/setter), but generally it is exponentially closer to the realities of the web than Photoshop. It thinks in boxes, not pixels, and offers paragraph-, character- and object-level stylesheets that can ... cascade! Just like with CSS, you can rapidly and dramatically alter the appearance of a page once you establish the base, semantic elements of it. It steers you to think about a page's structure, not just its presentation.

I'm hoping that the number of web designers who think that Photoshop is a sufficient tool will dwindle, but I'm not sure what the route is to get to that point. Photoshop's inadequacy in this regard is so clear to me -- and to people like the 37signals folks -- that I'm not sure how you persuade someone who still believes otherwise.