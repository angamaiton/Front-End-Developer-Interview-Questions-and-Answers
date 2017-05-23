#### General Questions (and Answers):

* What did you learn yesterday/this week?

	I learned how to deal with nested pseudoclasses in complex/old SASS files.
  
* What excites or interests you about coding?

	I'm passionate about creating things, primarily – but I also love to take highly technical concepts and turn them into things that are easy to understand and use.

* What is a recent technical challenge you experienced and how did you solve it?

* What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?

* Talk about your preferred development environment.

	When I first got into development, I prioritized the beauty of an editor over the actual productivity I got out of it – I wanted to feel ahead of the curve and to amaze more senior developers. When my bootcamp had us work with Sublime, I did Atom. When my coworkers used Notepad + +, I used Visual Studio Code. I had an IDE phase, but nothing ever really seemed to really make much of a meaningful difference in my productivity, and I realized that I was focusing too much on my tools instead of what I was building.
	I follow quite a few design blogs and established dev shops, and eventually came across an article by Thoughtbot about Vim, the twenty-year-old text editor that they used. I tried Vim and hated it, but I went back a few times and slowly started to get the hang of it. I'm in love with it now, and I get so much more productivity out of it than I did with almost anything else. I learned how to script, how to manage my Git repositories better, and how to be a better overall developer just from the process of learning how to use it.
* Which version control systems are you familiar with?
	Mainly Git, but I've also used Mercurial.
* Can you describe your workflow when you create a web page?

* If you have 5 different stylesheets, how would you best integrate them into the site?
* Can you describe the difference between progressive enhancement and graceful degradation?
* How would you optimize a website's assets/resources?
* How many resources will a browser download from a given domain at a time?
  * What are the exceptions?
* Name 3 ways to decrease page load (perceived or actual load time).
	There are quite a few ways to do this, but here are three of the most important:
	* Minify your production code with a build tool.
	* Minimize the amount of HTTP requests you make
	*[ Cache resources in the browser, if possible.]
* If you jumped on a project and they used tabs and you used spaces, what would you do?

	I would use tabs to match the project's conventions, create an ESLint config to enforce standard styling throughout the project, and create an .editorconfig file at the root of the project to ensure that developers' editors would use those standards automatically.
  
* Describe how you would create a simple slideshow page.
* If you could master one technology this year, what would it be?

	Elixir. I come from a Rails/JS background, and I've tried to take the best from both environments – I love the mindset of "convention over configuration" in the Rails community, but I love the performance and functional programming style that JavaScript enforces (particularly with tools like Redux and Elm).
	Elixir (and Phoenix) seem to combine the best of both worlds. It's like a newer, better Rails, and it has a lot of great/interesting conventions (it's easy to test, it comes with Brunch instead of Webpack, etc.)
  
* Explain the importance of standards and standards bodies.

* What is Flash of Unstyled Content? How do you avoid FOUC?

	FOUC is when a webpage's content loads before its styles (fonts, colors, etc.) are fully loaded.
  
* Explain what ARIA and screenreaders are, and how to make a website accessible.

* Explain some of the pros and cons for CSS animations versus JavaScript animations.

	Pros:
	* CSS animations are great for small tasks that don't require direct state management – making a tooltip, toggling navbars, displaying an animation when hovering over a <div>, etc.
	* CSS animations are GPU-intensive, not CPU-intensive.
	Cons:
	* Not supported in older browsers, which means that developers need to understand Babel
	* Harder to manage, as CSS doesn't really have logic in the same way JavaScript or other languages do.
  
* What does CORS stand for and what issue does it address?

	Cross-origin resource sharing. It's primarily used to solve the issue of concurrent downloads taking longer from a single source and speed up download time.

