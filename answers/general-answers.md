# General Questions (and Answers):

#### What did you learn yesterday/this week?

I learned how to deal with nested pseudoclasses in complex/old SASS files.
  
#### What excites or interests you about coding?

I'm passionate about creating things, primarily – but I also love to take highly technical concepts and turn them into things that are easy to understand and use.

#### What is a recent technical challenge you experienced and how did you solve it?

CODE GOES HERE

#### What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?

That would depend primarily upon a client's requirements, but here are some general rules I follow:
  
  - **UI**: Simplicity and ease of use above all else. Products should behave intuitively and predictably.
  - **Security**: I prefer using open-source tooling, and security is a metaphorical Prime Directive when it comes to designing and implementing features – it overrides all other concerns, and should be thought of as a feature.
  - **Performance**: This is heavily dependent upon an application's target demographic, but I'm obsessive when it comes to optimization and making good decisions from the outset – I prefer up-to-date tools, and I like modularity and small files that are easy to debug and improve upon.
  - **SEO**: For React, I emphasize SSR (server-side rendering), and I pay attention to `meta` tags when I'm designing the application. Being a (reluctant) millennial, I've also worked on ways to optimize social media performance and output.
  - **Maintainability**: My preferred toolkit revolves primarily around creating maintainable, scalable applications – I try to keep my data immutable, to use tools like Redux for store/state management, and to use statically typed languages like TypeScript or Elm.
  - **Technologies**: I enjoy using and experimenting with new technologies, but I tailor what I use according to the application I'm making. I prefer well-documented and widely used technologies wherever possible.
  
#### Talk about your preferred development environment.

When I first got into development, I prioritized the beauty of an editor over the actual productivity I got out of it – I wanted to feel ahead of the curve and to amaze more senior developers. When my bootcamp had us work with Sublime, I did Atom. When my coworkers used Notepad++, I used Visual Studio Code. I had an IDE phase, but nothing ever really seemed to really make much of a meaningful difference in my productivity, and I realized that I was focusing too much on my tools instead of what I was building.

I follow quite a few design blogs and established dev shops, and eventually came across an article by Thoughtbot about Vim, the twenty-year-old text editor that they used. I tried Vim and hated it, but I went back a few times and slowly started to get the hang of it. I'm in love with it now, and I get so much more productivity out of it than I did with almost anything else. I learned how to script, how to manage my Git repositories better, and how to be a better overall developer just from the process of learning how to use it.
  
#### Which version control systems are you familiar with?

Mainly Git, but I've also used Mercurial.
  
#### Can you describe your workflow when you create a web page?

  1. Go over the mockups and wireframes (and if there are none, make sure that my idea of what the page should look like matches the official spec) – this gives me a clear picture of what I'm doing and why, and helps with my workflow.
  2. Decide on my tooling. Depending on the project requirements, I pick different tools (if I'm handing it off later, I pick more easily accessible tools (SASS > PostCSS, React > Vue, Rails > Sinatra, etc.).
  3. Write out acceptance and functionality tests, and ensure that they fail appropriately.
  4. Code the site. I start with the largest pieces and work my way down, making each test pass.
  5. Integrate Travis CI.
  6. Publish my code and ensure that all tests pass.
  7. Deploy.

#### If you have 5 different stylesheets, how would you best integrate them into the site?

A good way of doing this would be using a preprocessor like SASS to nest and merge them together into a single source, and then minify the output in production.

#### Can you describe the difference between progressive enhancement and graceful degradation?

**Progressive enhancement** is a web design strategy where developers implement basic features supported universally and then enhance them according to more advanced requirements on different environments.

**Graceful degradation**, on the other hand, is a strategy where the most advanced features and pieces are implemented, and additional work is done to support environments where features don't work or perform poorly.

#### How would you optimize a website's assets/resources?

  A few examples:
    * Minify/uglify CSS and JavaScript
    * Use a CDN
    * Convert images to CSS sprites
    * Compress images
    * Serve images from different domains (CORS)
  
#### How many resources will a browser download from a given domain at a time?

It depends on the kind of browser – up-to-date Chrome, Firefox, and other major browsers should handle six to eight concurrent downloads, but older browsers will support much fewer. I use http://www.browserscope.org/ if there's a specific number that I need to know immediately.

#### What are the exceptions?

An example would be using subdomains that point at the same parent domain – implementing these helps increase the concurrency level of the download.

#### Name 3 ways to decrease page load (perceived or actual load time).

There are quite a few ways to do this, but here are three of the most important:
   * Minify your production code with a build tool.
   * Minimize the amount of HTTP requests you make
   * Cache resources in the browser, if possible.
   
#### If you jumped on a project and they used tabs and you used spaces, what would you do?

I would use tabs to match the project's conventions, create an ESLint config to enforce standard styling throughout the project, and create an .editorconfig file at the root of the project to ensure that developers' editors would use those standards automatically.
  
#### Describe how you would create a simple slideshow page.

  CODE GOES HERE

#### If you could master one technology this year, what would it be?

Elixir. I come from a Rails/JS background, and I've tried to take the best from both environments – I love the mindset of "convention over configuration" in the Rails community, but I love the performance and functional programming style that JavaScript enforces (particularly with tools like Redux and Elm).

Elixir (and Phoenix) seem to combine the best of both worlds. It's like a newer, better Rails, and it has a lot of great/interesting conventions (it's easy to test, it comes with Brunch instead of Webpack, etc.)
  
#### Explain the importance of standards and standards bodies.

In a nutshell, standards are useful because they make it easier for developers to use the same markup across different browsers and be sure that the page works the same way across rendering engines. Standards reduce the need for checking user agents and for writing specialized code to target older/different browsers.

For an example of what goes wrong when companies don't adopt or comply with standards, see Internet Explorer.

#### What is Flash of Unstyled Content? How do you avoid FOUC?

FOUC is when a webpage's content loads before its styles are fully loaded and applied. An example would be when style tags are placed after other content or applied asynchronously by JavaScript.

In order to avoid FOUC, styles should be placed in order so that they are loaded and applied alongside their matching HTML elements – developers can put styles in the `head`.
  
#### Explain what ARIA and screenreaders are, and how to make a website accessible.

ARIA and screen readers are used to make websites more accessible for disabled users. In order to make websites more accessible, developers should use semantically meaningful tags when building websites (for newer HTML5 content, for example, we use `section`, `aside`, and `main` to help screen readers understand what to prioritize, or `alt` attributes on `img` tags for blind/visually impaired readers).

#### Explain some of the pros and cons for CSS animations versus JavaScript animations.

##### Pros:
  - CSS animations are great for small tasks that don't require direct state management – making a tooltip, toggling navbars, displaying an animation when hovering over an element, etc.
  - CSS animations are GPU-intensive, not CPU-intensive.
  
##### Cons:
  - Not supported in older browsers, which means that developers need to understand Babel
  - Harder to manage, as CSS doesn't really have logic in the same way JavaScript or other languages do.
  
#### What does CORS stand for and what issue does it address?

Cross-origin resource sharing. It's primarily used to solve the issue of concurrent downloads taking longer from a single source and speed up download time.

