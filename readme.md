## Reading
### Books

* [Professional JavaScript for Web Developers](http://www.amazon.com/Professional-JavaScript-Developers-Wrox-Guides/dp/0764579088) (Zakas)
* [Even Faster Web Sites: Performance Best Practices for Web Developers](http://amazon.com/dp/0596522304) (Souders)
* [High Performance Websites](http://amazon.com/dp/0596529309) (Souders)
* [High Performance Javascript](http://amazon.com/dp/059680279X) (Zakas)
* [Javascript Patterns](http://www.amazon.com/JavaScript-Patterns-Stoyan-Stefanov/dp/0596806752) (Stefanov)
* [Designing with Progressive Enhancement](http://www.filamentgroup.com/dwpe/) (Filament Group)
* [Hardboiled Web Design](http://hardboiledwebdesign.com) (Clarke)
* [Javacsript Web Applications](http://oreilly.com/catalog/0636920018421/) (MacCaw)

### Online

* [Dive Into HTML5](http://diveintohtml5.org/)
* [JavaScript - The Core](http://dmitrysoshnikov.com/ecmascript/javascript-the-core/)
* [JavaScript Module Pattern In-Depth](http://www.adequatelygood.com/2010/3/JavaScript-Module-Pattern-In-Depth)
* [jQuery Fundamentals](http://jqfundamentals.com)
* [Google JavaScript Style Guide](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)
* [Namespacing Patterns](http://msdn.microsoft.com/en-us/scriptjunkie/gg578608.aspx)
* [MDN Javascript Docs](https://developer.mozilla.org/en/JavaScript/Guide)
* [Caching Tutorial](http://www.mnot.net/cache_docs/)
* [Responsive Web Design](http://www.alistapart.com/articles/responsive-web-design/)
* [SVG or Canvas](http://dev.opera.com/articles/view/svg-or-canvas-choosing-between-the-two/)
* [Making AJAX Applications Crawlable](http://code.google.com/intl/sv-SE/web/ajaxcrawling/docs/getting-started.html)
* [hasLayout explained](http://www.satzansatz.de/cssd/onhavinglayout.html)
* [MDN's "Learn Javascript"](https://developer.mozilla.org/en-US/learn/javascript)
* [Introduction to Version Control](http://guides.beanstalkapp.com/version-control/intro-to-version-control.html)
* [Version Control with Subversion](http://svnbook.red-bean.com/)
* [Git Community Book](http://book.git-scm.com/)
* [Git From the Bottom Up](http://ftp.newartisans.com/pub/git.from.bottom.up.pdf)
* [Isobar Code Standards](http://na.isobar.com/standards/)
* [Complete Guide to CSS Combinators](http://www.suburban-glory.com/blog?page=131)

## Presentations & Videos
* [Professional Front-end Engineering](http://www.yuiblog.com/blog/2009/03/18/video-koechley-prof2e/)
* [Crockford on Javascript](http://yuiblog.com/crockford/)
* [Chrome Developer Tools (Google I/O 2011)](http://paulirish.com/2011/a-re-introduction-to-the-chrome-developer-tools/)
* [Fixing These jQuery](http://fixingthesejquery.com/)
* [jQuery's Best Friends](http://jquerysbestfriends.com/)

## Tools
* [JSFiddle](http://jsfiddle.net)
* [SpriteMe](http://spriteme.org)
* [JSLint](http://www.jslint.com)
* [JSHint](http://jshint.com)
* [JSONLint](http://jsonlint.com)
* [YUI Compressor](http://developer.yahoo.com/yui/compressor/)
* [IE Testing Apps](http://www.iecss.com/spoon/)
* [WebPagetest](http://www.webpagetest.org)
* [YSlow](http://developer.yahoo.com/yslow/)
* [Google Page Speed Online](http://pagespeed.googlelabs.com)
* [CSS3, Please!](http://css3please.com)
* [jsPerf](http://jsperf.com)
* [jQuery Plugin Starter](http://starter.pixelgraphics.us)
* [iOS Media Query Previewer](http://markboultondesign.com/tools/index.html)
* [MicroJS](http://microjs.com/)
* [Font Squirrel](http://www.fontsquirrel.com)
* [CoffeeScript](http://jashkenas.github.com/coffee-script/)

## Libraries & Frameworks
* [jQuery](http://jquery.com)
* [Raphael](http://raphaeljs.com)
* [LABjs](http://labjs.com)
* [Modernizr](http://www.modernizr.com/)
* [Underscore.js](http://documentcloud.github.com/underscore/)
* [Mustache](http://mustache.github.com)
* [Backbone.js](http://documentcloud.github.com/backbone/)
* [HTML5 Boilerplate](http://html5boilerplate.com)
* [jQuery Mobile](http://jquerymobile.com)
* [Mobile Boilerplate](http://html5boilerplate.com/mobile/)
* [Node.js](http://nodejs.org)
* [QUnit](http://docs.jquery.com/QUnit)



# Front-end Code Standards

## General

### Desktop Browser Support
* IE6-9
* Firefox
* Chrome
* Safari
* Opera

### Core Libraries/Frameworks
* jQuery
* 960 grid system
* HTML5 Boilerplate

### Indentation
Indents should be made with 2 spaces (soft tabs). Be consistent and tidy with your nested HTML elements and code blocks!

### Comments
When appropriate, add comments for the benefit of future developers (and your future self). 

## HTML

### HTML5
We should strive to write valid, HTML5 spec compliant markup, but it's not necessary that every page pass a validation test. And while we want to write code that's HTML5 compliant, there are some HTML5 features that we're not yet using (e.g., semantic elements).  

### Doctype
HTML5 Doctype: 
    `<!DOCTYPE HTML>`

### Minimal boilerplate
    <!DOCTYPE html>
    <html lang="en" class="no-js">
    <head>
      <meta charset="utf-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />  
      <script>(function(H){H.className=H.className.replace(/\bno-js\b/,'js')})(document.documentElement)</script>    
      <!--[if lt IE 9]><script src="/_assets/js/html5-shiv.js"></script><![endif]-->  
  
      <link rel="stylesheet" href="/_assets/css/styles.css" media="all" />
      <!--[if IE]><link rel="stylesheet" href="/_assets/css/ie.css" media="all" /><![endif]-->
  
      <title>Page Title</title>
    </head>
    <body>
    
    </body>
    </html>

### Attributes
Attributes should always be wrapped in quotes (even though they are optional in the HTML5 spec).

### Self-closing elements
We prefer the XHTML syntax for self-closing elements: `<img src="" alt="" />`

### Semantic HTML
Semantic HTML. Write it. Always.

Good:

    <ul class="article-list">
      <li>
        <h3><a href="/some-story">Some Story</a></h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
      </li>
      ...
    </ul>

Bad:

    <div class="article-list">
      <div>
        <p class="article-title"><a href="/some-story">Some Story</a></p>
        <p class="article-teaser">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
      </div>
      ...
    </div>

### CSS and JS in External Files
All CSS and Javascript should be kept in external files. HTML should not contain inline styles, inline Javascript, and embedded stylesheets. The only exceptions to this are small snippets of Javascript init code or analytics tracking code. Embedded/inline CSS and Javascript create performance problems and make code very difficult to maintain. Clean separation of concerns is always a good idea.

Note that when linking to external CSS and Javascript, the `type` attribute is unnecessary. Wrapping Javascript in HTML comments or `CDATA` block is also unnecessary. The `language` attribute should be dropped too.  

## CSS

### Single-line vs multi-line CSS
Both styles are acceptable but only one style should be used for a particular project. Single-line is preferred for faster scanning of large stylesheets. 

One instance where mixing the styles is OK is when writing vendor-prefixed CSS3 rules. In this case, deviating from the single-line style and aligning the vendor-prefixed declarations on separate lines so the values line up is the way to go. For example:

    .rounded { 
         -moz-border-radius: 5px;
      -webkit-border-radius: 5px;
              border-radius: 5px;
    }

### CSS Scope
Global rules should be declared at the top of the stylesheet. In general, the majority of rules should be scoped to a page/module/ancestor. 

If a site has multiple stylesheets, be careful that you're not unintentionally clobbering rules in previously loaded stylesheets.

### CSS Specificity
Be aware of specificity when choosing selectors. Remember that selectors with greater specificity will override selectors with lesser specificity even if the selector with lesser specificity occurs later in the stylesheet. 

The way specificity is calculated is a little complex. It's a good thing to [read up on](http://coding.smashingmagazine.com/2007/07/27/css-specificity-things-you-should-know/).

Please **avoid** using `!important`. It nukes the specificity hierarchy and can make it difficult to debug CSS problems when styles live in multiple stylesheets.

### Combinators and Pseudo-classes
Avoid the child combinator (`>`) as it does not work in IE6. Be careful with other fancy combinators that may not work in various versions of IE.

When using CSS2 and CSS3 pseudo-classes, make sure you know what the browser support is. Generally speaking, because we have to support older versions of IE, things like `:first-child` cannot be used.

### Pixels, Ems
Size fonts in pixels. It's easier and the downsides are now minimal (IE6 can't resize text).

### IE Styles
Our current method of handling IE fixes/hacks is to load a single `ie.css` stylesheet using conditional comments and to target different versions of IE within that stylesheet using hacks. This keeps all the CSS nastiness quarantined in a single file while still allowing us to target IE versions separately.

### Sprites
As a general rule, using CSS sprites is a good idea. Always use sprites for hover state effects. Combining many images into a single master sprite file is sometimes good but sometimes can make things difficult to maintain. When we do use a master sprite file it's usually done at the very end of the development cycle. 

### Style Reset
Don't forget to begin your stylesheets with a CSS reset. The HTML5 Boilerplate reset (taken from the HTML5 Doctor reset) is a good one to use.

## Javascript

### Declaring variables
Always declare variables with the var keyword. Remember that in Javascript variables are function-scoped and identifiers are "hoisted" to the top of the function. It's recommended to declare all variables at the beginning of the function.

#### Preferred:

    function bakeCake(chocolate) {
     var frosting;
     if (chocolate typeof == 'undefined') {
       frosting = true;
     }
    }        
      
#### Discouraged:

    function bakeCake(chocolate) {
     if (chocolate typeof == 'undefined') {
       var frosting = true;
     }
    }
    
### Global Variables
To prevent conflicts with other scripts -- and as a general best practice -- avoid global variables. Use an Object Literal or Module design pattern that namespaces your code to a single app instance. You can also use immediately invoked function expressions (IIFE) to encapsulate your code:

    (function() {
      //All your code here is safely contained within the wrapping function expression
    })();        

### Whitespace in Javascript
Do it like this:

    function bakeCake(chocolate) {
      ...
    }    

### Browser sniffing
Avoid browser/UA sniffs. Instead use feature detection to test for unsupported features (there are lots of libraries to help with this).

### jQuery
We use jQuery as our base Javascript library. One thing to watch out for is overusing jQuery...it's great for DOM manipulation, working with AJAX, and event handling (among other things) but there are plenty of times when it's better to use regular Javascript. 

### Loading
Javascript should be kept in external files that are loaded at the bottom of the page. Asynchronous loaders like LABjs are a good idea, but need to be implemented carefully.

### General Best Practices
* Cache jQuery objects to reduce the number of times you have to query the DOM.
* Minimize interaction with the DOM. If iterating over an array to generate HTML, stuff the HTML into a variable and then do a batch insert into the DOM at the end.
* It's usually best to use strict equality operators (`===` and `!==`) to avoid problems with type conversion.
* Try to write loosely coupled functions that accept parameters and return values.
* Use literal notation when creating new objects and arrays.
* Instead of writing multiple var statements, declare/initialize your variables at the top of the function in a comma separated list.
