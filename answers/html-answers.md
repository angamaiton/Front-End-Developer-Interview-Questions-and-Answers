# HTML Questions

#### What does a `doctype` do?

Doctypes specify the markup standard used by a page and tell the browser how to render a page according to its source code.

#### What's the difference between standards mode and quirks mode?

In standards mode, a browser's engine will render a page as required by HTML and CSS specifications. Quirks mode is used to render legacy pages written before the adoption of fixed standards which contain irregular behaviors found in older browsers.

#### What's the difference between HTML and XHTML?

XHTML was designed to solve cross-browser compatibility issues by requiring more precise standards and specifications than < HTML5. I haven't seen it used in an application since the release of HTML5.

#### Are there any problems with serving pages as `application/xhtml+xml`?

IE < 8 shows a download dialog for pages instead of rendering them properly.

#### How do you serve a page with content in multiple languages?

Internationalization is achieved by using the `lang` tag, sending language-specific metadata, and sending a `Content-Language` HTTP header to the server.

#### What kind of things must you be wary of when design or developing for multilingual sites?

- `hreflang` attr in link
- `dir` attr indicating language direction, such as `rtl`
- `<meta charset='UTF-8'>`
- `font-size` for `:lang({language_code})` selectors in CSS
- difference in word length for each language

#### What are `data-` attributes good for?

They allow HTML elements to contain extra information (data) without using non-standard/hacky attributes.

#### Consider HTML5 as an open web platform. What are the building blocks of HTML5?

HTML5 is composed of HTML elements, CSS, SVG components, and JavaScript. As far as building blocks go, HTML5 adopted a great number of new blocks like more semantic markup/naming, APIs for different resources (audio, video, etc.).

#### Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

Each one of these is a client-side storage mechanism inside the browser, but they all function differently. `sessionStorage` only lasts until the browser is closed, while `localStorage` is stored for an indefinite period of time. Cookies also last indefinitely, but only store strings in plaintext and are sent with every request to the server. `localStorage` and `sessionStorage` both allow JavaScript objects to be stored, and are good for storing insecure data.

#### Describe the difference between `<script>`, `<script async>` and `<script defer>`.

- `<script>` stops the page from rendering while it downloads and runs a script.
- `<script async>` downloads and asynchronously runs a script without stopping the page from rendering.
- `<script defer>` downloads the script in the background without stopping the page from rendering – upon the download's completion, the page stops rendering and runs the script.

#### Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

Positioning `<link>`s between the head allows pages to render styling before executing scripts, which stops users from seeing blank pages while their content is loading. Putting `<script>`s just before the end of the `<body>` runs JavaScript after the page has fully loaded everything else, which also stops users from seeing white screens while the scripts load.

#### What is progressive rendering?

When a HTTP response is flushed multiple times, a browser doesn't wait until
the whole content is loaded and renders each part earlier.

#### Have you used different HTML templating languages before?

Yes. Here's a list of them by language:

- **JavaScript**: EJS, Pug (Jade)
- **Ruby**: ERB, HAML
- **Python**: Jinja2, Django
- **Elixir**: Phoenix templates
- **PHP**: Laravel Blade
