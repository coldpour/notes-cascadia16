# CascadiaFest 2016

* [CSS Day](#css-day)
* [Browser Day](#browser-day)
* [Node Day](#node-day)

Here are my tl;drs for the talks that I saw last week at [CascadiaFest](http://2016.cascadiafest.org). Videos of all the talks will be posted to the [CascadiaJS YouTube Channel](https://www.youtube.com/user/cascadiajs/playlists) in a few days.

Check out the [#cascadia16](https://twitter.com/hashtag/cascadia16?src=hash) hastag on Twitter. Also, [@floriidaaa](https://twitter.com/@floriidaaa) tweeted her sketchnotes from many of the talks which sum up the slides in a single page. 

## CSS Day

1. [Natalya Shelburne - Practical color theory for people who code](https://2016.cascadiafest.org/speakers/natalya-shelburne/)
 * Creating a color pallete is not magic, it's science and here's the [formula](http://tallys.github.io/color-theory/).
1. [Justin McDowell - Bauhaus in the Browser](https://2016.cascadiafest.org/speakers/justin-mcdowell/)
 * Bauhaus was a German collective that pushed the envelope of typography and graphic design. We are just now starting to be able to replicate their designs in CSS.
1. [Miriam Suzanne - Code Patterns for Pattern-Making](https://2016.cascadiafest.org/speakers/miriam-suzanne/)
 * Good patterns combine languages in ways that add meaning to your code by relating elements with common purpose. Get on the same page with your naming conventions. Abstract in layers.
1. [Mike Kivikoski - CSS Pseudo – :hover, ::after and beyond](https://2016.cascadiafest.org/speakers/mike-kivikoski/)
 * Pseudo selectors are like regular expressions. They are amazingly powerful and flexible. Please wield with an eye toward maintainability and common understanding on your team.
1. [Clarissa Peterson - Creating Beautiful, Accessible, and User-Friendly Forms](https://2016.cascadiafest.org/speakers/clarissa-peterson/)
 * Form elements ask questions of your users. Whittle down to the bare minimum number of questions you need to ask. Put directions at the top. Then make sure it still works in a screen reader. Oh and not everyone understands what red asterisks mean.
1. [Stephanie Hobson - Flipping Tables: Displaying Data on Small Screens](https://2016.cascadiafest.org/speakers/stephanie-hobson/)
 * Using a table for layout (lists, columns, etc...) is like crack. Don't do it, not even once. Tables are for displaying data that can be sorted, compared, cross-referenced, and calculated. If you're not going to allow sorting in your mobile browser, don't use a table to display the data. Make a card that contains the data for each entry that fits nicely on the screen or a graph to visualize the data.
1. [Alice Bartlett - “Can't you just make it more like Bootstrap” | Considerations for creating a component system](https://2016.cascadiafest.org/speakers/alice-bartlett/)
 * We wrote a component library called [Origami](http://origami.ft.com/) to unify the look and feel of the ~100 sites that make up the Financial Times online presense. It's not only a technical process, it's also political. People won't fight you, they'll just ignore you unless you can force the issue. 
1. [James Steinbach - Using Sass & PostCSS Together](https://2016.cascadiafest.org/speakers/james-steinbach/)
 * Sass and PostCSS are both preprocessors that do certain things really well. Use them for their individual strengths.
1. [Tyler Sticka - SVG: So Very Good](https://2016.cascadiafest.org/speakers/tyler-sticka/)
 * Most image formats express images in a bitmap of pixels. SVG expresses images in xml which is parseable and codeable by both humans and machines. The files are smaller and the rendered images are always higher fidelity on any screen size. Animate them to create native feeling apps in the browser.
1. [Lourdes Montano - Learning and feeling overwhelmed: methods to organize your learning process in CSS](https://2016.cascadiafest.org/speakers/lourdes-montano/)
 * Programming is hard, staying current is hard, getting discouraged is easy. Learn new things only when they seem relevant. Look back at your old code to see how you've changed. Respect your own learning pace. View messy projects as a learning opportunity.
1. [Gregor Martynus - Welcoming Communities](https://2016.cascadiafest.org/speakers/gregor-martynus/)
 * Building a community around your open source project takes more work and different skills than just writing and publishing the code. Don't treat people like code. Be generous when you interpret what people say. Say, "thank you" when people contribute. Respond quickly and tell people that it will take time to review and give them a thorough response. It's easier to contribute to projects that are broken up into small modules with good documentation.
1. [Alan Stearns - Becoming Responsible for CSS](https://2016.cascadiafest.org/speakers/alan-stearns/)
 * Browsers are evolving to support the features you want. CSS, HTML, and JS standards writers want input from developers, their users. Submit browser bugs. Do it.

## Browser Day

### Rebecca Murphey - Making it better without making it over

Every technology decision is eventually regrettable. Apply the shiny new techniques you're learning about on twitter and at conferences to the codebase you're maintaining. Refactoring is cheaper becuase you can keep making money while making things better.

[Slides](

### Nolan Lawson - Demystifying Web Workers and Service Workers

Noticing 'jank' on your site? That's cause JS code and DOM updates run in the same thread. You only have 16.7ms to do your JS calc. Web Workers run in a background thread for the tab. Service workers run in a background thread even if the tab is closed. Use Web Workers to remove 'jank' and Service Workers to create an offline experience complete with push notifications.

[Slides](https://nolanlawson.github.io/cascadia-2016/#/)
[Twitter](https://twitter.com/nolanlawson)
[Github](https://github.com/nolanlawson)

### Seth Samuel - Arbitrary Computation on the GPU Using WebGL

If you have a large computation you want to do from the browser and you can express it as matrix multiplication, you can use the GPU directly from the browser and speed it up by a lot.

[Slides](http://sethsamuel.github.io/talks/2016-08-03-cascadiafest/public/)
[Twitter](https://twitter.com/sethfsamuel)
[Github](https://github.com/sethsamuel)

### Liz Abinante - In Defense of Static Sites

Don't rebuild a select form element in JS. You'll get it wrong. Do you really need a database? Do you really need a server? Do you really need JS at all? HTML and CSS load fast and do a lot already especially with templaters and preprocessers. Don't start with complexity by default, only add if you really need it. 

[Slides](https://speakerdeck.com/feministy/in-defense-of-static-sites)
[Twitter](https://twitter.com/feministy)
[Github](https://github.com/feministy)

### Noah Adams - Scripting in the 3rd party: True tales of horror and hope from other people's pages

Writing code to inject into other people's webapp is probably the hardest thing ever. Think about combining every active browser variant, with every historical version of every library. Hacking hacks is the status quo.

[Slides](https://noahadams.github.io/scripting-in-the-third-party/#/)
[Twitter](https://twitter.com/noah_adams)
[Github](https://github.com/noahadams)

### Tara Scherner de la Fuente - Onboarding Superheroes

New employees are your company's lifeblood. Only you have the power to make their onboarding experience awesome. Reintroduce yourself later. Make a secret pact to remind them of people's names. Make another secret pact to answer their stupid questions. Ask, "what are your dietary preferences" so you don't presume anything.

[Twitter](https://twitter.com/MediaRemedial)
[Github](https://github.com/wisetara)

### Rachel White - JavaScript as Play: A primer on getting started with video games

[Slides]()
[Twitter](https://twitter.com/ohhoe)
[Github]()

### Thomas Wilburn - Custom elements in production

Web components are reusable, building blocks that are simple to use and don't require proprietary frameworks.

### Sarah Meyer - JavaScript Minus JavaScript

Your site should work with Javascript disabled. As a web-dev, you have one job, render comprehensible HTML quickly. Ignoring accessibility is a sure path to the dark side.

### Dale Bustad - Embrace HTTP/2 Server Push

HTTP/2 can speed up your page load times by parallelizing your requests. It also remembers that you already did the SSL handshake and eliminates it on subsequesnt requests. Bundling becomes obsolete. So use [interlockjs](https://github.com/interlockjs/interlock) instead.

### Marcy Sutton - Where in the Stack is Carmen Sanfrancisco?

Accessibility problems can creep into your app from every part of your stack. Be vigilent and test in a screen reader. Several browser extensions exist to find accessibility problems on the page.

## Node Day

### Mariko Kosaka - Making a Robot Eye with JavaScript - or Magic of Computer Vision Unraveled

Images are just data and computer vision is just interpreting that data. You can access the data through the browsers' `<canvas>` element and then write your own color filters or detect edges or specific images all in browser js.

### Pawel Szymczykowski - Why did the robot cross the road? Computer vision, robots and mobile games.

Need to watch ads to level up or unlock characters in your phone game? Don't watch the ads yourself, build a robot to watch and tap through ads for you.

### Russell Hay - Happy Sparkle Glitter Fun Zone - LEDs and JavaScript

You can program LEDs with JS to tell you the weather forecast at a glance, complete with rain animations.

### Jenn Turner - Open Source beyond software

There's more to your open source project than the software. Separating people into "coders" and "non-coders" is useless and needlessly degrading. If you want your project to thrive, welcome all contributers and their talents.

### Ivana McConnell - Our Identities Have No Bodies: Web, Code, and Self-Exploration

It's becoming less acceptable to be annonymous on the web which prevents people from exploring various parts of their identity that they may want to keep private. It can also lead to harassment. When building new experiences online, consider if you can allow your users to remain annonymous.

### Bryan Hughes - API Design Through the Lens of Photography

Learn an art. Embrace your constraints. Build beautifully creative APIs.

### Brock Whitten - To the Moon! - Overcoming latency for fun and adventure.

Network, disk, memory, redis, in-process LRU cache. Each of these is an order-of-magnatude faster than the previous. With 5 orders of magnatude to play with, make fast applications.

### Nwokedi Idika - Demystifying the Darknet in 30 Minutes or Less

If you want to browse the darknet or communicate with servers annonymously, download the TOR browser. The TOR protocol is like locking your message in a series of lockboxes that can only be opened by the individuals you specify. The individuals don't know where the message came from of where it's ultimately going.

### Bill Automata - require('crypto') is a human right

Strongly encrypt all of your app's network traffic. Your users deserve it.

### Safia Abdalla - The Hitchhiker's Guide to All Things Memory in Javascript

If your app crashes the browser, has jank, or just sucks, use memwatch, heapdump, v8-profiler, and other performance monitoring tools to see if the garbage collector is having to work overtime cleaning up after you.

### Stephan Bönnemann - Greenkeeper – managing dependencies with confidence

Dependency management is hard for for good reason. [Greenkeeper](https://greenkeeper.io/) makes it way easier.

### Alejandro Oviedo - Demystifying (JavaScript) engines

All 4 JS engines are open source. [V8](https://developers.google.com/v8/), [JavaScriptCore](http://trac.webkit.org/wiki/JavaScriptCore), [ChakraCore](https://github.com/Microsoft/ChakraCore), [SpiderMonkey](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/SpiderMonkey). They take source, parse it, transform it into bytecode and execute it. They all do it slightly differently. They all implement GC slightly differently. They all perform slightly differently.
