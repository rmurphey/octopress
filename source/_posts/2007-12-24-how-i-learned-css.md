---
layout: post
date: "2007-12-24"
title: How I learned CSS
comments: true
categories:
  - css
  - front-end development
  - thoughts
---

I remember when I first tried to understand how to produce designs for the web -- coming from the paper-based world, it was hard for me to accept everything that was suddenly out of my control. When I first tried to grasp CSS with the help of now-defunct Adobe GoLive, I bailed pretty quickly. Table-based layout and font tags didn't make much sense to me either -- why did I have to slice up a page into a bunch of adjoining cells, instead of just drawing independent boxes like I did in Quark?

A couple of years later, I decided to try again, motivated by the realization that my <a href="http://gmurphey.com/">eight-years-younger brother</a> seemed to be better at this web stuff than I was. I spent untold hours trying to wrap my brain around <a href="http://www.sustainablewebdesign.com/resources/601/">the difference between margin and padding</a> and exactly how to <a href="http://css.maxdesign.com.au/floatutorial/">get floated elements to bend to my will</a>. I remember the epiphany that one could <a href="http://www.sovavsiti.cz/css/horizontal_menu.html">use left-floated list items for a horizontal menu</a>, or that <a href="http://www.netmechanic.com/news/vol4/html_no22.htm">the right DOCTYPE can force Internet explorer to behave more like a real browser</a>.

These days, I have an honest-to-god job doing this stuff, and every now and then, someone will ask me how they can learn it too. It all makes so much more sense to me than it used to that it's hard to remember how I got here. In the interest of getting this stuff written down for passing along, though, here are a few thoughts:

<h3>The Tools</h3>
These are things without which the rest is impossible:
<ul>
<li>
<strong>A text editor</strong> Notepad will do just fine; for a few bucks, you can get <a href="http://macromates.com/">TextMate</a> for Mac or the <a href="http://www.e-texteditor.com/">e Text Editor</a> for PC. If you use Dreamweaver, hide everything but the file navigator panel and the code editing view. <em>You will learn nothing from Dreamweaver's "design" view.</em>
</li>
<li>
<strong><a href="http://www.mozilla.com/en-US/firefox/">Firefox</a></strong> You'll need to test anything you do in Internet Explorer, but first, you'll get it working in Firefox. Whereas Internet Explorer enjoys mocking web standards, Firefox does its best to adhere to them; plus, it has all sorts of extensions that make it easier to troubleshoot your work.</li>
<li>
<strong><a href="https://addons.mozilla.org/en-US/firefox/addon/60">Firefox Web Developer Toolbar</a></strong> This has all sorts of useful tools in it, including a real-time CSS editor that opens in the browser's sidebar so you try changes to your CSS and see the results immediately.</li>
<li>
<strong><a href="https://addons.mozilla.org/en-US/firefox/addon/1843">Firebug</a></strong> This is most useful for Javascript debugging, but it has some nice features for debugging CSS as well.</li>
<li>
<strong><a href="http://users.skynet.be/mgueury/mozilla/">HTML Validator</a></strong> Incredibly helpful for finding errors in your HTML.</li>
</ul>

(An aside: A few months ago I booted up an old laptop and found a preview release of Firefox 1.0 installed beside a well-worn Internet Explorer 6; when I abandoned the laptop, I was in the process of abandoning IE too. I can't help but wonder how difficult my learning would have continued to be without the arrival of Firefox, which, with the extensions mentioned above, makes it so much more possible to learn all of this stuff in a very tangible, immediate sort of way.)

<h3>Learning with Firefox</h3>
Once you have the tools above, open Firefox and start with a page someone else built -- like the one you're on right now -- and see what's inside. It pays to be curious about every web page you visit; if you see something interesting, view the source and figure out how it got there. Some tips:

<ul>
<li>
<code>Ctrl-U</code> will show you the HTML for a page, and with the HTML Validator extension, you can "clean up" the HTML so it's easier to read.</li>
<li>
<code>Ctrl-Shift-E</code> will open the Web Developer Toolbar CSS editor, which will show you the CSS for the page, with a tab for each CSS file. You can edit the CSS in the editor and see the effects immediately.</li>
<li>
<code>F12</code> will open Firebug. In the top left of the panel that opens, click the Inspect menu item, then move your mouse back to the page itself and click on an element to find out more about it. You can also click on the HTML tab to view the HTML and expand and collapse sections of it to see the structure of the page. Hovering over an element in the HTML panel will highlight it on the page; clicking on an element will let you find out more about it in the Style and Layout tabs of Firebug. (Firebug is an incredibly powerful tool that you really need to play with to fully appreciate. It's a completely non-destructive tool -- you can't hurt anything with it unless you try really, really hard -- so don't be afraid to click around and see what happens.)</li>
<li>Remember that these days, lots of page elements are built with Javascript rather than with straight HTML. <code>Ctrl-U</code> will show you only the HTML; Firebug will show you the "generated source," including any elements built with Javascript. Firebug also lets you look at the Javascript on a page, which can be helpful when you're trying to understand how something got there.
</li>
</ul>

<h3>POSH</h3>
<a href="http://www.456bereastreet.com/archive/200711/posh_plain_old_semantic_html/">Plain-old semantic HTML</a>. When you go to make a web page, write the simplest HTML you can, and use standard HTML elements whenever humanly possible. Start by creating HTML that represents the actual sections of the page -- header, navigation, sidebar, content, footer -- and give the elements names that say what they <em>are</em>, not where they go. When you think you're done, view the HTML in a browser, without CSS, and see if it makes sense. Then, <em>and only then</em>, open the browser's CSS editor and start styling the elements. See how far you can get without adding any design-related markup to your HTML. If you find yourself writing convoluted HTML or adding purely presentational markup, to make something work, it's time to reconsider your approach. Once you have a good stylesheet started, copy it to your text editor and continue working on it there.

<h3>Strategies</h3>
It helps to give yourself deadlines, even if they're imaginary. I've learned more about HTML, CSS and Javascript in the past 12 months than I learned in the three years before, and I think that's largely because deadlines have forced me to solve problems rather than pondering them.

Don't be afraid to do something less than perfectly; there can be value in just getting it done. I constantly look back at things I did three months ago -- let alone three years ago, and sometimes three weeks ago -- and I cringe when I think how differently I would do them today. But half the reason I know what I know now is precisely because I <em>didn't</em> know it then, and I learned it along the way. Understanding the building blocks of the web is an iterative process, and you'll do better if you remember that <strong>you cannot know everything you wish you knew</strong>.
