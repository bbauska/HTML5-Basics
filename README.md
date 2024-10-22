<!-- HTML Basics -->
<h1 id="html-basics">HTML Basics</h1>

<h2 id="topics">Related Topics</h2>
<ul>
  <li><i><a href="https://github.com/learning-zone/css-basics">CSS Basics</a></i></li>
  <li><i><a href="https://github.com/learning-zone/javascript-basics">JavaScript Basics</a></i></li>
</ul>

<br/>

<h2><a id="toc">Table of Contents</h2>

<ol>
  <li><a href="#01-intro">Introduction</a></li>
  <li><a href="#02-html-tags">HTML Tags</a></li>
  <li><a href="#03-html-events">HTML Events</a></li>
  <li><a href="#04-html-forms">HTML Forms</a></li>
  <li><a href="#05-html-tables">HTML Tables</a></li>
  <li><a href="#06-html-lists">HTML Lists</a></li>
  <li><a href="#07-html-iframe">HTML Iframe</a></li>
  <li><a href="#08-html-url">HTML URL</a></li>
  <li><a href="#09-html-svg">HTML SVG</a></li>
  <li><a href="#10-html-canvas">HTML Canvas</a></li>
  <li><a href="#11-html-storage">HTML Storage</a></li>
  <li><a href="#12-html-apis">HTML API's</a></li>
  <li><a href="#13-html-dragndrop">HTML Drag and Drop</a></li>
  <li><a href="#14-html-webworker">HTML Web Worker</a></li>
  <li><a href="#15-html-misc">HTML Miscellaneous</a></li>
  <li><a href="#16-misc">Miscellaneous</a></li>
  <li id="#improve-perf">Ways to improve website performance</h3>
</ol>

<h2 id="01-intro">01. Introduction</h2>

<h3>Q. What is difference between HTML and XHTML?</h3>

The Extensible Hypertext Markup Language, or XHTML, has two important notes for front 
end developers.

1) It needs to be well formed, meaning all elements need to be closed and nested correctly 
  or you will return errors.
2) Since it is more strict than HTML is requires less pre-processing by the browser, which 
  may improve your sites performance.

<h3>Q. What are the building blocks of HTML5?</h3>

<ul>
  <li><b>Semantics</b>: allowing you to describe more precisely what your content is.</li>
  <li><b>Connectivity</b>: allowing you to communicate with the server in new and innovative ways.</li>
  <li><b>Offline and storage</b>: allowing webpages to store data on the client-side locally 
  and operate offline more efficiently.</li>
  <li><b>Multimedia</b>: making video and audio first-class citizens in the Open Web.</li>
  <li><b>2D/3D graphics and effects</b>: allowing a much more diverse range of presentation options.</li>
  <li><b>Performance and integration</b>: providing greater speed optimization and better usage 
  of computer hardware.</li>
  <li><b>Device access</b>: allowing for the usage of various input and output devices.</li>
  <li><b>Styling</b>: letting authors write more sophisticated themes.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are the semantic tags available in html5?</h3>

HTML5 semantic tags define the function and the category of your text, simplifying the 
work for browsers and search engines, as well as developers.

HTML5 offers new semantic elements to define different parts of a web page:

<ul>
  <li>`&lt;article&gt;`</li>
  <li>`&lt;aside&gt;`</li>
  <li>`&lt;details&gt;`</li>
  <li>`&lt;figcaption&gt;`</li>
  <li>`&lt;figure&gt;`</li>
  <li>`&lt;footer&gt;`</li>
  <li>`&lt;header&gt;`</li>
  <li>`&lt;main&gt;`</li>
  <li>`&lt;mark&gt;`</li>
  <li>`&lt;nav&gt;`</li>
  <li>`&lt;section&gt;`</li>
  <li>`&lt;summary&gt;`</li>
  <li>`&lt;time&gt;`</li>
</ul>

<h5>Syntax:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html> 

<html>  
   <head> 
      <meta charset = "utf-8"/> 
      <title>...</title> 
   </head> 
  
   <body> 
      <header>...</header> 
      <nav>...</nav> 
      
      <article> 
         <section> 
            ... 
         </section> 
      </article> 
      <aside>...</aside> 
      
      <footer>...</footer> 
   </body> 
</html> 
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Why you would like to use semantic tags?</h3>

<ul>
  <li>Search Engine Optimization, accessibility, repurposing, light code.</li>
  <li>Many visually impaired person rely on browser speech and semantic tag helps to 
    interpret page content clearly.</li>
  <li>Search engine needs to understand page content to rank and semantic tag helps.</li>
  <li>Semantic code aids accessibility. Specially, many people whose eyes are not good rely 
    on speech browsers to read pages to them. These programs cannot interpret pages very 
    well unless they are clearly explained.</li>
  <li>Help Search engines to better understand pages. Search engine need to understand what 
    your content is about when rank you properly on search engines. Semantic code tends to 
    improve your placement on search engines, as it is easier for the "search engine spiders" 
    to understand.</li>
  <li>It's easier to read and edit, which saves time and money during maintenance.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What does a `&lt;DOCTYPE html&gt;` do?</h3>

<p>A DOCTYPE is always associated to a `DTD` ( <b>Document Type Definition</b> ). A DTD defines 
how documents of a certain type should be structured (i.e. a `button` can contain a `span` 
but not a `div`), whereas a DOCTYPE declares what DTD a document supposedly respects (i.e. 
this document respects the HTML DTD). For webpages, the DOCTYPE declaration is required. 
It is used to tell user agents what version of the HTML specifications your document respects.</p>

<p>Once a user agent has recognized a correct DOCTYPE, it will trigger the `no-quirks mode` 
matching this DOCTYPE forreading the document. If a user agent doesn't recognize a correct 
DOCTYPE, it will trigger the `quirks mode`.</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What happens when DOCTYPE is not given?</h3>

<p>The web page is rendered in quirks mode. The web browsers engines use quirks mode to 
support older browsers which does not follow the <b>W3C specifications</b>. In quirks mode 
CSS class and id names are case insensitive. In standards mode they are case sensitive.</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are the new form elements in HTML5?</h3>

<p>There are five new form elements in the HTML5 forms specification: `&lt;datalist&gt;`, `&lt;keygen&gt;`, `&lt;output&gt;`, 
`&lt;progress&gt;`, and `&lt;meter&gt;`.</p>

<h4>1. Datalist Tag</h4>

<p>Allows to attach a list of suggestions to a text input element. As soon as the user begins 
to type in the text field, the list of suggestions appears and the user can choose from 
the suggestions with the mouse.</p>

<details>
  <summary>html</summary>

```html
<p>Enter your favorite browser name:</p>
<input type="text" list="browsers" name="favorite_browser">
<datalist id="browsers">
  <option value="Firefox">
  <option value="Chrome">    
  <option value="Internet Explorer">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

</details>

<h4>2. Meter Tag</h4>

<p>Indicates a numeric value that falls within a range. The tag supports a number of attributes:
value: If you don't specify a value, the first numeric value inside the `<meter></meter>` 
pair becomes the value.</p>

<ul>
  <li><b>max</b>: The maximum possible value of the item.</li>
  <li><b>min</b>: The minimum possible value of the item.</li>
  <li><b>high</b>: If the value can be defined as a range, this is the high end of the range.</li>
  <li><b>low</b>: If the value can defined as a range, this is the low end of that range.</li>
  <li><b>optimum</b>: The optimal value of the element.</li>
</ul>

```html
<p>Disk Usage: <meter value="0.2">20%</meter></p>
<p>Total Score: <meter value="6" min="0" max="10">6 out of 10</meter></p>
<p>Pollution Level: <meter low="60" high="80" max="100" value="85">Very High</meter></p>
```

<h4>3. Output Tag</h4>

<p>It indicates a section of the page that can be modified by a script (usually JavaScript).</p>

```html
<form oninput="result.value=parseInt(a.value)+parseInt(b.value)">
  <input type="range" id="a" value="50"> +
  <input type="number" id="b" value="100"> =
  <output name="result" for="a b"></output>
</form>
```

<h4>4. Progress Tag</h4>

<p>Indicates how much of a task has been completed (often marked as a percentage). It is 
expected to be modified through JavaScript code.</p>

<details>
  <summary>html</summary>

```html
<p>Progress: <progress id="bar" value="0" max="100"><span>0</span>%</progress></p>

<script type="text/javascript">
  var i = 0;
  var progressBar = document.getElementById("bar");
    
  function countNumbers() {
    if(i < 100) {
      i = i + 1;
      progressBar.value = i;
      // For browsers that don't support progress tag
      progressBar.getElementsByTagName("span")[0].textContent = i;
    }

    // Wait for sometime before running this script again
    setTimeout("countNumbers()", 100);
  }
  countNumbers();
</script>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3 id="new-form-elements">List New form elements introduced in html5</h3>

|Sl.No| Element       | Description   |
|-----|---------------|---------------------------|
| 01. |color          |Gives the end user a native color picker to choose a color.|
| 02. |date           |Offers a datepicker.|
| 03. |datetime       |An element to choose both date and time.|
| 04. |datetime-local |An element to choose both date and time, with local settings support.|
| 05. |email          |A field for entering e-mail address(es).|
| 06. |month          |Choose a full month.|
| 07. |number         |Picking a number.|
| 08. |range          |Offers a slider to set to a certain value/position.|
| 09. |search         |A field for search queries.|
| 10. |tel            |Choosing a telephone number.|
| 11. |time           |Input a certain time.|
| 12. |url            |Entering a URL.|
| 13. |week           |Picking a specific week.|


<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<input type="color" value="#b97a57">
<input type="date" value="2020-06-08">
<input type="datetime" value="2020-06-09T20:35:34.32">
<input type="datetime-local" value="2020-06-09T22:41">
<input type="email" value="robert@robertnyman.com">
<input type="month" value="2020-06">
<input type="number" value="4">
<input type="range" value="15">

<!-- Note: If not set, default attribute values are min="0", max="100", step="1". -->
<input type="search" value="[Any search text]">
<input type="tel" value="[Any numeric value]">

<!-- Note: Most web browsers seem to let through any value at this time. -->
<input type="time" value="22:38">
<input type="url" value="https://www.google.com/">

<!-- Note: requires a protocol like http://, ftp:// etc in the beginning. -->
<input type="week" value="2020-W24">
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h4>Example to create a HTML form with below constraints</h4>

<ul>
  <li>Accept User Name, Email, Country and Subject,</li>
  <li>Validate the fields,</li>
  <li>Store data into local Storage,</li>
  <li>Fetch user data and display on right side of the page.</li>
</ul>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  body {font-family: Arial, Helvetica, sans-serif;}
  * {box-sizing: border-box;}
  
  input[type=text], input[type=email], select, textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    margin-top: 6px;
    margin-bottom: 16px;
    resize: vertical;
  }
  
  input[type=submit] {
    background-color: #0e8af7;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  
  input[type=submit]:hover {
    background-color: #1181e3;
  }
  
  .container {
    border-radius: 5px;
    background-color: #f2f2f2;
    padding: 20px;
  }
</style>
</head>
<body>

<h3>Contact Form</h3>

<div class="container">
  <form name="contactForm" onsubmit="return validateForm()" method="post">
    <label for="fname">Name</label>
    <input type="text" id="user_name" name="user_name" placeholder="Your name.." required>

    <label for="lname">Email ID</label>
    <input type="email" id="email" name="email" placeholder="Your Email Address.." required>

    <label for="country">Country</label>
    <select id="country" name="country" required>
      <option value="">--- SELECT ---</option>
      <option value="australia">Australia</option>
      <option value="canada">Canada</option>
      <option value="india">India</option>
      <option value="usa">USA</option>
    </select>

    <label for="subject">Subject</label>
    <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>

    <input type="submit" value="Submit">
  </form>
</div>
<script>
  function validateForm() {
    let name = document.forms["contactForm"]["user_name"].value;
    let email = document.forms["contactForm"]["email"].value;
    let country = document.forms["contactForm"]["country"].value;
    let subject = document.forms["contactForm"]["subject"].value;

    if (name === "" || email === "" || country === "") {
      alert("All the fields are mandatory");
      return false;
    } else { 
      // Create a JSON Object
      const userData = {
        name: name,
        email: email,
        country: country,
        subject: subject
      };

      // Store the object into storage
      localStorage.setItem("userData", JSON.stringify(userData));

      // Retrieve the object from the storage
      const data = localStorage.getItem("userData");
      console.log("data: ", JSON.parse(data));
        
      return false;
    }
  }
</script>
</body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3 id="diff-span-div">What is the difference between `span` tag and `div` tag?</h3>

<p>The primary difference between div and span tag is their default behavior. By default, 
a `&lt;div&gt;` is a <b>block-level-element</b> and a `&lt;span&gt;` is an <b>inline element</b>.</p>

<ul>
  <li>`&lt;div&gt;` is a block level element which means it will render it on 
    it&apos;s own line with a width of a 100% of the parent element.</li>
  <li>`&lt;span&gt;` is an inline element which means it will render on the same 
    line as the previous element, if it is also an inline element, and it's width 
    will be determined by it's content.</li>
</ul>

```html
<div>Demo Text, with <span>some other</span> text.</div>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are optional closing tags?</h3>

<p>`&lt;p&gt;`, `&lt;li&gt;`, `&lt;td&gt;`, `&lt;tr&gt;`, `&lt;th&gt;`, `&lt;html&gt;`, 
`&lt;body&gt;`, etc. don't have to provide an end tag. Whenever a browser hits a new tag 
it automatically ends the previous tag.</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is a self closing tag?</h3>

<p>In HTML5 it is not strictly necessary to close certain HTML tags. The tags that aren't 
required to have specific closing tags are called “self closing” tags.</p>

<p>An example of a self closing tag is something like a line break (`&lt;br /&gt;`) or the meta 
tag (`&lt;meta&gt;`). This means that the following are both acceptable:</p>

```html
<meta charset="UTF-8">
...
<meta charset="UTF-8" />
```

<h3>Q. Explain the difference between block elements and inline elements?</h3>

<p>Inline elements are typically used to define small pieces of content such as text or 
images that are integrated into a larger block of text. Block elements are typically 
used to define larger blocks of content such as paragraphs, headings, and lists. Take 
up only as much width as necessary to display their content.</p>

<ul>
  <li>block elements: `&lt;h1&gt;`, `&lt;p&gt;`, `&lt;ul&gt;`, `&lt;ol&gt;`, `&lt;li&gt;`</li>
  <li>inline elements: `&lt;span&gt;`, `&lt;a&gt;`, `&lt;strong&gt;`, `&lt;i&gt;`, `&lt;img&gt;`</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are semantic and non-semantic elements?</h3>

<ul>
  <li><b>Semantic elements</b>: clearly describes its meaning to both the browser and the developer.
    For example: `&lt;form&gt;`, `&lt;table&gt;`,  `&lt;article&gt;`, `&lt;aside&gt;`, `&lt;details&gt;`, `&lt;figcaption&gt;`, 
	`&lt;figure&gt;`, `&lt;footer&gt;`, `&lt;header&gt;`, `&lt;main&gt;`, `&lt;mark&gt;`, `&lt;nav&gt;`, `&lt;section&gt;`, `&lt;summary&gt;`, 
	`&lt;time&gt;` clearly defines its content.</li>
  <li><b>Non-semantic elements</b>: `&lt;div&gt;` and `&lt;span&gt;` tells nothing about its content.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the purpose of `main` element?</h3>

<p>The HTML `&lt;main&gt;` element represents the dominant content of the `&lt;body&gt;` 
of a document. The main content area consists of content that is directly related to or 
expands upon the central topic of a document, or the central functionality of an 
application.</p>

```html
<main role="main">
  <p>Geckos are a group of usually small, usually nocturnal lizards. 
  They are found on every continent except Australia.</p>
  <p>Many species of gecko have adhesive toe pads which enable them to climb walls 
    and even windows.</p>
</main>
```

<p><i>Note: A document mustn't have more than one `&lt;main&gt;` element that doesn't 
have the hidden attribute specified.</i></p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are the semantic meanings for &lt;section&gt;, &lt;article&gt;, &lt;aside&gt;, 
&lt;nav&gt;, &lt;header&gt;, &lt;footer&gt; and how should each be used in structuring html markup?</h3>

<ul>
  <li><b>`&lt;header&gt;`</b> is used to contain introductory and navigational information about a section 
    of the page. This can include the section heading, the author's name, time and date of 
	publication, table of contents, or other navigational information.</li>
  <li><b>`&lt;article&gt;`</b> is meant to house a self-contained composition that can logically be 
    independently recreated outside of the page without losing it's meaining. Individual 
	blog posts or news stories are good examples.</li>
  <li><b>`&lt;section&gt;`</b> is a flexible container for holding content that shares a common informational 
    theme or purpose.</li>
  <li><b>`&lt;footer&gt;`</b> is used to hold information that should appear at the end of a section of content 
    and contain additional information about the section. Author's name, copyright information, 
	and related links are typical examples of such content.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. When should you use `section`, `div` or `article`?</h3>

<ul>
  <li>`&lt;section&gt;`, group of content inside is related to a single theme, and should appear 
    as an entry in an outline of the page. It's a chunk of related content, like a subsection 
	of a long article, a major part of the page (eg the news section on the homepage), or a 
	page in a webapp's tabbed interface. A section normally has a heading (title) and maybe 
	a footer too.</li>
  <li>`&lt;article&gt;`, represents a complete, or self-contained, composition in a document, page, 
    application, or site and that is, in principle, independently distributable or reusable, 
	e.g. in syndication. This could be a forum post, a magazine or newspaper article, a blog 
	entry, a user-submitted comment, an interactive widget or gadget, or any other independent 
	item of content.</li>
  <li>`&lt;div&gt;`, on the other hand, does not convey any meaning, aside from any found in its class, 
    lang and title attributes.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Can a web page contain multiple `&lt;header&gt;` elements? What about `&lt;footer&gt;` elements?</h3>

<p>Yes, header elements can be used multiple times in documents. A `&lt;header&gt;` tag must be present 
for all articles, sections, and pages, although a `&lt;footer&gt;` tag is not necessary.</p>

<h4>From W3C standards</h4>

```html
A header element is intended to usually contain the section's heading (an h1–h6 element or an hgroup 
element), but this is not required. The header element can also be used to wrap a section's table of 
contents, a search form, or any relevant logos.
```

```html
The footer element represents a footer for its nearest ancestor sectioning content or 
sectioning root element. A footer typically contains information about its section such 
as who wrote it, links to related documents, copyright data, and the like.
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are the physical tags and logical tags in HTML?</h3>

<h4>1. Physical Tags:</h4>

<p>Physical tags are used to indicate how a particular character is to be formatted. Any 
physical style tag may contain any item allowed in text, including conventional text, 
images, line breaks, etc.</p>

<h5>Example:</h5>

|Tags      | Description                                                      |
|----------|------------------------------------------------------------------|
|`<sup>`   |Superscript is usually used for showing elements above base-line |
|`<sub>`   |The subscript is used for alternate baseline.|
|`<i>`     |An Italic tag is used to define a text with a special meaning. |
|`<big>`   |Big tag increase the font size by 1 (Note: You can not use the big tag in HTML 5)|
|`<small>` |A small tag defines the small text, and it is used while writing copyright.|
|`<b>`     |Bold increases the importance of the text because bold tag covert the text into bold size.|
|`<u>`     |It is used to underline the text.|
|`<tt>`    |Teletype text gives the default font-family which is monospace.|
|`<strike>`|It is an editing markup that tells the reader to ignore the text passage.|

<h4>2. Logical Tags:</h4>

<p>Logical tags are used to tell the browser what kind of text is written inside the tags. 
Logical tags are also known as Structural tags because they specify the structure of the 
document. Logical tags are used to indicate to the visually impaired person that there 
is something more important in the text or to emphasize the text ie, logical tags can be 
used for styling purposes as well as to give special importance to text content.</p>

<h5>Example:</h5>

|Tags       | Description                     |
|-----------|---------------------------------|
|`<abbr>`   |Defines the abbreviation of text.|
|`<acronym>`|Defines the acronym.|
|`<address>`|Contact information of a person or an organization.|
|`<cite>`   |Defines citation. It displays the text in italic format.|
|`<code>`   |Defines the piece of computer code.|
|`<blockquote>`|Defines a long quotation.|
|`<del>`    |Defines the deleted text and is used to mark a portion of text which has been deleted from the document.|
|`<dfn>`    |Defines the definition element and is used to representing a defining instance in HTML.|
|`<ins>`    |Defines inserted text.|
|`<kbd>`    |Defines keyboard input text.|
|`<pre>`    |Defines the block of preformatted text which preserves the text spaces, line breaks, tabs, and other formatting characters which are ignored by web browsers.|
|`<q>`      |Defines the short quotation.|
|`<samp>`   |Defines the sample output text from a computer program.|
|`<strong>` |Defines strong text i.e. show the importance of the text.|
|`<var>`    |Defines the variable in a mathematical equation or in the computer program.|

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is Character Encoding?</h3>

<p>Character encoding is a method of converting bytes into characters. To validate or display 
an HTML document properly, a program must choose a proper character encoding. This is 
specified in the tag:</p>

```html
<meta charset="utf-8"/>
```

<ul>
  <li><b>UTF-8</b>: A Unicode Translation Format that comes in 8-bit units that is, it comes in 
    bytes. A character in UTF8 can be from 1 to 4 bytes long, making UTF8 variable width.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the purpose of meta tags?</h3>

<p>Meta tags are pieces of information you use to tell the search engines and those 
viewing your site more about your page and the information it contains. Meta tags include: 
Title tags: the title of your page, which should be unique for every page you publish. 
Meta description: a description of the content on the page.</p>

<p>The META elements can be used to include name/value pairs describing properties of the 
HTML document, such as author, expiry date, a list of keywords, document author etc.</p>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
  <head>
    <!--Recommended Meta Tags-->
    <meta charset="utf-8">
    <meta name="language" content="english"> 
    <meta http-equiv="content-type" content="text/html">
    <meta name="author" content="Author Name">
    <meta name="designer" content="Designer Name">
    <meta name="publisher" content="Publisher Name">
    <meta name="no-email-collection" content="name@email.com">
    <meta http-equiv="X-UA-Compatible" content="IE=edge"/>

    <!--Search Engine Optimization Meta Tags-->
    <meta name="description" content="Project Description">
    <meta name="keywords" content="Software Engineer,Product Manager,Project Manager,Data Scientist">
    <meta name="robots" content="index,follow">
    <meta name="revisit-after" content="7 days">
    <meta name="distribution" content="web">
    <meta name="robots" content="noodp">
        
    <!--Optional Meta Tags-->
    <meta name="distribution" content="web">
    <meta name="web_author" content="">
    <meta name="rating" content="">
    <meta name="subject" content="Personal">
    <meta name="title" content=" - Official Website.">
    <meta name="copyright" content="Copyright 2020">
    <meta name="reply-to" content="">
    <meta name="abstract" content="">
    <meta name="city" content="Bangalore">
    <meta name="country" content="INDIA">
    <meta name="distribution" content="">
    <meta name="classification" content="">
    
    <!--Meta Tags for HTML pages on Mobile-->
    <meta name="format-detection" content="telephone=yes"/>
    <meta name="HandheldFriendly" content="true"/> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/> 
    <meta name="apple-mobile-web-app-capable" content="yes" />
        
    <!--http-equiv Tags-->
    <meta http-equiv="Content-Style-Type" content="text/css">
    <meta http-equiv="Content-Script-Type" content="text/javascript">
      
    <title>HTML5 Meta Tags</title>
  </head>
  <body>
    ...
  </body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What does async and defer refer in script tag?</h3>

<p>Scripts with an <mark>async</mark> attribute will execute as soon as the download is 
complete. This blocks the page and does not guarantee any specific execution order. 
Scripts with a <mark>defer</mark> attribute will load in the order they are in and 
will only execute once everything has finished loading.</p>

<h4>1. Async:</h4>

<p>Downloads the script file during HTML parsing and will pause the HTML parser to execute 
it when it has finished downloading.</p>

<h5>Example:</h5>

```html
<!-- 
  With async (asynchronous), browser will continue to load the HTML 
  page and render it while the browser load and execute the script at the same time. 
-->
<!-- Google Analytics is usually added like this -->
<script async src="https://google-analytics.com/analytics.js"></script>
```

<h4>2. Defer:</h4>

Defer downloads the script file during HTML parsing and will only execute it after the 
HTML parser has completed. Not all browsers support this.

<h5>Example:</h5>

```html
<!-- 
  With defer, browser will run your script when the page finished parsing. 
  (not necessary finishing downloading all image files. This is good.) 
-->
<script defer src="myscript.js"></script>
```

<p>The async attribute is used to indicate to the browser that the script file can be executed 
asynchronously. The HTML parser does not need to pause at the point it reaches the script 
tag to fetch and execute, the execution can happen whenever the script becomes ready after 
being fetched in parallel with the document parsing.</p>

<p>The defer attribute tells the browser to only execute the script file once the HTML document 
has been fully parsed.</p>

<h5>Example:</h5>

```html
<!-- 
  Without async or defer, browser will run your script immediately, 
  before rendering the elements. 
-->
<script src="myscript.js"></script>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is local storage in html5?</h3>

The <b>localStorage</b> read-only property of the window interface allows you to access a 
Storage object for the Document's origin; the stored data is saved across browser sessions.

<h5>Example:</h5>

```js
// Store
localStorage.setItem("name", "Kanti Ahluwalia");

// Retrieve
localStorage.getItem("name"); // Kanti Ahluwalia
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is session storage in html5?</h3>

<p>The <b>sessionStorage</b> object is equal to the localStorage object, except that it stores 
the data for only one session. The data is deleted when the user closes the specific browser tab.</p>

<h5>Example:</h5>

```js
// Save data to sessionStorage
sessionStorage.setItem('key', 'value');

// Get saved data from sessionStorage
let data = sessionStorage.getItem('key');

// Remove saved data from sessionStorage
sessionStorage.removeItem('key');

// Remove all saved data from sessionStorage
sessionStorage.clear();
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is cookies in html5?</h3>

<p>A cookie is an amount of information that persists between a server-side and a client-side. 
A web browser stores this information at the time of browsing.</p>

<p>A cookie contains the information as a string generally in the form of a name-value pair 
separated by semi-colons. It maintains the state of a user and remembers the user's 
information among all the web pages.</p>

<h5>Example 01: Create a Cookies</h5>

```js
// create a cookie
document.cookie = "username=Anjali Batta";

// cookie with expiry date
document.cookie = "username=Anjali Batta; expires=Thu, 18 Dec 2022 12:00:00 UTC";
```

<h5>Example 02: Cookie with expiry date</h5>

```js
// cookie with expiry date
document.cookie = "username=Anjali Batta; expires=Thu, 18 Dec 2022 12:00:00 UTC";
```

<h5>Example 03: Read Cookie</h5>

```js
let myCookies = document.cookie;

console.log(myCookies);
```

<h5>Example 04: Update Cookie</h5>

```js
document.cookie = "username=John Smith; expires=Thu, 18 Dec 2022 12:00:00 UTC; path=/";
```

<h5>Example 05: Delete Cookie</h5>

```js
document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;";
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Describe the difference between a cookie, sessionStorage and localStorage?</h3>

|                                        | `cookie`                                                 | `localStorage` | `sessionStorage` |
|----------------------------------------|----------------------------------------------------------|------------|------------------|
| Initiator                              | Client or server. Server can use `Set-Cookie` header     | Client     | Client           |
| Expiry                                 | Manually set                                             | Forever    | On tab close     |
| Persistent across browser sessions     | Depends on whether expiration is set                     | Yes        | No               |
| Sent to server with every HTTP request | Cookies are automatically being sent via `Cookie` header | No         | No               |
| Capacity (per domain)                  | 4kb                                                      | 5MB        | 5MB              |
| Accessibility                          | Any window                                               | Any window | Same tab         |

<p><i>Note: If the user decides to clear browsing data via whatever mechanism provided by 
the browser, this will clear out any `cookie`, `localStorage`, or `sessionStorage` stored. 
It's important to keep this in mind when designing for local persistance, especially when 
comparing to alternatives such as server side storing in a database or similar (which of 
course will persist despite user actions).</i></p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Does localStorage throw error after reaching maximum limits?</h3>

<p>Yes</p>

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE HTML>
<html>
  <head>
    <title>HTML5 localStorage</title>
  </head>
  <body>
    <script type="text/javascript">
      try {
        if(window.localStorage){ // Check if the localStorage object exists
          var result = "";
          var characters  = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
          var charactersLength = characters.length;
          for(var i = 0; i < 10000; i++){
            result += characters.charAt(Math.floor(Math.random() * charactersLength));
            localStorage.setItem("key"+i, result);
          }  
        } else {
          alert("Sorry, your browser do not support localStorage.");
        }
      } catch(e) {
        console.log('Exception: '+e);
      }
    </script>
  </body>
</html>
```

</details>

<h5>Output</h5>

```js
Exception: QuotaExceededError: Failed to execute 'setItem' on 'Storage': 
           Setting the value of 'key3230' exceeded the quota.
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Why use IndexedDB instead of WebSQL in HTML5?</h3>

<h4>1. WebSQL</h4>

<p>It is an API that is only supported in Chrome and Safari (and Android and iOS by extension). 
It provides an asynchronous, transactional interface to SQLite. Since 2010, it has been 
deprecated in favor of IndexedDB.</p>

<h5>Advantages</h5>

<ul>
  <li>Supported on major mobile browsers (Android Browser, Mobile Safari, Opera Mobile) 
    as well as several desktop browsers (Chrome, Safari, Opera).</li>
  <li>Good performance generally, being an asynchronous API. Database interaction won't 
    lock up the user interface. (Synchronous API is also available for WebWorkers.)</li>
  <li>Good search performance, since data can be indexed according to search keys.</li>
  <li>Robust, since it supports a transactional database model.</li>
  <li>Easier to maintain integrity of data, due to rigid data structure.</li>
</ul>

<h5>Disadvantages</h5>

<ul>
  <li>Deprecated. Will not be supported on IE or Firefox, and will probably be phased out 
    from the other browsers at some stage.</li>
  <li>Steep learning curve, requiring knowledge of relational databases and SQL.</li>
  <li>Suffers from object-relational impedance mismatch.
  <li>Diminishes agility, as database schema must be defined upfront, with all records in a 
    table matching the same structure.</li>
</ul>

<h4>2. IndexedDB</h4>

It is the successor to both LocalStorage and WebSQL, designed to replace them as the 
“one true” browser database. It exposes an asynchronous API that supposedly avoids 
blocking the DOM, but as we'll see below, it doesn't necessarily live up to the hype. 
Browser support is extremely spotty, with only Chrome and Firefox having fully usable 
implementations.

<h5>Advantages</h5>

<ul>
  <li>Good performance generally, being an asynchronous API. Database interaction won't 
    lock up the user interface. (Synchronous API is also available for WebWorkers.)</li>
  <li>Good search performance, since data can be indexed according to search keys.</li>
  <li>Supports versioning.</li>
  <li>Robust, since it supports a transactional database model.</li>
  <li>Fairly easy learning curve, due to a simple data model.</li>
  <li>Decent browser support: Chrome, Firefox, mobile FF, IE10.</li>
</ul>

<h5>Disadvantages</h5>

<ul>
  <li>Very complex API resulting in large amounts of nested callbacks.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain Application Cache in HTML5. OR What is a manifest file in HTML?</h3>

<p>HTML5 provides an application caching mechanism that lets web-based applications run offline. 
Developers can use the Application Cache (AppCache) interface to specify resources that the 
browser should cache and make available to offline users. Applications that are cached load 
and work correctly even if users click the refresh button when they are offline.</p>

<h4>Using an application cache gives an application the following benefits:</h4>

<ul>
  <li><b>Offline browsing</b>: users can navigate a site even when they are offline.</li>
  <li><b>Speed</b>: cached resources are local, and therefore load faster.</li>
  <li><b>Reduced server load</b>: the browser only downloads resources that have changed 
    from the server.</li>
</ul>

<h5>Syntax:</h5>

```html
<html manifest="example.appcache">
  ...
</html>
```

<p><i>Note: Using the application caching feature described here is at this point highly 
discouraged; it's in the process of being removed from the Web platform. Use <b>Service 
Workers</b> instead. In fact as of Firefox 44, when AppCache is used to provide offline 
support for a page a warning message is now displayed in the console advising developers 
to use Service workers instead (bug 1204581).</i></p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the purpose of cache busting and how can you achieve it?</h3>

<p>Browsers have a cache to temporarily store files on websites so they don't need to be 
re-downloaded again when switching between pages or reloading the same page. The server 
is set up to send headers that tell the browser to store the file for a given amount of 
time. This greatly increases website speed and preserves bandwidth.</p>

<p>However, it can cause problems when the website has been changed by developers because 
the user's cache still references old files. This can either leave them with old 
functionality or break a website if the cached CSS and JavaScript files are referencing 
elements that no longer exist, have moved or have been renamed.</p>

<p><b>Cache busting</b> is the process of forcing the browser to download the new files. This 
is done by naming the file something different from the old file.</p>

<p>A common technique to force the browser to re-download the file is to append a query 
string to the end of the file.</p>

```html
<!-- src="js/script.js" => src="js/script.js?v=2" -->
<script src="js/script.js?v=2"></script>
```

<p>The browser considers it a different file but prevents the need to change the file name.</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What ARIA and screenreaders are, and how to make a website accessible?</h3>

Screen readers are software programs that  provide assistive technologies that allow 
people with disabilities (such as no sight, sound or mouse-ing ability) to use web 
applications. You can make your sites more accessible by following ARIA standards 
such as semantic HTML, alt attributes and using [role=button] in the expected ways.

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How to use data- attribute in html5?</h3>

Any attribute on any element whose attribute name starts with <b>data-</b> is a data attribute. 
The data-&ast; attributes gives us the ability to embed custom data attributes on all HTML 
elements. The stored (custom) data can then be used in the page's JavaScript to create 
a more engaging user experience.

<b>Example:</b>

```html
<article
  id="electric-cars"
  data-columns="10"
  data-index-number="100"
  data-parent="cars"
>
  <h1>Electric Cars</h1>
</article>
```

```js
/**
 * Access data attribute
**/
const article = document.getElementById("electric-cars");

article.dataset.columns; // "10"
article.dataset.indexNumber; // "100"
article.dataset.parent; // "cars"
```

<p><b>&#9885; <a href="https://codesandbox.io/s/html-data-attribute-llxlkn?file=/script.js">
Try this example on CodeSandbox</a></b></p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the purpose of the <mark>alt</mark> attribute on images?</h3>

<p>The <mark>alt</marK attribute provides alternative information for an image if a user 
cannot view it. The <mark>alt</mark> attribute should be used to describe any images 
except those which only serve a decorative purposes, in which case it should be left 
empty.</p>

<pre>
&lt;img src="pancakes.png" alt="Stack of blueberry pancakes with powdered sugar"&gt;
</pre>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What does `enctype='multipart/form-data'` mean?</h3>

The enctype attribute specifies how the form-data should be encoded when submitting it to the server.

<b>Example: 01</b>

```html
<form action="fileupload.php" method="post" enctype="multipart/form-data"> 
  <p>Please select the file you would like to upload.</p> 
  <input type="file" name="upload"> 
  <br> 
  <input type="submit" value="Upload File">
</form>
```

<b>Example: 02</b>

```html
<form action="/urlencoded?token=A87412B" method="POST" enctype="application/x-www-form-urlencoded">
  <input type="text" name="username" value=""/>
  <input type="text" name="password" value=""/>
  <input type="submit" value="Submit" />
</form>
```

<b>Example: 03</b>

```html
<form action="action.do" method="get" enctype="text/plain">
    Name: <input type="text" name="name" />
    Phone: <input type="number" name="phone" />
    <input type="submit" value="Submit" />
</form>
```

|Sl.No|Value                              |Description                        |
|-----|-----------------------------------|-----------------------------------|
| 01. |application/x-www-form-urlencoded  |Default. All characters are encoded before sent (spaces are converted to "+" symbols, and special characters are converted to ASCII HEX values)|
| 02. |multipart/form-data        |No characters are encoded. This value is required when you are using forms that have a file upload control |
| 03. |text/plain                |Spaces are converted to "+" symbols, but no special characters are encoded|

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the difference between Select and Datalist?</h3>

<p>For the select element, the user is required to select one of the options you've given. 
For the datalist element, it is suggested that the user select one of the options you've 
given, but he can actually enter anything he wants in the input.</p>

<h4><b>1. Select:</b></h4>

<pre>
&lt;select name="browser"&gt;
  &lt;option value="firefox"&gt;Firefox&lt;/option&gt;
  &lt;option value="ie"&gt;IE&lt;/option&gt;
  &lt;option value="chrome"&gt;Chrome&lt;/option&gt;
  &lt;option value="opera"&gt;Opera&lt;/option&gt;
  &lt;option value="safari"&gt;Safari&lt;/option&gt;
&lt;/select&gt;
</pre>

<h4><b>2. Datalist:</b></h4>

```html
<input type="text" list="browsers">
<datalist id="browsers">
  <option value="Firefox">
  <option value="IE">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain some of the pros and cons for CSS animations versus JavaScript animations?</h3>

<p>Regarding optimization and responsiveness the debate bounces back and forth but, the concept is:</p>

<ul>
  <li>CSS animations allows the browser to choose where the animation processing is done, 
    CPU or the GPU. (Central or Graphics Processing Unit)</li>
  <li>That said, adding many layers to a document will eventually have a performance hit.</li>
  <li>JS animation means more code for the user to download and for the developer to maintain.</li>
  <li>Applying multiple animation types on an element is harder with CSS since all transforming 
    power is in one property transform.</li>
  <li>CSS animations being declarative are not programmable therefore limited in capability.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What does CORS stand for and what issue does it address?</h3>

<p>Cross-Origin Resource Sharing (CORS) is a W3C spec that allows cross-domain communication 
from the browser. By building on top of the XMLHttpRequest object, CORS allows developers 
to work with the same idioms as same-domain requests. CORS gives web servers cross-domain 
access controls, which enable secure cross-domain data transfers.</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Can you describe the difference between progressive enhancement and graceful degradation?</h3>

<ul>
  <li>Graceful degradation is when you initially serve the best possible user experience, 
    with all modern functionality, but use feature detection to “gracefully degrade” parts 
	of your application with a fallback or polyfill.</li>
  <li>Progressive enhancement ensures a page works at the lowest expected abilities of 
    browsers. So if you have a JavaScript web application that enhances a persons ability 
	to send information to a database with features like ajax – at the very least you need 
	to provide the ability for a person to send that same information without JavaScript 
	enabled. In this case a simple form with full-page refresh will do what you need.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the DOM? How does the DOM work?</h3>

<p>The DOM (Document Object Model) is a cross-platform API that treats HTML documents as a 
tree structure consisting of nodes. These nodes (such as elements and text nodes) are 
objects that can be programmatically manipulated and any visible changes made to them 
are reflected live in the document. In a browser, this API is available to JavaScript 
where DOM nodes can be manipulated to change their styles, contents, placement in the 
document, or interacted with through event listeners.</p>

<ul>
  <li>The DOM was designed to be independent of any particular programming language, making 
    the structural representation of the document available from a single, consistent API.</li>
  <li>document.getElementById() and document.querySelector() are common functions for selecting 
    DOM nodes.</li>
  <li>Setting the innerHTML property to a new value runs the string through the HTML parser, 
    offering an easy way to append dynamic HTML content to a node.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How does the browser rendering engine work?</h3>

<p>In order to render content the browser has to go through a series of steps:</p>

<ul>
  <li>Document Object Model(DOM)</li>
  <li>CSS object model(CSSOM)</li>
  <li>Render Tree</li>
  <li>Layout</li>
  <li>Paint</li>
</ul>

<p align="center">
  <img src="assets/images/layers.png" alt="Browser Rendering Engine" />
</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the difference between standards mode and quirks mode?</h3>

In <b>Quirks mode</b>, layout emulates nonstandard behavior in Navigator 4 and Internet 
Explorer 5. This is essential in order to support websites that were built before the 
widespread adoption of web standards. In <b>Standards mode</b>, the behavior is described 
by the HTML and CSS specifications. 

For HTML documents, browsers use a `<!DOCTYPE html>` in the beginning of the document to 
decide whether to handle it in quirks mode or standards mode. 

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset=UTF-8>
    <title>Hello World!</title>
  </head>
  <body>
  </body>
</html>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is Critical Rendering Path?</h3>

<ul>
  <li>Constructing the DOM Tree</li>
  <li>Constructing the CSSOM Tree</li>
  <li>Running JavaScript - parser blocking resource</li>
  <li>Creating the Render Tree</li>
  <li>Generating the Layout</li>
  <li>Painting</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are the Benefits of Server Side Rendering (SSR) Over Client Side Rendering (CSR)?</h3>

<ul>
  <li>We are using server side rendering for two reasons:
    <ul>
	  <li>Performance benefit for our customers</li>
	  <li>Consistent SEO performance</li>
	</ul>
  </li>
</ul>

<ul>
  <li>The main difference is that for SSR your server's response to the browser is the HTML 
    of your page that is ready to be rendered, while for CSR the browser gets a pretty empty 
	document with links to your javascript. That means for SSR your browser will start rendering 
	the HTML from your server without having to wait for all the JavaScript to be downloaded 
	and executed.</li>
  <li>for SSR, the user can start viewing the page while all of that is happening. For the 
    CSR world, you need to wait for all of the above to happen and then have the virtual dom 
	moved to the browser dom for the page to be viewable.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Name 3 ways to decrease page load?</h3>

<ol start="1">
  <li>Optimize images</li>
  <li>Enable browser caching</li>
  <li>Reduce Redirects</li>
  <li>Asynchronous loading</li>
  <li>Enable compression</li>
  <li>Implement lazy loading</li>
  <li>Make JavaScript files minified</li>
  <li>Try <a href="https://www.webpagetest.org/">Webpage Test</a></li>
  <li>Try <a href="https://tools.pingdom.com/">Pingdom</a></li>
</ol>

<h4>Others</h4>

<ol start="10">
  <li>LocalStorage</li>
  <li>Caching resources</li>
  <li>DNS-prefetch (sample below)</li>
</ol>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3 id="improve-perf">Q. Ways to improve website performance</h3>

<ul>
  <li>Minimize HTTP Requests
    <ul>
	  <li>Sites are mainly slow because of too many (or too large) HTTP requests. We can 
	    eliminate unnecessary request;
      <li>combined files: js to a file, css to a file</li>
      <li>CSS sprites: CSS Sprites are the preferred method for reducing the number of 
	    image requests. Combine your background images into a single image and use the 
		CSS background-image and background-position properties to display the desired 
		image segment.</li>
	  </li>
	</ul>
  </li>
  <li>Use a Content Delivery Network CDN
    <ul>
	  <li>A CDN is essentially many optimized servers around the world that deliver web 
	    content to users based on their geographic location. This means big performance 
		improvements for site users. Because, say, if a person accessing your site in 
		India, they will be retrieving web content from a server nearby</li>
	</ul>
  </li>
  <li>Optimize Images:
    <ul>
	  <li>image sizes make a huge difference to site speed. The larger content/images, the 
	    slower the site. we could:
	    <ul>
		  <li>Changing the resolution: reducing the “quality” of the image (and thereby 
		    the file size)
		    <ul>
              <li>Compressing the picture: increasing the efficiency of image data storage</li>
			  <li>Cropping the picture: when cropping, you are cutting out unneeded areas and 
			    thus making the image smaller in size</li>
			</ul>
		  </li>
		</ul>
	  </li>
    </ul>
  </li>
  <li>Put Scripts at the Bottom:
    <ul>
	  <li>Javascript files can load after the rest of your page. The simplest solution is to place your external Javascript files at the bottom of your page, just before the close of your body tag. Now more of your site can load before your scripts. Another method that allows even more control is to use the defer or async attributes when placing external .js files on your site.
	    <ul>
          <li>Async tags load the scripts while the rest of the page loads, but this means scripts can be loaded out of order. Basically, lighter files load first. This might be fine for some scripts, but can be disastrous for others.</li>
		  <li>The defer attribute loads your scripts after your content has finished loading. It also runs the scripts in order. Just make sure your scripts run so late without breaking your site.</li>
		</ul>
      </li>
    </ul>
  </li>
  <li>Add an Expires or a Cache-Control Header
    <ul>
	  <li>Web page designs are getting richer and richer, which means more scripts, stylesheets, images, and Flash in the page. A first-time visitor to your page may have to make several HTTP requests, but by using the Expires header you make those components cacheable. This avoids unnecessary HTTP requests on subsequent page views. Expires headers are most often used with images, but they should be used on all components including scripts, stylesheets, and Flash components.</li>
	</ul>
  </li>
  <li>Gzip Components
    <ul>
	  <li>Compression reduces response times by reducing the size of the HTTP response. Gzipping generally reduces the response size by about 70%.</li>
  <li>Put Stylesheets at the Top:
    <ul>
	  <li>This is because putting stylesheets in the HEAD allows the page to render progressively.</li>
	</ul>
  </li>
  <li>Avoid CSS Expressions</li>
  <li>Use GET for AJAX Requests:
    <ul>
	  <li>Ajax is that it provides instantaneous feedback to the user because it requests information asynchronously from the backend web server.</li>
    </ul>
  </li>
  <li>Make JavaScript and CSS External:
    <ul>
      <li>Using external files in the real world generally produces faster pages because the JavaScript and CSS files are cached by the browser. JavaScript and CSS that are inlined in HTML documents get downloaded every time the HTML document is requested. This reduces the number of HTTP requests that are needed, but increases the size of the HTML document. On the other hand, if the JavaScript and CSS are in external files cached by the browser, the size of the HTML document is reduced without increasing the number of HTTP requests.</li>
	</ul>
  </li>
  <li>Use get to ajax request:
    <ul>
      <li>POST is implemented in the browsers as a two-step process: sending the headers first, then sending data. So it's best to use GET, which only takes one TCP packet to send (unless you have a lot of cookies).</li>
    </ul>
  </li>
  <li>No 404s:
    <ul>
	  <li>HTTP requests are expensive so making an HTTP request and getting a useless response (i.e. 404 Not Found) is totally unnecessary and will slow down the user experience without any benefit.</li>
	</ul>
  </li>
  <li>Reduce Cookie Size:
    <ul>
	  <li>HTTP cookies are used for a variety of reasons such as authentication and personalization. Information about cookies is exchanged in the HTTP headers between web servers and browsers. It's important to keep the size of cookies as low as possible to minimize the impact on the user's response time.</li>
	</ul>
  </li>
  <li>Reduce DNS Lookups</li>
  <li>Minify JavaScript and CSS</li>
  <li>Avoid Redirects</li>
  <li>Remove Duplicate Scripts</li>
  <li>Configure Etags</li>
  <li>Make Ajax Cacheable</li>
  <li>Post-load Components</li>
  <li>Preload Components</li>
  <li>Reduce the Number of DOM Elements</li>
  <li>Minimize the Number of iframes</li>
  <li>Minimize DOM Access</li>
  <li>Optimize CSS Sprites</li>
  <li>Don't Scale Images in HTML</li>
  <li>Make favicon.ico Small and Cacheable</li>
  <li>Avoid Empty Image src</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Comparison of browsers engines like Chrome, Firefox, Internet explorer, Safari?</h3>

* Chrome: 
    * Layout rendering engine <b>Webkit</b>. 
    * JavaScript engine <b>V8</b>

* Firefox: 
    * Layout rendering engine <b>Gecko</b>. 
    * JavaScript engine <b>Spider monkey</b>
        
* Internet explorer: 
    * Layout rendering engine <b>Trident</b>. 
    * JavaScript  engine <b>Chakra</b>
        
* Safari:
    * Layout rendering engine <b>Webkit</b>. 
    * JavaScript engine JavascriptCore i.e <b>Nitro</b>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What does the lang attribute in html do?</h3>

* Helps in styling pages by using them in css `:lang()` pseudo class Spelling and grammar checkers Languade detection by search engines

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is desktop first and mobile first design approach?</h3>

* Desktop first : 
        General selectors and styles designed to make the site look good on DESKTOP screens defined globally. But they affect all devices, and must be overridden by max-width media queries targeting minimum screen size

* Mobile First : 
        General selectors and styles designed to make the site look good on small MOBILE screens go here. But they affect all devices, and must be overridden by min-width media queries targeting maximum scrren size
    
    In desktop first approach the media queries will be written with respect to max-width whereas in mobile first approach media queries will be written with respect to min-width

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are `data-` attributes good for?</h3>

* The HTML5 data attribute lets you assign custom data to an element. When we want to store more information/data about the element when no suitable HTML5 element or attribute exists

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain the difference between layout, painting and compositing?</h3>

```
<img src="assets/lib/img/frame-full.jpg" alt="Browser Engine" />
```

<b>1. JavaScript:</b>

Typically JavaScript is used to handle work that will result in visual changes, whether 
it's jQuery's animate function, sorting a data set, or adding DOM elements to the page. 
It doesn't have to be JavaScript that triggers a visual change, though: CSS Animations, 
Transitions, and the Web Animations API are also commonly used.

<b>2. Style:</b>

This is the process of figuring out which CSS rules apply to which elements based on 
matching selectors, for example, .headline or .nav > .nav__item. From there, once 
rules are known, they are applied and the final styles for each element are calculated.

<b>3. Layout:</b>

Once the browser knows which rules apply to an element it can begin to calculate how much 
space it takes up and where it is on screen. The web's layout model means that one element 
can affect others, for example the width of the `<body>` element typically affects its 
children's widths and so on all the way up and down the tree, so the process can be quite 
involved for the browser.

<b>4. Paint:</b>

Painting is the process of filling in pixels. It involves drawing out text, colors, images, 
borders, and shadows, essentially every visual part of the elements. The drawing is typically 
done onto multiple surfaces, often called layers.

<b>5. Compositing:</b>

Since the parts of the page were drawn into potentially multiple layers they need to be 
drawn to the screen in the correct order so that the page renders correctly. This is 
especially important for elements that overlap another, since a mistake could result in 
one element appearing over the top of another incorrectly.

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain about HTML Layout Engines used by browsers?</h3>

|Engine          |Status   |Embedded in           |
|-------------|-----------------|--------------|
|WebKit          |Active    |Safari browser, plus all browsers hosted on the iOS App Store                        |
|Blink          |Active    |Google Chrome and all other Chromium-based browsers like Opera and Microsoft Edge    |
|Gecko          |Active    |Firefox browser and Thunderbird email client, plus forks like SeaMonkey and Waterfox |
|EdgeHTML      |Discontinued      |formerly in the Microsoft Edge browser                                         |
|Trident      |Discontinued      |Internet Explorer browser and Microsoft Outlook email client                   |

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How to make page responsive?</h3>

Responsive Web Design is about using HTML and CSS to automatically resize, hide, shrink, or enlarge, a website, to make it look good on all devices (desktops, tablets, and phones).

<b>1. Setting the viewport:</b>

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

<b>2. Responsive Images:</b>

If the CSS width property is set to 100%, the image will be responsive and scale up and down

```html
<img src="img.png" style="width:100%;">
```

<b>3. Show different Images depending on Browser Width:</b>

The HTML `<picture>` element allows you to define different images for different browser window sizes.

```html
<picture>
  <source srcset="img_small.jpg" media="(max-width: 600px)">
  <source srcset="img_large.jpg" media="(max-width: 1500px)">
  <source srcset="img.jpg">
  <img src="img_small.jpg" alt="Image">
</picture>
```

<b>4. Responsive Text Size:</b>

The text size can be set with a "vw" unit, which means the "viewport width". That way the text size will follow the size of the browser window.

```html
<h1 style="font-size:10vw">Hello World</h1>
```

<b>5. Media Queries:</b>

Using media queries you can define completely different styles for different browser sizes.

```css
/* Use a media query to add a breakpoint at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Does the following trigger http request at the time of page load?</h3>

```html
<img src="mypic.jpg" style="visibility: hidden" alt="My photo">

<div style="display: none;">
  <img src="mypic.jpg" alt="My photo">
</div>
```

* Yes

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. List the API available in HTML5?</h3>

<b>1. High Resolution Time API</b>

The High Resolution Time API provides the current time in sub-millisecond resolution and 
such that it is not subject to system clock skew or adjustments.

It exposes only one method, that belongs to the `window.performance` object, called 
`now()`. It returns a `DOMHighResTimeStamp` representing the current time in milliseconds. 
The timestamp is very accurate, with precision to a thousandth of a millisecond, allowing 
for accurate tests of the performance of our code.

```javascript
var time = performance.now();
```

<b>2. User Timing API</b>

It allows us to accurately measure and report the performance of a section of JavaScript 
code. It deals with two main concepts: mark and measure. The former represents an instant 
(timestamp), while the latter represents the time elapsed between two marks.

```javascript
performance.mark("startFoo");
// A time consuming function
foo();
performance.mark("endFoo");

performance.measure("durationFoo", "startFoo", "endFoo");
```

<b>3. Network Information API</b>

This API belongs to the connection property of the `window.navigator` object. It exposes 
two read-only properties: `bandwidth` and `metered`. The former is a number representing 
an estimation of the current bandwidth, while the latter is a Boolean whose value is true 
if the user's connection is subject to limitation and bandwidth usage, and false otherwise.

|Sl.No| API                            | Description
|-----|--------------------------------|--------------------------------------------------------------------|
| 01. |navigator.connection.type       |Network Type                               |
| 02. |navigator.connection.downlink   |Effective bandwidth estimate ( downlink )                               |
| 03. |navigator.connection.rtt        |Effective round-trip time estimate ( rtt )                                |
| 04. |navigator.connection.downlinkMax|Upper bound on the downlink speed of the first network hop ( downlinkMax )|
| 05. |navigator.connection.effectiveType|Effective connection type  |
| 06. |navigator.connection.saveData   |True if the user has requested a reduced data usage mode from the user agent ( saveData )|

<b>4.) Vibration API</b>

It exposes only one method, `vibrate()`, that belongs to the `window.navigator` object. This method accepts one parameter specifying the duration of the vibration in milliseconds. The parameter can be either an integer or an array of integers. In the second case, it's interpreted as alternating vibration times and pauses.

```javascript
// Vibrate once for 2 seconds
navigator.vibrate(2000);
```

<b>5.) Battery Status API</b>

The Battery Status API exposes four properties (`charging`, `chargingTime`, `discharingTime`, 
and `level`) and four events. The properties specify if the battery is in charge, the 
seconds remaining until the battery is fully charged, the seconds remaining until the 
battery is fully discharged, and the current level of the battery. These properties 
belongs to the `battery` property of the `window.navigator` object.

```javascript
// Retrieves the percentage of the current level of the device's battery
var percentageLevel = navigator.battery.level * 100;
```

<b>6.) Page Visibility API</b>

The Page Visibility API enables us to determine the current visibility state of the page. 
The Page Visibility API is especially useful for saving resources and improving performance 
by letting a page avoid performing unnecessary tasks when the document isn't visible.

```javascript
// document.hidden retuns true if page is not visible.
console.log('Page Visibility: '+document.hidden); 
```

<b>7.) Fullscreen API</b>

The Fullscreen API provides a way to request fullscreen display from the user, and exit 
this mode when desired. This API exposes two methods, `requestFullscreen()` and 
`exitFullscreen()`, allowing us to request an element to become fullscreen and to exit 
fullscreen.

```javascript
document.addEventListener("keypress", function(e) {
    if (e.keyCode === 13) { // Enter Key
        toggleFullScreen();
    }
}, false);

function toggleFullScreen() {
    if (!document.fullscreenElement) {
        document.documentElement.requestFullscreen();
    } else {
        if (document.exitFullscreen) {
        document.exitFullscreen(); 
        }
    }
}
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How geolocation api works in html5?</h3>

The Geolocation API allows the user to provide their location to web applications if they 
so desire. For privacy reasons, the user is asked for permission to report location information.

The Geolocation API is published through the `navigator.geolocation` object.

<details>
  <summary>html</summary>

```javascript
if ("geolocation" in navigator) {
  /* geolocation is available */
} else {
  /* geolocation IS NOT available */
}
```

</details>

<h5>Example</h5>
<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
    <head>
         <title>Geolocation</title>
    </head>
   <body>
    <p><button onclick="geoFindMe()">Show my location</button></p>
    <div id="out"></div>
</body>

<script type="text/javascript">
  /<b>
    The Geolocation API allows the user to provide their location to web applications 
    if they so desire. For privacy reasons, the user is asked for permission to report 
    location information.
  <b>/
  function geoFindMe() {
    var output = document.getElementById("out");

    if (!navigator.geolocation){
      output.innerHTML = "<p>Geolocation is not supported by your browser</p>";
      return;
    }

    function success(position) {
      var latitude  = position.coords.latitude;
      var longitude = position.coords.longitude;

      output.innerHTML = '<p>Latitude is ' + latitude + '° <br>Longitude is ' + longitude + '°</p>';
      var img = new Image();
      img.src = "https://maps.googleapis.com/maps/api/staticmap?center=" + latitude + "," + longitude + "&zoom=13&size=300x300&sensor=false";

      output.appendChild(img);
    }

    function error() {
      output.innerHTML = "Unable to retrieve your location";
    }

    output.innerHTML = "<p>Locating…</p>";

    navigator.geolocation.getCurrentPosition(success, error); //function to get the current position of the device
  }
</script>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the use of WebSocket API?</h3>

The <b>WebSocket API</b> is an advanced technology that makes it possible to open a two-way 
interactive communication session between the user's browser and a server. With this API, 
you can send messages to a server and receive event-driven responses without having to 
poll the server for a reply.

<b>Interfaces:</b>  

|Sl.No|   API      | Description    |
|-----|------------|----------------|
| 01. |WebSocket   |The primary interface for connecting to a WebSocket server and then sending and receiving data on the connection.|   
| 02. |CloseEvent  |The event sent by the WebSocket object when the connection closes.   |
| 03. |MessageEvent|The event sent by the WebSocket object when a message is received from the server.|

Example

```javascript
  // Create WebSocket connection.
  const socket = new WebSocket('ws://localhost:8080/');

  // Connection opened
  socket.addEventListener('open', function(event) {
    socket.send('Hello Server!');
  });

  // Listen for messages
  socket.addEventListener('message', function(event) {
    console.log('Message from server ', event.data);
  });
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain about HTML Canvas?</h3>

<p><b>canvas</b> is an HTML element which can be used to draw graphics via JavaScript. This can, 
for instance, be used to draw graphs, combine photos, or create animations.</p>

<h4><b>1. Colors, Styles, and Shadows:</b></h4>

|  Property    |    Description                                                           |
|--------------|--------------------------------------------------------------------------|
|fillStyle     | Sets or returns the color, gradient, or pattern used to fill the drawing |
|strokeStyle   | Sets or returns the color, gradient, or pattern used for strokes         |
|shadowColor   | Sets or returns the color to use for shadows                             |
|shadowBlur    | Sets or returns the blur level for shadows                               |
|shadowOffsetX | Sets or returns the horizontal distance of the shadow from the shape     |
|shadowOffsetY | Sets or returns the vertical distance of the shadow from the shape       |

<h4><b>2. Line Styles:</b></h4>

|Property     |  Description                                                   |
|------------|----------------------------------------------------------------|
|lineCap     |Sets or returns the style of the end caps for a line            |
|lineJoin     |Sets or returns the type of corner created, when two lines meet |
|lineWidth     |Sets or returns the current line width                          |
|miterLimit     |Sets or returns the maximum miter length                        |

<h4><b>3. Rectangles:</b></h4>
  
|Method         |Description                                          |
|---------------|-----------------------------------------------------|
|rect()         |Creates a rectangle                                  |
|fillRect()     |Draws a "filled" rectangle                           |
|strokeRect()   |Draws a rectangle (no fill)                          |
|clearRect()    |Clears the specified pixels within a given rectangle |

<h4><b>4. Paths:</b></h4>

| Method          | Description                                                                             |
|-----------------|-----------------------------------------------------------------------------------------|
|fill()      |Fills the current drawing (path)                                                              |
|stroke()    |Actually draws the path you have defined                                                      |
|beginPath() |Begins a path, or resets the current path                                                     |
|moveTo()    |Moves the path to the specified point in the canvas, without creating a line                  |
|closePath() |Creates a path from the current point back to the starting point                              |
|lineTo()    |Adds a new point and creates a line to that point from the last specified point in the canvas |
|clip()      |Clips a region of any shape and size from the original canvas                                 |
|arc()       |Creates an arc/curve (used to create circles, or parts of circles)                            |
|arcTo()     |Creates an arc/curve between two tangents                                                     |

<h4><b>5. Transformations:</b></h4>

| Method        | Description                                                                   |
|---------------|-------------------------------------------------------------------------------|
|scale()        | Scales the current drawing bigger or smaller                                  |
|rotate()       | Rotates the current drawing                                                   |
|translate()    | Remaps the (0,0) position on the canvas                                       |
|transform()    | Replaces the current transformation matrix for the drawing                    |
|setTransform() | Resets the current transform to the identity matrix. Then runs transform()    |

<h4><b>6. Text:</b></h4>

|Property        |Description                                                       |
|---------------|----------------------------------------------------------------- |
|font            |Sets or returns the current font properties for text content      |
|textAlign        |Sets or returns the current alignment for text content            |
|textBaseline    |Sets or returns the current text baseline used when drawing text  |
|fillText()        |Draws "filled" text on the canvas                                 |
|strokeText()    |Draws text on the canvas (no fill)                                |
|measureText()    |Returns an object that contains the width of the specified text   |

<h5><b>Example 01:</b> HTML5 Canvas for Text</h5>
<details>
  <summary>html</summary>

```html
<div>Text</div>
<canvas id="text" width="200" height="100" ></canvas>

<script type="text/javascript">
    // Text with style
    var canvas = document.getElementById('text');
    var context = canvas.getContext('2d');
    context.font = '20pt Calibri';
    context.fillStyle = 'blue';
    context.fillText('Hello World!', 50, 50);
</script>
```

</details>

<h5><b>Example 02:</b> HTML5 Canvas for Straight Line</h5>

<details>
  <summary>html</summary>

```html
<div>Straight Line</div>
<canvas id="line" width="300" height="0" style="border: 1px solid #333;"></canvas>

<script type="text/javascript">
    // Straight Line
    var canvas = document.getElementById("line");
    var context = canvas.getContext("2d");
    context.moveTo(50, 150);
    context.lineTo(250, 50);
    context.stroke();
</script>
```

</details>

<h5><b>Example 03:</b> HTML5 Canvas for Rectangle</h5>

<details>
  <summary>html</summary>

```html
<div>Rectangle with Style</div>
<canvas id="rectangle" width="300" height="200" style="border: 1px solid #999;"></canvas>

<script type="text/javascript">
    // Rectange with style
    var canvas = document.getElementById("rectangle");
    var context = canvas.getContext("2d");
    context.fillStyle = "#FF0000";
    context.fillRect(0, 0, 300, 200);
</script>
```

</details>

<h5><b>Example 04:</b> HTML5 Canvas for Circle</h5>

<details>
  <summary>html</summary>

```html
<div>Circle</div>
<canvas id="circle">This browser does not support Canvas!</canvas>

<script type="text/javascript">
  // Circle
  var canvas = document.getElementById("circle");
  var context = canvas.getContext("2d");
  context.beginPath();
  context.arc(95, 50, 40, 0, 2 * Math.PI);
  context.stroke();
</script>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is difference between SVG and Canvas?</h3>

<h4><b>1. SVG:</b></h4>

The Scalable Vector Graphics (SVG) is an XML-based image format that is used to define 
two-dimensional vector based graphics for the web. Unlike raster image (e.g. .jpg, .gif, 
.png, etc.), a vector image can be scaled up or down to any extent without losing the 
image quality.

There are following advantages of using SVG over other image formats like JPEG, GIF, PNG, etc.

<ul>
  <li>SVG images can be searched, indexed, scripted, and compressed.</li>
  <li>SVG images can be created and modified using JavaScript in real time.</li>
  <li>SVG images can be printed with high quality at any resolution.</li>
  <li>SVG content can be animated using the built-in animation elements.</li>
  <li>SVG images can contain hyperlinks to other documents.</li>
</ul>

<h5>Example:</h5>

<details>
  <summary>html</summary>
  
```html
<!DOCTYPE html>
<html>
   <head>
      <style>
         #svgelem {
            position: relative;
            left: 50%;
            -webkit-transform: translateX(-20%);
            -ms-transform: translateX(-20%);
            transform: translateX(-20%);
         }
      </style>
      <title>HTML5 SVG</title>
   </head>
   <body>
      <h2 align="center">HTML5 SVG Circle</h2>
      <svg id="svgelem" height="200" xmlns="http://www.w3.org/2000/svg">
         <circle id="bluecircle" cx="60" cy="60" r="50" fill="blue" />
      </svg>
   </body>
</html>
```

</details>

<h4><b>2. Canvas:</b></h4>

Canvas is a HTML element is used to draw graphics on a web page. It is a  bitmap with an 
“immediate mode” graphics application programming interface (API) for drawing on it. The 
`<canvas>` element is only a container for graphics. In order to draw the graphics, you 
are supposed to use a script. Canvas has several strategies when it comes to drawing paths, 
boxes, circles, text & adding images.

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
   <head>
      <title>HTML5 Canvas Tag</title>
   </head>
   <body>
      <canvas id="newCanvas" width="200" height="100" style="border:1px solid #000000;"></canvas>
      <script>
         var c = document.getElementById('newCanvas');
         var ctx = c.getContext('2d');
         ctx.fillStyle = '#7cce2b';
         ctx.fillRect(0,0,300,100);
      </script>
   </body>
</html>
```

</details>

<h4>Differences:</h4>

|SVG                    |Canvas                                         |
|-----------------------|-----------------------------------------------|
|Vector based (composed of shapes)    |Raster based (composed of pixel) |
|Multiple graphical elements, which become the part of the page's DOM tree|Single element similar to <img> in behavior. Canvas diagram can be saved to PNG or JPG format|
|Modified through script and CSS    |Modified through script only |
|Good text rendering capabilities    |Poor text rendering capabilities |
|Give better performance with smaller number of objects or larger surface, or both |Give better performance with larger number of objects or smaller surface, or both|
|Better scalability. Can be printed with high quality at any resolution. Pixelation does not occur | Poor scalability. Not suitable for printing on higher resolution. Pixelation may occur |

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain Drag and Drop in HTML5?</h3>

HTML5 drag-and-drop uses the `DOM event model` and `drag events` inherited from `mouse events`. 
A typical drag operation begins when a user selects a draggable element, drags the element 
to a droppable element, and then releases the dragged element.

|Event     |Description                                                                   |
|----------|------------------------------------------------------------------------------|
|Drag      |It fires every time when the mouse is moved while the object is being dragged.|
|Dragstart |It is a very initial stage. It fires when the user starts dragging object.    |
|Dragenter |It fires when the user moves his/her mouse cursur over the target element.    |
|Dragover  |This event is fired when the mouse moves over an element.                     |
|Dragleave |This event is fired when the mouse leaves an element.                         |
|Drop      |Drop It fires at the end of the drag operation.                               |
|Dragend   |It fires when user releases the mouse button to complete the drag operation.  |

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE HTML>
<html>
<head>
  <script>
    function allowDrop(ev) {
      ev.preventDefault();
    }

    function drag(ev) {
      ev.dataTransfer.setData("text", ev.target.id);
    }

    function drop(ev) {
      ev.preventDefault();
      var data = ev.dataTransfer.getData("text");
      ev.target.appendChild(document.getElementById(data));
    }
  </script>
</head>
<body>
  <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
  <img id="drag1" src="img_logo.gif" draggable="true" ondragstart="drag(event)" 
    width="336" height="69">
</body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain Microdata in HTML5?</h3>

Microdata is a standardized way to provide additional semantics in web pages. Microdata 
lets you define your own customized elements and start embedding custom properties in 
your web pages. At a high level, microdata consists of a group of name-value pairs.

The groups are called <b>items</b>, and each name-value pair is a <b>property</b>. Items and 
properties are represented by regular elements. Search engines benefit greatly from 
direct access to this structured data because it allows search engines to understand 
the information on web pages and provide more 
relevant results to users.

At a high level, microdata consists of a group of name-value pairs
<ul>
  <li><b>itemscope</b>:- To create an item</li>
  <li><b>itemprop</b>:- To add a property to an item</li>
</ul>

<h5>Example:</h5>

```html
<div itemscope>
  <p>My name is <span itemprop="name">Elizabeth</span>.</p>
</div>

<div itemscope>
  <p>My name is <span itemprop="name">Daniel</span>.</p>
</div>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What are the HTML tags which deprecated in HTML5?</h3>

<h4>1. Deprecated Tags:</h4>

The following elements are not available in HTML5 anymore and their function is better handled by CSS.

|Sl.No|Tags (Elements)  |    Description        |
|-----|-----------------|----------------------|
| 01. |`<acronym>`      |Defines an acronym|
| 02. |`<applet>`       |Defines an applet|
| 03. |`<basefont>`     |Defines an base font for the page|
| 04. |`<big>`          |Defines big text|
| 05. |`<center>`       |Defines centered text|
| 06. |`<dir>`          |Defines a directory list|
| 07. |`<font>`         |Defines text font, size, and color|
| 08. |`<frame>`        |Defines a frame|
| 08. |`<frameset>`     |Defines a set of frames|
| 10. |`<isindex>`      |Defines a single-line input field|
| 11. |`<noframes>`     |Defines a noframe section|
| 12. |`<s>`            |Defines strikethrough text|
| 13. |`<strike>`       |Defines strikethrough text|
| 14. |`<tt>`           |Defines teletype text|
| 15. |`<u>`            |Defines underlined text|

<h4>2. Deprecated Attributes:</h4>

|Removed Attributes      |From the Elements     |
|---------------------|----------------------|
|rev                  |link, a|
|charset              |link and a|
|shape                  |a|
|coords                  |a|
|longdesc              |img and iframe.|
|target                  |link|
|nohref                  |area|
|profile              |head|
|version              |html|
|name                  |img|
|scheme                  |meta|
|archive              |object|
|classid              |object|
|codebase              |object|
|codetype              |object|
|declare              |object|
|standby              |object|
|valuetype              |param|
|type                  |param|
|axis                  |td and t|
|abbr                  |td and t|
|scope                  |td|
|align                  |caption, iframe, img, input, object, legend, table, hr, div, h1, h2, h3, h4, h5, h6, p, col, colgroup, tbody, td, tfoot, th, thead and tr.|
|alink                  |body|
|link                  |body|
|vlink                  |body|
|text                  |body|
|background              |body|
|bgcolor              |table, tr, td, th and body.|
|border                  |table and object.|
|cellpadding          |table|
|cellspacing          |table|
|char                  |col, colgroup, tbody, td, tfoot, th, thead and tr.|
|charoff               |col, colgroup, tbody, td, tfoot, th, thead and tr.|
|clear                  |br|
|compact              |dl, menu, ol and ul.|
|frame                  |table|
|compact              |dl, menu, ol and ul.|
|frame                  |table|
|frameborder          |iframe|
|hspace                  |img and object.|
|vspace                  |img and object.|
|marginheight  |iframe|
|marginwidth   |iframe|
|noshade       |hr|
|nowrap        |td and th|
|rules         |table|
|scrolling     |iframe|
|size          |hr|
|type          |li, ol and ul.|
|valign        |col, colgroup, tbody, td, tfoot, th, thead and tr|
|width         |hr, table, td, th, col, colgroup and pre.|

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How you can Use Modernizr in HTML5?</h3>

Modernizr is a JavaScript library that detects which HTML5 and CSS3 features visitor's 
browser supports. In detecting feature support, it allows developers to test for some of 
the new technologies and then provide fallbacks for browsers that do not support them. 
This is called <b>feature detection</b> and is much more efficient than browser sniffing.

<h4>1. Using Modernizr with CSS:</h4>

By default, Modernizr sets classes for all of your tests on the root element (`<html>` for 
websites). This means adding the class for each feature when it is supported, and adding 
it with a no- prefix when it is not (e.g. `.feature` or `.no-feature`).

```css
.no-cssgradients .header {
  background: url("images/glossybutton.png");
}

.cssgradients .header {
  background-image: linear-gradient(cornflowerblue, rebeccapurple);
}
```

<h4>2. Using Modernizr with JavaScript:</h4>

Modernizr keeps track of the results of all of it's feature detections via the `Modernizr` object.

```javascript
  if (Modernizr.canvas) {
    alert("This browser supports HTML5 canvas!");
  } else {
    alert("no canvas :(");
  }
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is progressive rendering?</h3>

Progressive Rendering is the technique of sequentially rendering portions of a webpage in 
the server and streaming it to the client in parts without waiting for the whole page to 
rendered.

It implies that once the important material is produced on the server, you may stream it 
to the client without having to wait for non-critical stuff to be displayed. It combines 
the advantages of both CSR (Client Side Rendering) and SSR (Server Side Rendering) (Server 
Side Rendering).

<h4>1. Client Side Rendering:</h4>

<p>Client Side Rendering (CSR) is a technique in which content is rendered in the browser 
using JavaScript. Instead of getting all the content from the HTML file itself, the 
server sends HTML with an empty body and script tags that contain links to JavaScript 
bundles that the browser will use to render the content.</p>

<h5>Typical page load behaviour in CSR —</h5>

<ul>
  <li>Browser requests the server for HTML</li>
  <li>Server sends HTML with script tags in head and no content in body</li>
  <li>Browser parses the HTML and makes http requests to load the scripts</li>
  <li>Once the scripts are loaded, the browser parses them and makes API requests and loads 
    all the content asynchronously</li>
</ul>

<p>Since the all the content starts loading only after loading the initial JavaScript, it 
takes a longer time to show any content on the page. If the user is on a slow network, 
the content is blocked for an even longer time due to lower bandwidth and higher latency.</p>

<h4>2. Server Side Rendering:</h4>

<p>When rendering on the server side, the HTML is rendered on the server and sent to the 
client. The content that we need to display on the screen becomes available immediately 
after the HTML is parsed; hence, primary rendering of content is faster than CSR.</p>

<h5>Typical page load behaviour in SSR —</h5>

<ul>
  <li>Browser requests the server for HTML.</li>
  <li>Server makes API requests (usually co-located) and renders the content in the server.</li>
  <li>Once the page is ready, the server sends it to the browser.</li>
  <li>The browser loads and parses the HTML and paints the content on the screen without 
    waiting for the JavaScript bundle(s) to load.</li>
  <li>Once the JavaScript bundle(s) are loaded, the browser hydrates interactivity to DOM 
    elements, which is usually attaching event handlers and other interactive behaviours.</li>
</ul>

<p>Since the APIs are usually co-located with the server, the content is loaded super 
fast (faster than CSR) and the HTML is sent to the browser. Initial JavaScript load 
doesn't block content load as the HTML sent by the server already has the content.</p>

<p align="center">
  <img src="assets/images/progressive-rendering.png" alt="Progressive Rendering" width="500px" />
</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h2 id="07-html-iframe">07. HTML iframe</h2>

HTML iframes offer a powerful way to embed external content, such as videos, maps, or 
other webpages, directly into your own webpage. This article provides an in-depth 
exploration of HTML iframes, their syntax, and how they can be used to enhance your 
web development projects.

<h3>What are HTML Iframes?</h3>
An iframe is an HTML document embedded inside another HTML document. The `<iframe>` tag 
specifies the URL of the embedded content, allowing for seamless integration of external 
resources. This section will guide you through the syntax and attributes of the `<iframe>` 
tag, providing a solid foundation for your iframe usage.

<h5>Syntax:</h5>

```html
<iframe src="URL" title="description"></iframe>
```

The src attribute specifies the URL of the document you want to embed.
Iframes can include videos, maps, or entire web pages from other sources.

<h3>Q. What is an iframe and how does it work?</h3>

The `<iframe>` HTML element represents a nested browsing context, embedding another HTML 
page into the current one. Each embedded browsing context has its own <b>session history</b> 
and <b>document</b>. The browsing context that embeds the others is called the parent browsing 
context. The topmost browsing context — the one with no parent — is usually the browser 
window, represented by the <b>Window</b> object.

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
  <head>
    <title>HTML5 iframe</title>
  </head>
  <style type="text/css">
    iframe {
      border: 1px solid #333;
      width: 50%;
    }
    .output {
      background: #eee;
    }
  </style>
  <body>
    <p>The Inline iFrame Example</p>
    <iframe id="inlineFrameId"
      title="Inline iFrame Example"
      width="300"
      height="200"
      src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&layer=mapnik">
        Sorry your browser does not support inline frames.
    </iframe>
  </body>
</html>
```

</details>

<h4>The Iframe Tag Attributes:</h4>

|Attribute       | Description                |
|----------------|----------------------------|
|allow           |indicates what features the iframe is allowed to use (e.g. fullscreen, camera, autoplay)|
|allowfullscreen |grants or denies permission for the iframe to appear in full-screen mode|
|height           |sets the height of the iframe (if not specified, the default height is 150 pixels)|
|loading         |sets lazy loading or eager loading for the iframe|
|referrerpolicy  |sets what referrer information should be sent in the request for the iframe|
|src             |the address of the resource included in the iframe|
|width           |sets the width of the iframe (if not specified, the default width is 300 pixels)|

<i>Note: Because each browsing context is a complete document environment, every `<iframe>` 
in a page requires increased memory and other computing resources.</i>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Explain the use of rel="nofollow", rel="noreferrer", rel="noopener" attribute?</h3>

<h4>1. rel="nofollow"</h4>

When `rel="nofollow"` tag is used, it instruct the search engines not to pass any PageRank 
from one page to the other. It does not allow it to pass the authority to the specific 
website. The main advantage of using this attribute is to control the spam attack.

There may be times, when you do not have control over what people publish on your websites, 
for example some blog comments and some kind of forum posting.

<h5>Example:</h5>

```html
<a href="https://www.website.com" rel="nofollow">Link to yoursite.com</a>
```

<h4>2. rel="noreferrer"</h4>

Noreferrer is related to analytics and tracking. The referrer value shows the previous 
page where a user came from. By using the noreferrer attribute on a link, you are 
preventing other pages from seeing that traffic came from a click on your link.

<h5>Example:</h5>

```html
<a href="https://www.website.com" rel="noreferrer">Link to yoursite.com</a>
```

<h4>3. rel="noopener"</h4>

It prevents the new page from being able to access the `window.opener` property and will 
make it run in a separate process. noopener tag works as a security fix which prevents 
malicious links to take control over an opened tab.

<h5>Example:</h5>

```html
<a href="https://www.website.com" target="_blank" rel="noopener">Link to yoursite.com</a>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How can you highlight text in HTML?</h3>

The `<mark>` HTML element represents text which is marked or highlighted for reference or 
notation purposes, due to the marked passage's relevance or importance in the enclosing 
context.

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Highlight text in HTML</title>
  </head>
  <body>
    <p>Search results for "salamander":</p>
    <hr>
    <p>Several species of <mark>salamander</mark> inhabit the temperate rainforest of the 
	  Pacific Northwest.</p>
    <p>Most <mark>salamander</mark>s are nocturnal, and hunt for insects, worms, and other 
	  small creatures.</p>
  </body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How can I get indexed better by search engines?</h3>

HTML tags are used to influence the way our pages appear in search results. With the help 
of certain tags, we can turn regular search snippets into rich snippets, and maybe even 
into featured snippets. And, as our search snippets get more advanced, they are able to 
secure better <b>Search Engine Results Pages (SERP)</b> positions and attract more traffic.

Here are all the HTML tags that still matter:

<h2 id="02-html-tags">02. HTML Tags</h2>

<h3>1. Title tag:</h3>

Title tags are used by search engines to determine the subject of a page and display it 
in SERP. As a rule of thumb, titles that are under 60 characters long will fit on most 
screens. In HTML, a title tag looks like this:

```html
<title>Your Title Goes Here</title>
```

<h3>2. Meta description tag:</h3>

Meta description is a short paragraph of text used to describe your page in search results. 
The function of meta description is similar to the title. It provides a little more detail 
about your page and it helps users decide whether to visit your page or not. In HTML, a 
meta description tag looks like this:

```html
<meta name="description" content="Your description goes here">
```

<h3>3. Heading tags:</h3>

Headings (H1-H6) are used to split your page into sections or chapters. Each heading is 
like a small title within the page. In HTML, a heading looks like this:

```html
<h1>Your heading goes here</h1>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>4. Image alt attribute:</h3>

The `alt` text attribute is a part of an image tag, and it provides a description for an 
image. Alt text plays a major role in image optimization. It makes your images accessible 
both to search engines (by telling them what a particular image means) and to people (by 
displaying an alternative text in case a particular image cannot be loaded or by helping 
screen readers convey images). In HTML it may look like this:

```html
<img src="url" alt="Your image description goes here">
```

<h3>5. Open Graph tags:</h3>

Open Graph (OG) tags are placed in the `<head>` section of a page and allow any webpage 
to become a rich object in social networks. OG tags let you control how the information 
about your page is represented when shared via social channels. This possibility may help 
you enhance the performance of your links on social media, thus driving more click-throughs 
and increasing conversions. In HTML, it can look like this:

```html
<meta name="og:title" property="og:title" content="Your Open Graph Title Goes Here">
```

<h3>6. Robots tag:</h3>

A robots tag is an element in the HTML of a page that informs search engines which pages 
on your site should be indexed and which should not. Its functions are similar to robots.txt, 
but robots.txt gives suggestions. Whereas robots tags give instructions. In HTML, it can 
look like this:

```html
<meta name="robots" content="index, follow">
```

<h3>7. Canonical tag:</h3>

A canonical tag is a way of telling search engines that a specific URL represents the 
master copy of a page. Using the canonical tag prevents problems caused by identical 
or "duplicate" content appearing on multiple URLs. Practically speaking, the canonical 
tag tells search engines which version of a URL you want to appear in search results. 
In HTML, it may look like this:

```html
<link href="URL" rel="canonical">
```

<h3>8. HTML5 semantic tags:</h3>

One of the most important features of HTML5 is its semantics tags. Semantic tags refers to 
syntax that makes the HTML more comprehensible by better defining the different sections 
and layout of web pages. It makes web pages more informative and adaptable, allowing browsers 
and search engines to better interpret content. For example, instead of using 
`<div id="header"></div>` you can use a `<header></hrader>` tag.

<p align="center">
  <img src="assets/images/semantic-tags.png" alt="HTML5 semantic tags" width="300px" />
</p>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the difference between an "attribute" and a "property" in HTML?</h3>

Attributes are defined by HTML. Properties are accessed from DOM (Document Object Model) nodes.

<h5>Example:</h5>

```html
<input id="inputId" type="text" value="Hello World!" />
```

The <b>value</b> property reflects the current text-content inside the input box, 
whereas the <b>value</b> attribute contains the initial text-content of the <b>value</b> 
attribute from the HTML source code

<h4>Difference between HTML attributes and DOM properties:</h4>

|Attribute                               |Property                |
|----------------------------------------|------------------------|
|Attributes are defined by HTML.         |Properties are defined by the DOM.|
|The value of an attribute is constant.  |The value of a property is variable.|
|These are used to initialize the DOM properties.| No such job defined.|

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How do you set IE compatibility mode?</h3>

<b>X-UA-Compatible</b> is a document mode meta tag that allows to choose what version of 
Internet Explorer the page should be rendered as. It is used by Internet Explorer 8 to 
specify whether a page should be rendered as IE 7 (compatibility view) or IE 8 (standards view).

<details>
  <summary>html</summary>

```html
<html>
  <head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <title>My Web Page</title>
  </head>
  <body>
    <p>Content goes here.</p>
  </body>
</html>
```

</details>

Emulating the version tells the browser to use the DOCTYPE to determine how to render 
content. pages without a DOCTYPE will be rendered in quirks mode. Edge mode tells Windows 
Internet Explorer to display content in the highest mode available, which actually breaks 
the "lock-in" paradigm. With Internet Explorer 8, this is equivalent to IE8 mode.

<h4>Setting the Meta Element:</h4>

The meta element includes a content attribute that enables you to specify the mode that 
content is rendered in for the webpage, as the following table shows.

|Value          |Rendering mode                                              |
|---------------|------------------------------------------------------------|
|IE=edge        |Display content in the highest mode available               |
|IE=9           |Use the Windows Internet Explorer 9 standards rendering mode|
|IE=8           |Use the Internet Explorer 8 standards rendering mode        |
|IE=7           |Use the Windows Internet Explorer 7 standards rendering mode|
|IE=5           |Use the Microsoft Internet Explorer 5 standards rendering mode|

<i>Note: It is recommended that Web developers restrict their use of Edge mode to test pages 
and other non-production uses because of the possible unexpected results of rendering page 
content in future versions of Windows Internet Explorer.</i>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is an optional tag?</h3>

The following lists all optional tags.

|Tag            |Description  |
|---------------|-------------|
|`<area>`       | The `<area>` tag defines an area inside an image map (an image map is an image with clickable areas).|
|               | `<area>` elements are always nested inside a `<map>` tag. |
|               | Note: The usemap attribute in `<img>` is associated with the `<map>` element's name attribute, and creates a relationship between the image and the map. |
|               | See <a href="https://www.w3schools.com/tags/tag_area.asp">area tag</a> |
|`<base>`       | The `<base>` tag specifies the base URL and/or target for all relative URLs in a document. |
|               | The `<base>` tag must have either an href or a target attribute present, or both. |
|               | There can only be one single `<base>` element in a document, and it must be inside the `<head>` element. |
|               | See <a href="https://www.w3schools.com/tags/tag_base.asp">base tag</a> |
|`<body>`       | The `<body>` tag defines the document's body. |
|               | The `<body>` element contains all the contents of an HTML document, such as headings, paragraphs, images, hyperlinks, tables, lists, etc. |
|               | Note: There can only be one `<body>` element in an HTML document.            |
|               | See <a href="https://www.w3schools.com/tags/tag_body.asp">body tag</a> |
|`<br>`         | The `<br>` tag inserts a single line break. |
|               | The `<br>` tag is useful for writing addresses or poems. |
|               | The `<br>` tag is an empty tag which means that it has no end tag. |
|               | See <a href="https://www.w3schools.com/tags/tag_br.asp">br tag</a> |
|`<caption>`    | The `<caption>` tag defines a table caption. |
|               | The `<caption>` tag must be inserted immediately after the `<table>` tag. |
|               | Tip: By default, a table caption will be center-aligned above a table. However, the CSS properties text-align and caption-side can be used to align and place the caption. |
|               | See <a href="https://www.w3schools.com/tags/tag_caption.asp">caption tag</a> |
|`<col>`        | The `<col>` tag specifies column properties for each column within a `<colgroup>` element. |
|               | The `<col>` tag is useful for applying styles to entire columns, instead of repeating the styles for each cell, for each row. |
|               | See <a href="https://www.w3schools.com/tags/tag_col.asp">col tag</a> |
|`<colgroup>`   | The `<colgroup>` tag specifies a group of one or more columns in a table for formatting. |
|               | The `<colgroup>` tag is useful for applying styles to entire columns, instead of repeating the styles for each cell, for each row. |
|               | Note: The `<colgroup>` tag must be a child of a `<table>` element, after any `<caption>` elements and before any `<thead>`, `<tbody>`, `<tfoot>`, and `<tr>` elements. |
|               | Tip: To define different properties to a column within a `<colgroup>`, use the `<col>` tag within the `<colgroup>` tag. |
|               | See <a href="https://www.w3schools.com/tags/tag_colgroup.asp">colgroup tag</a> |
|`<dd>`         | The `<dd>` tag is used to describe a term/name in a description list. |
|               | The `<dd>` tag is used in conjunction with `<dl>` (defines a description list) and `<dt>` (defines terms/names). |
|               | Inside a `<dd>` tag you can put paragraphs, line breaks, images, links, lists, etc. |
|               | See <a href="https://www.w3schools.com/tags/tag_dd.asp">dd tag</a> |
|`<dt>`         | The `<dt>` tag defines a term/name in a description list. |
|               | The `<dt>` tag is used in conjunction with `<dl>` (defines a description list) and `<dd>` (describes each term/name). |
|               | See <a href="https://www.w3schools.com/tags/tag_dt.asp">dt tag</a> |
|`<embed>`      | The `<embed>` tag defines a container for an external resource, such as a web page, a picture, a media player, or a plug-in application. |
|               | See <a href="https://www.w3schools.com/tags/tag_embed.asp">embed tag</a> |
|`<head>`       | The `<head>` element is a container for metadata (data about data) and is placed between the `<html>` tag and the `<body>` tag. |
|               | Metadata is data about the HTML document. Metadata is not displayed. |
|               | Metadata typically define the document title, character set, styles, scripts, and other meta information. |
|               | The following elements can go inside the `<head>` element: |
|               | - `<title>` (required in every HTML document) |
|               | - `<style>` |
|               | - `<base>`  |
|               | - `<link>`  |
|               | - `<meta>`  |
|               | - `<script>` |
|               | - `<noscript>` |
|               | See <a href="https://www.w3schools.com/tags/tag_head.asp">head tag</a> |
|`<hr>`         | The `<hr>` tag defines a thematic break in an HTML page (e.g. a shift of topic). |
|               | The `<hr>` element is most often displayed as a horizontal rule that is used to separate content (or define a change) in an HTML page. |
|               | See <a href="https://www.w3schools.com/tags/tag_hr.asp">hr tag</a> |
|`<html>`       | The `<html>` tag represents the root of an HTML document. |
|               | The `<html>` tag is the container for all other HTML elements (except for the `<!DOCTYPE>` tag). |
|               | Note: You should always include the lang attribute inside the `<html>` tag, to declare the language of the Web page. This is meant to assist search engines and browsers. |
|               | `<!DOCTYPE html>` |
|               | `<html lang="en">` |
|               | `<head>`
|               |   `<title>`Title of the document`</title>` |
|               | `</head>` |
|               | `<body>` |
|               |   `<h1>`This is a heading`</h1>` |
|               |   `<p>`This is a paragraph.`</p>` |
|               | `</body>` |
|               | `</html>` |
|               | See <a href="https://www.w3schools.com/tags/tag_html.asp">html tag</a> |
|`<img>`        | The `<img>` tag is used to embed an image in an HTML page. |
|               | Images are not technically inserted into a web page; images are linked to web pages. The `<img>` tag creates a holding space for the referenced image. |
|               | The `<img>` tag has two required attributes: |
|               |   - src - Specifies the path to the image |
|               |   - alt - Specifies an alternate text for the image, if the image for some reason cannot be displayed |
|               | Note: Also, always specify the width and height of an image. If width and height are not specified, the page might flicker while the image loads. |
|               | Tip: To link an image to another document, simply nest the `<img>` tag inside an `<a>` tag (see example below). |

| Image tag | Attribute     | Value           | Description                        |
|-----------|---------------|-----------------|-----------------------------------|
| `<img>`   | alt            | text            | Specifies an alternate text for an image.  |
|           | crossorigin    | anonymous       | Allow images from third-party sites that allow cross-origin access to be used with canvas. |
|           |                | use-credentials |                          |
|           | height         | pixels	       | Specifies the height of an image. |
|           | ismap          | ismap           | Specifies an image as a server-side image map. |
|           | loading        | eager           | Specifies whether a browser should load an image immediately or to defer loading of images until some conditions are met. |
|           |                | lazy            |                   |
|           | longdesc       | URL             | Specifies a URL to a detailed description of an image. |
|           | referrerpolicy | no-referrer     | Specifies which referrer information to use when fetching an image. |
|           |                | no-referrer-when-downgrade |            |
|           |                | origin          |                       |
|           |                | origin-when-cross-origin |              |
|           |                | unsafe-url	|                          |
|           | sizes          | sizes | Specifies image sizes for different page layouts. |
|           | src            | URL   | Specifies the path to the image. |
|           | srcset         | URL-list | Specifies a list of image files to use in different situations. |
|           | usemap         | #mapname	| Specifies an image as a client-side image map. |
|           | width          | pixels   | Specifies the width of an image. |
|           | See <a href="https://www.w3schools.com/tags/tag_img.asp">img tag</a> |

Optional tags, cont'd

|Tag            |Description  |
|---------------|-------------|
|`<input>`      | The `<input>` tag specifies an input field where the user can enter data. |
|               | The `<input>` element is the most important form element. |
|               | The `<input>` element can be displayed in several ways, depending on the type attribute. |
|               | The different input types are as follows: |
|               | - `<input type="button">` |
|               | - `<input type="checkbox">` |
|               | - `<input type="color">` |
|               | - `<input type="date">` |
|               | - `<input type="datetime-local">` |
|               | - `<input type="email">` |
|               | - `<input type="file">` |
|               | - `<input type="hidden">` |
|               | - `<input type="image">` |
|               | - `<input type="month">` |
|               | - `<input type="number">` |
|               | - `<input type="password">` |
|               | - `<input type="radio">` |
|               | - `<input type="range">` |
|               | - `<input type="reset">` |
|               | - `<input type="search">` |
|               | - `<input type="submit">` |
|               | - `<input type="tel">` |
|               | - `<input type="text"> (default value)` |
|               | - `<input type="time">` |
|               | - `<input type="url">` |
|               | - `<input type="week">` |
|               | Look at the <a href="https://www.w3schools.com/tags/att_input_type.asp">type</a> attribute to see examples for each input type! |
|               | Tip: Always use the <label> tag to define labels for `<input type="text">`, `<input type="checkbox">`, `<input type="radio">`, `<input type="file">`, and `<input type="password">`. |
|               | See <a href="https://www.w3schools.com/tags/tag_input.asp">input tag</a> |
|`<li>`         | The `<li>` tag defines a list item. |
|               | The `<li>` tag is used inside ordered lists(`<ol>`), unordered lists (`<ul>`), and in menu lists (`<menu>`). |
|               | In `<ul>` and `<menu>`, the list items will usually be displayed with bullet points. |
|               | In `<ol>`, the list items will usually be displayed with numbers or letters. |
|               | Tip: Use CSS to style lists. |
|               | See <a href="https://www.w3schools.com/tags/tag_li.asp">li tag</a> |
|`<link>`       | The `<link>` tag defines the relationship between the current document and an external resource. |
|               | The `<link>` tag is most often used to link to external style sheets or to add a favicon to your website. |
|               | The `<link>` element is an empty element, it contains attributes only.            |
|               | See <a href="https://www.w3schools.com/tags/tag_link.asp">link tag</a> |
|`<meta>`       | The `<meta>` tag defines metadata about an HTML document. Metadata is data (information) about data. |
|               | `<meta>` tags always go inside the <head> element, and are typically used to specify character set, page description, keywords, author of the document, and viewport settings. |
|               | Metadata will not be displayed on the page, but is machine parsable. |
|               | Metadata is used by browsers (how to display content or reload page), search engines (keywords), and other web services. |
|               | There is a method to let web designers take control over the viewport (the user's visible area of a web page), through the <meta> tag (See "Setting The Viewport" example below). |
|               | See <a href="https://www.w3schools.com/tags/tag_meta.asp">meta tag</a> |
|`<optgroup>`   | The `<optgroup>` tag is used to group related options in a `<select>` element (drop-down list). |
|               | If you have a long list of options, groups of related options are easier to handle for a user. |
|               | See <a href="https://www.w3schools.com/tags/tag_optgroup.asp">optgroup tag</a> |
|`<option>`     | The `<option>` tag defines an option in a select list. |
|               | `<option>` elements go inside a `<select>`, `<optgroup>`, or `<datalist>` element. |
|               | Note: The `<option>` tag can be used without any attributes, but you usually need the value attribute, which indicates what is sent to the server on form submission. |
|               | Tip: If you have a long list of options, you can group related options within the `<optgroup>` tag. |
|               | See <a href="https://www.w3schools.com/tags/tag_option.asp">option tag</a> |
|`<p>`          | The `<p>` tag defines a paragraph. |
|               | Browsers automatically add a single blank line before and after each `<p>` element. |
|               | Tip: Use CSS to style paragraphs. |
|               | See <a href="https://www.w3schools.com/tags/tag_p.asp">p tag</a> |
|`<param>`      | The `<param>` tag is used to define parameters for an `<object>` element. |
|               | See <a href="https://www.w3schools.com/tags/tag_param.asp">param tag</a> |

| Attribute | Value | Description |
|-----------|--------|-------------------------------------------------------------|
| name	    | name   | Specifies the name of a parameter |
| value     | value  | Specifies the value of the parameter |

Optional tags, cont'd

|Tag            |Description  |
|---------------|-------------|
|`<rp>`         | The `<rp>` tag can be used to provide parentheses around a ruby text, to be shown by browsers that do not support ruby annotations. |
|               | Use `<rp>` together with `<ruby>` and `<rt>`: The `<ruby>` element consists of one or more characters that needs an explanation/pronunciation, and an `<rt>` element that gives that information, and an optional `<rp>` element that defines what to show for browsers that not support ruby annotations. |
|               | See <a href="https://www.w3schools.com/tags/tag_rp.asp">rp tag</a> |
|`<rt>`         | The `<rt>` tag defines an explanation or pronunciation of characters (for East Asian typography) in a ruby annotation.
|               | Use `<rt>` together with `<ruby>` and `<rp>`: The `<ruby>` element consists of one or more characters that needs an explanation/pronunciation, and an `<rt>` element that gives that information, and an optional `<rp>` element that defines what to show for browsers that not support ruby annotations.  |
|               | See <a href="https://www.w3schools.com/tags/tag_rt.asp">rt tag</a> |
|`<source>`     | The `<source>` tag is used to specify multiple media resources for media elements, such as `<video>`, `<audio>`, and `<picture>`. |
|               | The `<source>` tag allows you to specify alternative video/audio/image files which the browser may choose from, based on browser support or viewport width. The browser will choose the first `<source>` it supports. |
|               | See <a href="https://www.w3schools.com/tags/tag_source.asp">source tag</a> |
|`<tbody>`      | The `<tbody>` tag is used to group the body content in an HTML table. |
|               | The `<tbody>` element is used in conjunction with the `<thead>` and `<tfoot>` elements to specify each part of a table (body, header, footer). |
|               | Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page. |
|               | Note: The `<tbody>` element must have one or more `<tr>` tags inside. |
|               | The `<tbody>` tag must be used in the following context: As a child of a `<table>` element, after any `<caption>`, `<colgroup>`, and `<thead>` elements. |
|               | Tip: The `<thead>`, `<tbody>`, and `<tfoot>` elements will not affect the layout of the table by default. However, you can use CSS to style these elements (see example below)!  |
|               | See <a href="https://www.w3schools.com/tags/tag_tbody.asp">tbody tag</a> |
|`<td>`         | The `<td>` tag defines a standard data cell in an HTML table. |
|               | An HTML table has two kinds of cells: |
|               |   - Header cells - contains header information (created with the `<th>` element) |
|               |   - Data cells - contains data (created with the `<td>` element) |
|               | The text in `<td>` elements are regular and left-aligned by default. |
|               | The text in `<th>` elements are bold and centered by default. |
|               | See <a href="https://www.w3schools.com/tags/tag_td.asp">td tag</a> |
|`<tfoot>`      | The `<tfoot>` tag is used to group footer content in an HTML table. |
|               | The `<tfoot>` element is used in conjunction with the `<thead>` and `<tbody>` elements to specify each part of a table (footer, header, body). |
|               | Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page. |
|               | Note: The `<tfoot>` element must have one or more `<tr>` tags inside. |
|               | The `<tfoot>` tag must be used in the following context: As a child of a `<table>` element, after any `<caption>`, `<colgroup>`, `<thead>`, and `<tbody>` elements. |
|               | Tip: The `<thead>`, `<tbody>`, and `<tfoot>` elements will not affect the layout of the table by default. However, you can use CSS to style these elements (see example below)! |
|               | See <a href="https://www.w3schools.com/tags/tag_tfoot.asp">tfoot tag</a> |
|`<th>`         | The `<th>` tag defines a header cell in an HTML table. |
|               | An HTML table has two kinds of cells: |
|               |   - Header cells - contains header information (created with the `<th>` element) |
|               |   - Data cells - contains data (created with the `<td>` element) |
|               | The text in `<th>` elements are bold and centered by default. |
|               | The text in `<td>` elements are regular and left-aligned by default. |
|               | See <a href="https://www.w3schools.com/tags/tag_th.asp">th tag</a> |
|`<thead>`      | The `<thead>` tag is used to group header content in an HTML table. |
|               | The `<thead>` element is used in conjunction with the `<tbody>` and `<tfoot>` elements to specify each part of a table (header, body, footer). |
|               | Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page. |
|               | Note: The `<thead>` element must have one or more `<tr>` tags inside. |
|               | The `<thead>` tag must be used in the following context: As a child of a `<table>` element, after any `<caption>` and `<colgroup>` elements, and before any `<tbody>`, `<tfoot>`, and `<tr>` elements. |
|               | Tip: The `<thead>`, `<tbody>`, and `<tfoot>` elements will not affect the layout of the table by default. However, you can use CSS to style these elements (see example below)! |
|               | See <a href="https://www.w3schools.com/tags/tag_thead.asp">thead tag</a> |
|`<tr>`         | The `<tr>` tag defines a row in an HTML table. |
|               | A `<tr>` element contains one or more `<th>` or `<td>` elements. |
|               | See <a href="https://www.w3schools.com/tags/tag_tr.asp">tr tag</a> |
|`<track>`      | The `<track>` tag specifies text tracks for `<audio>` or `<video>` elements. |
|               | This element is used to specify subtitles, caption files or other files containing text, that should be visible when the media is playing. |
|               | Tracks are formatted in WebVTT format (.vtt files). |
|               | See <a href="https://www.w3schools.com/tags/tag_track.asp">track tag</a> |
|`<wbr>`        | The `<wbr>` (Word Break Opportunity) tag specifies where in a text it would be ok to add a line-break. |
|               | Tip: When a word is too long, the browser might break it at the wrong place. You can use the `<wbr>` element to add word break opportunities. |
|               | See <a href="https://www.w3schools.com/tags/tag_wbr.asp">wbr tag</a> |

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is an HTML preprocessor? Have you used different HTML templating languages before?</h3>

A <b>HTML preprocessor</b> is a program that takes one type of data and converts it to another 
one. In case of HTML and CSS, some of the more popular preprocessor languages are Slim and 
Sass. Slim is processed into HTML and Sass is processed into CSS.

No, but I heard about html template language like PUG (formerly Jade), Haml, ERB, Slim, 
Handlebars, Jinja, Liquid etc which is HTML preprocessor this mean that it is basically 
a language that will be converted to native html code.

The typical usage is when you render something on the server side. The usual use-case is 
when you have to add dynamic content to your website, so when you fetch something from 
your database, you will have to replace some parts in your original template.

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How do you change the direction of html text?</h3>

The default text direction in HTML is left-to-right. However, when developing web content 
and applications, we may need to set it to right-to-left, for instance, to cater for 
languages such as Arabic, Hebrew, Pashto, Persian, Urdu, and Sindhi.

<h4>We can set text direction in HTML in one of two ways:</h4>

<ul>
  <li>With the HTML <b>dir</b> attribute</li>
  <li>With the CSS <b>direction</b> property</li>
</ul>

<h5>Example:</h5>

```html
<!-- Syntax -->
<element dir="ltr|rtl|auto">

<!-- Example -->
<textarea dir="rtl"></textarea>
```

<h4>Attribute Values:</h4>

|Value          |Description                |
|---------------|---------------------------|
|ltr            |Default. Left-to-right text direction|
|rtl            |Right-to-left text direction|
|auto           |Let the browser figure out the text direction, based on the content|

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. When is it appropriate to use the small element?</h3>

The `<small>` HTML element represents side-comments and small print, like copyright and 
legal text, independent of its styled presentation. By default, it renders text within 
it one font-size smaller, such as from `small` to `x-small`.

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
  <head>
      <title>Small Element</title>
  </head>
  <style>
    small {
      font-size: .7em
    }
  </style>
  <body>
    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
    <hr>
    <p><small>The content is licensed under a W3C License.</small></p>
  </body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. How do you serve a page with content in multiple languages?</h3>

The <b>lang</b> attribute specifies the language of the element's content.

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>HTML5 Multilanguage Page</title>
  </head>
  <body>
    <h2>English</h2>
    <p lang="en">This is demo text</p>
     
    <h2>French</h2>
    <p lang="fr">Ceci est un texte de démonstration</p>
     
    <h2>Spanish</h2>
    <p lang="es">Este es un texto de demostración</p>
  </body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is the difference between `&lt;section&gt;` and `&lt;div&gt;`?</h3>

The `<section>` tag creates independent sections within a webpage having logically connected 
content. And the `<div>` tag is an empty container specifying a division or a section.

<h4>The `&lt;section&gt;` Element</h4>

According to the W3C specification, the `<section>` tag means that the content inside this 
element is grouped. In other words, the content relates to a single theme. It must be an 
entry in the outline of the page.

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Section Tag Example</title>
  </head>
  <body>
    <h1>W3Docs</h1>
    <section>
      <h2>W3Docs Sections</h2>
      <ul>
        <li>Books</li>
        <li>Quizzes</li>
        <li>Snippets</li>
      </ul>
    </section>
    <section>
      <h3>Books</h3>
      <p>Learn HTML</p>
      <p>Learn CSS</p>
      <p>Learn Javascript</p>
    </section>
  </body>
</html>
```

</details>

<h4>The `&lt;div&gt;` Element</h4>

The `<div>` element only represents its child elements and doesn't have a special meaning. 
It can be used with the `lang`, `title`, and `class` attributes to add semantics that is 
common to a group of consecutive elements. This element can also be used in a `<dl>` tag 
and wrap groups of `<dt>` and `<dd>` elements.

<h5>Example:</h5>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Div Tag Example</title>
    <style>
      div {
        background-color: #87f5b3
      }
    </style>
  </head>
  <body>
    <h1>Example</h1>
    <div>
      <h2>A heading in a <div> tag.</h2>
      <p>Some text in a <div> tag.</p>
    </div>
    <p>Here is some other text in a <p> tag.</p>
  </body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Discuss the differences between an HTML specification and a browser's implementation thereof.</h3>

HTML specifications such as HTML5 define a set of rules that a document must adhere to in 
order to be "valid" according to that specification. In addition, a specification provides 
instructions on how a browser must interpret and render such a document.

A browser is said to "support" a specification if it handles valid documents according to 
the rules of the specification. As of yet, no browser supports all aspects of the HTML5 
specification (although all of the major browser support most of it), and as a result, it 
is necessary for the developer to confirm whether the aspect they are making use of will 
be supported by all of the browsers on which they hope to display their content. This is 
why cross-browser support continues to be a headache for developers, despite the improved 
specificiations.

In addition, while HTML5 defines some rules to follow for an invalid HTML5 document (i.e., 
one that contains syntactical errors), invalid documents may contain anything, and it is 
impossible for the specification to handle all possibilities comprehensively. Thus, many 
decisions about how to handle malformed documents are left up to the browser.

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Why you would use a srcset attribute in an image tag? Explain the process the browser 
used when evaluating the content of this attribute.</h3>

The `srcset` attribute allows to define a list of different image resources along with size 
information so that browser can pick the most appropriate image based on the actual device's 
resolution.

<h5>Syntax:</h5>

```html
<img 
   srcset=" 
      url size, 
      url size, 
      url size " 
   src="default url" 
/>
```

<h4>1. Using display density descriptor:</h4>

`srcset` provides a comma-separated list of image resources along with display density it 
should be used, for example1x, 2x etc.

<h5>Example:</h5>

```html
<img src="image.jpg" 
  srcset="image.jpg,
          image_2x.jpg 2x"
/>
```

<h4>2. Using width descriptor:</h4>

The syntax is similar to the display density descriptor, but instead of display density 
values, we provide the actual width of the image.

<h5>Example:</h5>

```html
<img src="image.jpg" 
  srcset="small.jpg 300w,
          medium.jpg 600w,
          large.jpg 900w"
/>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. What is accessibility & ARIA role means in a web application?</h3>
<p>ARIA is shorthand for Accessible Rich Internet Applications. ARIA is a set of attributes 
you can add to HTML elements that define ways to make web content and applications 
accessible to users with disabilities who use assistive technologies (AT). When accessibility 
issues cannot be managed with native HTML, ARIA can help bridge those gaps.</p>

<p>The <b>Accessible Rich Internet Applications (ARIA)</b> Suite, defines a way to make Web 
content and Web applications more accessible to people with disabilities. It especially 
helps with dynamic content and advanced user interface controls developed with HTML, 
JavaScript, and related technologies.</p>

<p>Screen readers work with regular HTML, but adding ARIA can provide screen reader users 
with greater context and interactivity with the content on the page. ARIA has no effect 
on how elements are displayed or behave in browsers. It does not add new functionality, 
and is meant to act only as an extra descriptive layer for screen readers.</p>

<p>Without WAI-ARIA certain functionality used in Web sites is not available to some users 
with disabilities, especially people who rely on screen readers and people who cannot 
use a mouse. WAI-ARIA addresses these accessibility challenges, for example, by defining 
ways for functionality to be provided to assistive technology. With WAI-ARIA, developers 
can make advanced Web applications accessible and usable to people with disabilities.</p>

<p>ARIA attributes are divided into two categories: roles, and states & properties.</p>

<h4>ARIA Roles:</h4>

<p>An ARIA role is added via a `role="&lt;ROLE TYPE&gt;"` attribute, and does not ever change for 
an element once it is set. There are four categories of ARIA roles:</p>

<ul>
  <li>landmark</li>
  <li>document</li>
  <li>widget</li>
  <li>abstract</li>
</ul>

<h4>Landmark ARIA Roles:</h4>

Much like semantic HTML elements, landmark ARIA Roles are used to give users of assistive 
technology a better way to navigate and identify the different parts of a web page.

<h5>Example:</h5>

```html
 <nav class='mobile-nav' role='navigation' aria-label='Mobile Menu'>List of Links</nav>
```

While seeming redundant, is actually useful for screen readers. It wouldn't read the 
aria-label on this navigation, which is really helpful for giving greater context to 
visually impaired users, without the `role="navigation"`.

The different landmark roles you can use are as follows, copied from the W3C Wiki Page:

<ul>
  <li><b>banner</b>: A region that contains the prime heading or internal title of a page.</li>
  <li>complementary: Any section of the document that supports the main content, yet is 
  separate and meaningful on its own.</li>
  <li><b>contentinfo</b>: A region that contains information about the parent document such as 
  copyrights and links to privacy statements.</li>
  <li><b>form</b>: A region of the document that represents a collection of form-associated 
  elements, some of which can represent editable values that can be submitted to a server 
  for processing.</li>
  <li><b>main</b>: Main content in a document. In almost all cases a page will have only one 
  'role="main"'.</li>
  <li><b>navigation</b>: A collection of links suitable for use when navigating the document or 
  related documents.</li>
  <li><b>search</b>: The search tool of a Web document.</li>
  <li>application: A region declared as a web application, as opposed to a web document.</li>
</ul>

<h4>Document ARIA Roles:</h4>

<p><a href="https://www.digitala11y.com/wai-aria-1-1-cheat-sheet/">Cheat Sheet of ARIA Roles</a>.</p>

<p>Document roles describe the structure of the content on the page, as opposed to the structure 
of the whole page, which landmark roles describe. The roles in bold are the ones we think 
are the most common document aria roles, and the ones which are useful to think about 
including in your HTML.</p>

<ul>
  <li>article: A section of a page that consists of a composition that forms an independent 
  part of a document, page, or site.</li>
  <li>columnheader: Title or header information for the column.</li>
  <li>definition: A definition of a term or concept.</li>
  <li>directory: deprecated in ARIA 1.2. List of references to members of a group, such as a static table of contents.</li>
  <li><b>document</b>: The document role is for focusable content within complex composite widgets or applications for which assistive technologies can swith reading context back to a reading mode.</li>
  <li>group: A set of user interface objects which are not intended to be included in a 
  page summary or table of contents by assistive technologies.</li>
  <li><b>heading</b>: A heading for a section of the page.</li>
  <li><b>img</b>: Can be used to identify multiple elements inside page content that should be considered as a single image.
   These elements could be images, code snippets, text, emojis, or other content that can be combined to deliver information in a visual manner.</li>
  <li><b>list</b>: The ARIA list role can be used to identify a list of items. It is normally used in conjunction with the listitem role, which is used to identify a list item contained inside the list.</li>
  <li><b>listitem</b>: The ARIA listitem role can be used to identify an item inside a list of items. It is normally used in conjunction with the list role, which is used to identify a list container.</li>
  <li>math: The math role indicates that the content represents a mathematical expression.</li>
  <li>note: A note role suggests a section whose content is parenthetic or ancillary to the main content.</li>
  <li>presentation: The presentation role and its synonym none remove an element's implicit ARIA semantics from being exposed to the accessibility tree.</li>
  <li>region: The region role is used to identify document areas the author deems significant. It is a generic landmark available to aid in navigation when none of the other landmark roles are appropriate.</li>
  <li>row: An element with role="row" is a row of cells within a tabular structure. A row contains one or more cells, grid cells or column headers, and possibly a row header, within a grid, table or treegrid, and optionally within a rowgroup.</li>
  <li>rowgroup: An element with role="rowgroup" is a group of rows within a tabular structure. A rowgroup contains one or more rows of cells, grid cells, column headers, or row headers within a grid, table or treegrid.</li>
  <li>rowheader: An element with role="rowheader" is a cell containing header information for a row within a tabular structure of a grid, table or treegrid.</li>
  <li>separator: The separator role indicates the element is a divider that separates and distinguishes sections of content or groups of menuitems. The implicit ARIA role the native thematic break <hr> element is separator.</li>
  <li><b>toolbar</b>: The toolbar role defines the containing element as a collection of commonly used function buttons or controls represented in a compact visual form.</li>
</ul>

<h4>Widget ARIA Roles:</h4>

<p>Widget Roles are used to describe what are often javascript-based interfaces, or the more 
complicated parts of your web page's interface. The roles that are starred are the ones 
we think are the most common elements widget aria roles, and the ones which are useful 
useful to think about including in your HTML.</p>

<ul>
  <li><b>alert</b>: A message with important, and usually time-sensitive, information.</li>
  <li>alertdialog: A type of dialog that contains an alert message, where initial focus 
    goes to an element within the dialog.</li>
  <li><b>button</b>: An input that allows for user-triggered actions when clicked or pressed.</li>
  <li><b>checkbox</b>: A checkable input that has three possible values: true, false, or mixed.</li>
  <li>dialog: A dialog is an application window that is designed to interrupt the current 
    processing of an application in order to prompt the user to enter information or require 
	a response.</li>
  <li>gridcell</li>
  <li><b>link</b></li>
  <li>log</li>
  <li>marquee</li>
  <li><b>menuitem</b></li>
  <li>menuitemcheckbox</li>
  <li>menuitemradio</li>
  <li>option</li>
  <li>progressbar</li>
  <li>radio: A checkable input in a group of radio roles, only one of which can be 
    checked at a time.</li>
  <li>scrollbar</li>
  <li>slider</li>
  <li>spinbutton</li>
  <li>status</li>
  <li><b>tab</b>: A grouping label providing a mechanism for selecting the tab content that is 
  to be rendered to the user.</li>
  <li><b>tabpanel</b>: A container for the resources associated with a tab, where each tab is 
  contained in a tablist.</li>
  <li>textbox: Input that allows free-form text as its value.</li>
  <li>timer</li>
  <li>tooltip</li>
  <li>treeitem</li>
</ul>

<h4>Abstract ARIA Roles:</h4>

<p>Abstract aria roles are the basis of how the other ARIA roles are defined. These are not 
to be used in HTML.</p>

<h4>ARIA States & Properties:</h4>

<p>ARIA states and properties are often used to support ARIA roles that exist on a page. 
ARIA Properties often describe relationships with other elements, and for the most part, 
do not change once they're set.</p>

<p>ARIA States are more dynamic and are typically updated with JavaScript as a user interacts 
with a page. Screen readers are notified when these states change, and can announce these 
changes to users after an interaction takes place.</p>

<p>While there are 35 aria properties and states the W3C defines and which you can read more 
about on the W3C site, here are the ones we believe to most commonly used and practical 
for most web pages/applications.</p>

<ul>
  <li>aria-activedescendant: Identifies the currently active descendant of a composite 
    widget. Use with autofill search suggestions.</li>
  <li>aria-autocomplete: Indicates whether user input completion suggestions are provided. 
    Use with autofill search suggestions.</li>
  <li>aria-checked (state): Indicates the current “checked” state of checkboxes, radio 
    buttons, and other widgets. You can set this to true, false, or mixed state.</li>
  <li>aria-controls: Identifies the element (or elements) whose contents or presence are 
  controlled by the current element.</li>
  <li><b>aria-describedby</b>: Identifies the element (or elements) that describes the object.</li>
  <li>aria-disabled (state): Indicates that the element is perceivable but disabled, so 
  it is not editable or otherwise operable.</li>
  <li>aria-expanded (state): Indicates whether the element, or another grouping element 
    it controls, is currently expanded or collapsed.</li>
  <li><b>aria-haspopup</b>: </li>
  <li><b>aria-hidden (state)</b>: Indicates that the element and all of its descendants are 
    not visible or perceivable to any user as implemented by the author.</li>
  <li>aria-invalid (state): Indicates the entered value does not conform to the format 
    expected by the application.</li>
  <li><b>aria-label</b>: Defines a string value that labels the current element.</li>
  <li><b>aria-labelledby</b>: Identifies the element (or elements) that labels the current element.</li>
  <li>aria-live: Indicates that an element is dynamic, changing, and will be updated, 
    and describes the types of updates the user can expect from the live region.</li>
  <li>aria-owns: Identifies an element (or elements) in order to define a visual, 
    functional, or contextual parent/child  relationship between DOM elements where the 
	DOM hierarchy cannot be used to represent the relationship.</li>
  <li>aria-pressed (state): Indicates the current “pressed” state of toggle buttons.</li>
  <li>aria-required: Indicates that user input is required on the element before a form 
    may be submitted.</li>
  <li><b>aria-selected (state)</b>: Indicates the current “selected” state of various widgets.</li>
</ul>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h3>Q. Create a traffic signal light in html?</h3>

<details>
  <summary>html</summary>

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Traffic Signal
    </title>
    <style>
      #green {
        background-color: green;
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 2px solid #333;
      }
      #yellow{
        background-color: yellow;
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 2px solid #333;
      }
      #red{
        background-color: red;
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 2px solid #333;
      }
    </style>
  </head>
  <body onload="timer;">
    <div id="red"></div>
    <div id="yellow"></div>
    <div id="green"></div>
      
    <script>
      function startTrafficSignal() {
        
        const red = document.getElementById("red");
        const yellow = document.getElementById("yellow");
        const green = document.getElementById("green");
      
        green.style.opacity = 1;
      
        // Red Signal
        setTimeout(function () {
          green.style.opacity = 0.3;
          red.style.opacity = 1;
          yellow.style.opacity = 0.3;
        }, 7000);
        
        // Yellow Signal
        setTimeout(function () {
          green.style.opacity = 1;
          red.style.opacity = 0.3;
          yellow.style.opacity = 0.3;
        }, 5000);
        
        // Green Signal
        setTimeout(function () {
          green.style.opacity = 0.3;
          red.style.opacity = 0.3;
          yellow.style.opacity = 1;
        }, 12000);
      }

      const timer = setInterval(function () {
        startTrafficSignal();
      }, 12000);
      
      startTrafficSignal();
    </script>
  </body>
</html>
```

</details>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="03-html-events">03. HTML Events</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3>Types of Events</h3>

<h4>There are muliple types; Window, Form, Keyboard, Mouse, Drag, Clipboard, 
Media, &amp; Miscellaneous.</h4>

<h4 id="global-events">Global Event Attributes</h4>
HTML has the ability to let events trigger actions in a browser, like starting a JavaScript 
when a user clicks on an element.

<p>Below are the global event attributes that can be added to HTML elements to define event actions.</p>

<h4 id="window-events">Window Event Attributes</h4>
<p>Events triggered for the window object (applies to the &lt;body&gt; tag):</p>

| Attribute      | Value  | Description |
|----------------|--------|--------------------------------------------------------------------------|
| onafterprint   | script | Script to be run after the document is printed |
| onbeforeprint  | script | Script to be run before the document is printed |
| onbeforeunload | script | Script to be run when the document is about to be unloaded |
| onerror        | script | Script to be run when an error occurs |
| onhashchange   | script | Script to be run when there has been changes to the anchor part of the a URL |
| onload         | script | Fires after the page is finished loading |
| onmessage      | script | Script to be run when the message is triggered |
| onoffline      | script | Script to be run when the browser starts to work offline |
| ononline       | script | Script to be run when the browser starts to work online |
| onpagehide     | script | Script to be run when a user navigates away from a page |
| onpageshow     | script | Script to be run when a user navigates to a page |
| onpopstate     | script | Script to be run when the window's history changes |
| onresize       | script | Fires when the browser window is resized |
| onstorage      | script | Script to be run when a Web Storage area is updated |
| onunload       | script | Fires once a page has unloaded (or the browser window has been closed) |

<h4 id="form-events">Form Events</h4>
<p>Events triggered by actions inside a HTML form (applies to almost all HTML elements, but is most used in form elements):</p>

| Attribute      | Value  | Description |
|----------------|--------|--------------------------------------------------------------------------|
| onblur         | script | Fires the moment that the element loses focus |
| onchange       | script | Fires the moment when the value of the element is changed |
| oncontextmenu  | script | Script to be run when a context menu is triggered |
| onfocus        | script | Fires the moment when the element gets focus |
| oninput        | script | Script to be run when an element gets user input |
| oninvalid      | script | Script to be run when an element is invalid |
| onreset        | script | Fires when the Reset button in a form is clicked |
| onsearch       | script | Fires when the user writes something in a search field (for &lt;input="search"&gt;) |
| onselect       | script | Fires after some text has been selected in an element |
| onsubmit       | script | Fires when a form is submitted |

<h4 id="keyboard-events">Keyboard Events</h4>

| Attribute  | Value  | Description |
|------------|--------|--------------------------------------------------------------------------|
| onkeydown  | script | Fires when a user is pressing a key |
| onkeypress | script | Fires when a user presses a key |
| onkeyup    | script | Fires when a user releases a key |

<h4 id="mouse-events">Mouse Events</h4>

| Attribute    | Value  | Description |
|--------------|--------|--------------------------------------------------------------------------|
| onclick      | script | Fires on a mouse click on the element |
| ondblclick   | script | Fires on a mouse double-click on the element |
| onmousedown  | script | Fires when a mouse button is pressed down on an element |
| onmousemove  | script | Fires when the mouse pointer is moving while it is over an element |
| onmouseout   | script | Fires when the mouse pointer moves out of an element |
| onmouseover  | script | Fires when the mouse pointer moves over an element |
| onmouseup    | script | Fires when a mouse button is released over an element |
| onmousewheel | script | Deprecated. Use the onwheel attribute instead |
| onwheel      | script | Fires when the mouse wheel rolls up or down over an element |

<h4 id="drag-events">Drag Events</h4>

| Attribute    | Value  | Description |
|--------------|--------|--------------------------------------------------------------------------|
| ondrag       | script | Script to be run when an element is dragged |
| ondragend    | script | Script to be run at the end of a drag operation |
| ondragenter  | script | Script to be run when an element has been dragged to a valid drop target |
| ondragleave  | script | Script to be run when an element leaves a valid drop target |
| ondragover   | script | Script to be run when an element is being dragged over a valid drop target |
| ondragstart  | script | Script to be run at the start of a drag operation |
| ondrop       | script | Script to be run when dragged element is being dropped |
| onscroll     | script | Script to be run when an element's scrollbar is being scrolled |

<h4 id="clipboard-events">Clipboard Events</h4>

| Attribute       | Value    | Description |
|----------------|--------|--------------------------------------------------------------------------|
| oncopy    | script  |   Fires when the user copies the content of an element |
| oncut    | script    | Fires when the user cuts the content of an element |
| onpaste  |   script   |  Fires when the user pastes some content in an element |

<h4 id="media-events">Media Events</h4>

<p>Events triggered by medias like videos, images and audio (applies to all HTML 
elements, but is most common in media elements, like &lt;audio&gt;, &lt;embed&gt;, &lt;img&gt;, 
&lt;object&gt;, and &lt;video&gt;).</p>

|Attribute       |Value    |Description |
|----------------|--------|--------------------------------------------------------------------------|
| onabort    | script | Script to be run on abort |
| oncanplay    | script | Script to be run when a file is ready to start playing (when it has buffered enough to begin) |
| oncanplaythrough | script | Script to be run when a file can be played all the way to the end without pausing for buffering |
| oncuechange    | script | Script to be run when the cue changes in a <track> element |
| ondurationchange | script | Script to be run when the length of the media changes |
| onemptied   | script  | Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects) |
| onended    | script  | Script to be run when the media has reach the end (a useful event for messages like "thanks for listening") |
| onerror    | script  | Script to be run when an error occurs when the file is being loaded |
| onloadeddata  | script | Script to be run when media data is loaded |
| onloadedmetadata | script | Script to be run when meta data (like dimensions and duration) are loaded |
| onloadstart    | script  | Script to be run just as the file begins to load before anything is actually loaded |
| onpause  | script | Script to be run when the media is paused either by the user or programmatically |
| onplay   | script  | Script to be run when the media is ready to start playing |
| onplaying  | script | Script to be run when the media actually has started playing |
| onprogress   | script  | Script to be run when the browser is in the process of getting the media data |
| onratechange   | script | Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode) |
| onseeked   | script  | Script to be run when the seeking attribute is set to false indicating that seeking has ended |
| onseeking   | script   | Script to be run when the seeking attribute is set to true indicating that seeking is active |
| onstalled  | script | Script to be run when the browser is unable to fetch the media data for whatever reason |
| onsuspend | script   | Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason |
| ontimeupdate | script  | Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media) |
| onvolumechange | script | Script to be run each time the volume is changed which (includes setting the volume to "mute") |
| onwaiting   | script  | Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data) |

<h4 id="misc-events">Misc Events</h4>

|Attribute       |Value    |Description |
|----------------|--------|-----------------------------------------------------------|
| ontoggle | script | Fires when the user opens or closes the &lt;details&gt; element |

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="04-html-forms">04. HTML Form Elements</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>The HTML &lt;form&gt; comprises several elements, each serving a unique purpose. For 
instance, the &lt;label&gt; element is used to define labels for other &lt;form&gt; elements. 
The &lt;input&gt; element, on the other hand, is versatile and can be used to capture 
various types of input data such as text, password, email, and more, simply by 
altering its type attribute. Now, let’s all the list of HTML Form Elements one 
by one:</p>

| Elements     | Descriptions |
|----------|----------------------------------------------------------------------------------|
| &lt;label&gt;    | It defines labels for &lt;form&gt; elements. |
| &lt;input&gt;    | It is used to get input data from the form in various types such as text, password, email, etc by changing its type. |
| &lt;button&gt;   | It defines a clickable button to control other elements or execute a functionality. |
| &lt;select&gt;   | It is used to create a drop-down list. |
| &lt;textarea&gt; | It is used to get input long text content. |
| &lt;fieldset&gt; | It is used to draw a box around other form elements and group the related data. |
| &lt;legend&gt;     | It defines a caption for fieldset elements. |
| &lt;datalist&gt; | It is used to specify pre-defined list options for input controls. |
| &lt;output&gt;     | It displays the output of performed calculations. |
| &lt;option&gt;     | It is used to define options in a drop-down list. |
| &lt;optgroup&gt; | It is used to define group-related options in a drop-down list. |

<h3>Commonly Used Input Types in HTML Forms</h3>

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<p>In HTML forms, various input types are used to collect different types of 
data from users. Here are some commonly used input types:</p>

| Input Type | Description |
|------------|------------------------------------------------------------------------------------|
| &lt;input type="text"&gt; | Defines a one-line text input field |
| &lt;input type="password"&gt;   | Defines a password field |
| &lt;input type="submit"&gt;     | Defines a submit button |
| &lt;input type="reset"&gt;      | Defines a reset button |
| &lt;input type="radio"&gt;      | Defines a radio button |
| &lt;input type="email"&gt;      | Validates that the input is a valid email address. |
| &lt;input type="number"&gt;     | Allows the user to enter a number. You can specify min, max, and step attributes for range. |
| &lt;input type="checkbox"&gt;   | Used for checkboxes where the user can select multiple options. |
| &lt;input type="date"&gt;       | Allows the user to select a date from a calendar. |
| &lt;input type="time"&gt;       | Allows the user to select a time. |
| &lt;input type="file"&gt;       | Allows the user to select a file to upload. |

<h3>HTML Forms Examples</h3>

<h4>1. Basic HTML Forms Example:</h4>

<p><b>Example:</b> This HTML forms collects the user personal information such 
as username and password with the button to submit the form.</p>

```
<!DOCTYPE html>
<html lang="en">
<head>
<title>Html Forms</title>
</head>
<body>
  <h2>HTML Forms</h2>
  <form>
    <label for="username">Username:</label><br>
    <input type="text" id="username" name="username"><br><br>
    
    <label for="password">Password:</label><br>
    <input type="password" id="password" name="password"><br><br>
    
    <input type="submit" value="Submit">
  </form>
</body> 
</html>
```

<h5>Output:</h5>

<!-- image 2 -->

<h4>2. HTML Forms Example:</h4>

<p><b>Example:</b> This HTML form collects user personal information including 
name, email, password, gender, date of birth, and address. It features proper 
styling for input fields and submission button.</p>

```
<!DOCTYPE html>
<html>
  <head>
    <title>HTML Form</title>
    <style>
      body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        background-color: #f0f0f0;
      }

      form {
        width: 400px;
        background-color: #fff;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px
        rgba(0, 0, 0, 0.1);
      }

      fieldset {
        border: 1px solid black;
        padding: 10px;
        margin: 0;
      }

      legend {
        font-weight: bold;
        margin-bottom: 10px;
      }

      label {
        display: block;
        margin-bottom: 5px;
      }

      input[type="text"],
      input[type="email"],
      input[type="password"],
      textarea,
      input[type="date"] {
        width: calc(100% - 20px);
        padding: 8px;
        margin-bottom: 10px;
        box-sizing: border-box;
        border: 1px solid #ccc;
        border-radius: 4px;
      }

      input[type="radio"] {
        margin-left: 20px;
      }

      input[type="submit"] {
        padding: 10px 20px;
        border-radius: 5px;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <form>
      <fieldset>
        <legend>
          User personal information
        </legend>
        <label>
          Enter your full name
        </label>
        <input type="text" name="name" />
        <label>Enter your email</label>
        <input
          type="email"
          name="email"
        />
        <label>Enter your password</label>
        <input
          type="password"
          name="pass"
        />
        <label>Confirm your password</label>
        <input
          type="password"
          name="confirmPass"
        />
        <label>Enter your gender</label>
        <input
          type="radio"
          name="gender"
          value="male"
        />Male
        <input
          type="radio"
          name="gender"
          value="female"
        />Female
        <input
          type="radio"
          name="gender"
          value="others"
        />Others
        <label>Enter your Date of Birth</label>
        <input type="date" name="dob" />
        <label>Enter your Address:</label>
        <textarea
          name="address">
        </textarea>
        <input
          type="submit"
          value="submit"
        />
      </fieldset>
    </form>
  </body>
</html>
```

<!-- form 3 -->

<p>Here are some of the key attributes that can be used with the &lt;form&gt; element:</p>

<ol>
  <li>action: This attribute specifies where to send the form-data when a form 
    is submitted. The value of this attribute is typically a URL.</li>
  <li>method: This attribute defines the HTTP method used to send the form-data. 
    The values can be “get” or “post”.</li>
  <li>target: This attribute specifies where to display the response received after 
    submitting the form. The values can be “_blank”, “_self”, “_parent”, “_top”, or 
    the name of an iframe.</li>
  <li>enctype: This attribute is used when method=“post”. It specifies how the form-
    data should be encoded when submitting it to the server. The values can be 
    “application/x-www-form-urlencoded”, “multipart/form-data”, or “text/plain”.</li>
  <li>autocomplete: This attribute specifies whether a form should have autocomplete 
    on or off. When autocomplete is on, the browser automatically completes values 
    based on values that the user has entered before.</li>
  <li>novalidate: This Boolean attribute specifies that the form-data should not 
    be validated on submission.</li>
</ol>

<h4>Features</h4>

<ul>
  <li>Facilitates user input collection through various elements.</li>
  <li>Utilizes <form> tags to structure input elements.</li>
  <li>Defines actions for data submission upon form completion.</li>
  <li>Supports client-side validation for enhanced user experience.</li>
</ul>

<h4>Conclusion</h4>

<p>In conclusion, HTML forms are a powerful tool for collecting user input on 
the web. They provide a wide range of interactive controls, from text fields 
to checkboxes, radio buttons, and more. Understanding the syntax and attributes 
of the <form> element is crucial for creating effective and user-friendly forms.</p>

<p>This article has provided a comprehensive overview of HTML forms, including their 
syntax, key attributes, and various form elements. By mastering HTML forms, you 
can create more engaging, user-friendly, and accessible web applications.</p>
<!- end of html-forms -->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="05-html-tables">05. HTML Tables</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3>What is an HTML Table?</h3>

<p>An HTML Table is an arrangement of data in rows and columns in tabular format. 
Tables are useful for various tasks, such as presenting text information and 
numerical data. A table is a useful tool for quickly and easily finding connections 
between different types of data. Tables are also used to create databases.</p>

<h3>HTML Table Code Example</h3>

```
<!-- index.html -->
<!DOCTYPE html>
<html>
<body>
  <table>
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>
```

<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>

<h4>Output</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-01. simple html table ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image001.png"
  title="Simple HTML table"
  alt="Simple HTML table."
  style="width:40%" >
</p>  

<h3>Tags used in HTML Tables</h3>

| HTML Tags    | Descriptions |
|--------------|-------------------------------------------------------------------------------------|
| &lt;table&gt; | Defines the structure for organizing data in rows and columns within a web page. |
| &lt;tr&gt;    | Represents a row within an HTML table, containing individual cells. |
| &lt;th&gt;    | Shows a table header cell that typically holds titles or headings. |
| &lt;td&gt;    | Represents a standard data cell, holding content or data. |
| &lt;caption&gt;    | Provides a title or description for the entire table. |
| &lt;thead&gt;    | Defines the header section of a table, often containing column labels. |
| &lt;tbody&gt;    | Represents the main content area of a table, separating it from the header or footer. |
| &lt;tfoot&gt;    | Specifies the footer section of a table, typically holding summaries or totals. |
| &lt;col&gt;    | Defines attributes for table columns that can be applied to multiple columns at once. |
| &lt;colgroup&gt; |    Groups together a set of columns in a table to which you can apply formatting or properties collectively. |

<h3>Defining Tables in HTML</h3>

<p>An HTML table is defined with the "table" tag. Each table row is defined with 
the "tr" tag. A table header is defined with the "th" tag. By default, table 
headings are bold and centered. A table data/cell is defined with the "td" tag.</p>

<h4>Table Cells</h4>
<p>Table Cell are the building blocks for defining the Table. It is denoted with 
&lt;td&gt; as a start tag &amp; &lt;/td&gt; as a end tag.</p>

<h5>Syntax</h5>

```
</td> Content...</td> 
```

<h4>Table Rows</h4>
<p>The rows can be formed with the help of combination of Table Cells. It is 
denoted by &lt;tr&gt; and &lt;/tr&gt; tag as a start & end tags.</p>

<h5>Syntax</h5>

```
<tr>Content...</tr> 
```

<h4>Table Headers</h4>
The Headers are generally use to provide the Heading. The Table Headers can also be used 
to add the heading to the Table. This contains the <th> & </th> tags.

<h5>Syntax</h5>

```
<th>Content...</th> 
```

<p><b>Example 1:</b> Creating a simple table in HTML using a table tag.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<body>
  <table>
    <tr>
      <th>Book Name</th>
      <th>Author Name</th>
      <th>Genre</th>
    </tr>
    <tr>
      <td>The Book Thief</td>
      <td>Markus Zusak</td>
      <td>Historical Fiction</td>
    </tr>
    <tr>
      <td>The Cruel Prince</td>
      <td>Holly Black</td>
      <td>Fantasy</td>
    </tr>
    <tr>
      <td>The Silent Patient</td>
      <td> Alex Michaelides</td>
      <td>Psychological Fiction</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-02. html table ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image002.png"
  title="HTML table"
  alt="HTML table."
  style="width:40%" >
</p>

<h4>Adding a border to an HTML Table</h4>
<p>A border is set using the CSS border property. If you do not specify a border 
for the table, it will be displayed without borders.</p>

<h5>Syntax</h5>

```
table, th, td {
      border: 1px solid black;
}
```

<p><b>Example:</b> Addition of the border to the HTML Table.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-03. table with border ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image003.png"
  title="Table with border"
  alt="Table with border."
  style="width:40%" >
</p>

<h4>Adding Collapsed Borders in an HTML Table</h4>
<p>For borders to collapse into one border, add the CSS border-collapse property.</p>

<h5>Syntax</h5>

```
  table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
  }
```

<p><b>Example:</b> Addition of Collapsed Borders in HTML.</p>


```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-04. table with collapsed borders ~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image004.png"
  title="Table with collapsed borders"
  alt="Table with collapsed borders."
  style="width:40%" >
</p>

<h4>Adding Cell Padding in an HTML Table</h4>
<p>Cell padding specifies the space between the cell content and its borders. If 
we do not specify a padding, the table cells will be displayed without padding.</p>

<h5>Syntax</h5>

```
th, td {
  padding: 20px;
}
```

<p><b>Example:</b> Addition of Table cell padding in HTML.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }
    
    th,
    td {
      padding: 20px;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-05. adding table cell padding ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image005.png"
  title="Adding table cell padding"
  alt="Adding table cell padding."
  style="width:40%" >
</p>

<h4>Adding Left Align Headings in an HTML Table</h4>
<p>By default, the table headings are bold and centered. To left-align the table 
headings, we must use the CSS text-align property.</p>

<h5>Syntax</h5>

```
th {
  text-align: left;
}
```

<p><b>Example:</b> Explains the text-align property where the text is aligned to the left.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 20px;
    }

    th {
      text-align: left;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-06. text-align property ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image006.png"
  title="text-align property"
  alt="text-align property."
  style="width:40%" >
</p>

<h4>Adding Border Spacing in an HTML Table</h4>

<p>Border spacing specifies the space between the cells. To set the border-spacing 
for a table, we must use the CSS border-spacing property.</p>

<h5>Syntax</h5>

```
table {
  border-spacing: 5px;
}
```

<p><b>Example:</b> Explains the border space property to make the space between the Table cells.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
    }

    table {
      border-spacing: 5px;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-07. border spacing property ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image007.png"
  title="Border spacing property"
  alt="Border spacing property."
  style="width:40%" >
</p>

<h4>Adding Cells that Span Many Columns in HTML Tables</h4>
<p>To make a cell span more than one column, we must use the colspan attribute.</p>

<p><b>Example:</b> Use of colspan attribute in HTML.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 5px;
      text-align: left;
    }
  </style>
</head>

<body>
  <h2>Cell that spans two columns:</h2>
  <table style="width:100%">
    <tr>
      <th>Name</th>
      <th colspan="2">Telephone</th>
    </tr>
    <tr>
      <td>Vikas Rawat</td>
      <td>9125577854</td>
      <td>8565557785</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-08. use of colspan attribute ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image008.png"
  title="Use of colspan attribute"
  alt="Use of colspan attribute."
  style="width:40%" >
</p>

<h4>Adding Cells that span many rows in HTML Tables</h4>
<p>To make a cell span more than one row, we must use the rowspan attribute.</p>

<p><b>Example:</b> Use of the rowspan attribute in HTML.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 5px;
      text-align: left;
    }
  </style>
</head>

<body>
  <h2>Cell that spans two rows:</h2>
  <table style="width:100%">
    <tr>
      <th>Name:</th>
      <td>Vikas Rawat</td>
    </tr>
    <tr>
      <th rowspan="2">Telephone:</th>
      <td>9125577854</td>
    </tr>
    <tr>
      <td>8565557785</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-09. use of rowspan attribute ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image009.png"
  title="Use of rowspan attribute"
  alt="Use of rowspan attribute."
  style="width:40%" >
</p>

<h4>Adding a Caption in an HTML Table</h4>

<p>To add a caption to a table, we must use the "caption" tag.</p>

<h5>Syntax</h5>

```
<table style="width:100%">
<caption>DETAILS</caption>
```

<p><b>Example:</b> HTML Table caption by specifying the CSS properties for setting its width.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 20px;
    }

    th {
      text-align: left;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <caption>DETAILS</caption>
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-10. adding caption using the tag ~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image010.png"
  title="Adding Caption using the Tag"
  alt="Adding Caption using the Tag."
  style="width:40%" >
</p>

<h4>Adding a Background Colour to the Table</h4>
<p>A color can be added as a background in an HTML table using the "background-
color" option.</p>

<h5>Syntax</h5>

```
table#t01 {
  width: 100%;
  background-color: #f2f2d1;
}
```

<p><b>Example:</b> Addition of the Table background color in HTML.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
  <style>
    table,
    th,
    td {
      border: 1px solid black;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 5px;
      text-align: left;
    }

    table#t01 {
      width: 100%;
      background-color: #f2f2d1;
    }
  </style>
</head>

<body>
  <table style="width:100%">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
  <br />
  <br />
  <table id="t01">
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
      <th>Age</th>
    </tr>
    <tr>
      <td>Priya</td>
      <td>Sharma</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Arun</td>
      <td>Singh</td>
      <td>32</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>Watson</td>
      <td>41</td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-11. adding background color ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image011.png"
  title="Adding Background Color"
  alt="Adding Background Color."
  style="width:40%" >
</p>

<h4>Creating Nested Tables</h4>
<p>Nesting tables simply means making a Table inside another Table. Nesting tables 
can lead to complex tables layouts, which are visually interesting and have the 
potential of introducing errors.</p>

<p><b>Example:</b> Nesting of HTML Table.</p>

```
<!-- index.html -->
<!DOCTYPE html>
<html>

<body>
  <table border=5 bordercolor=black>
    <tr>
      <td>First Column of Outer Table</td>
      <td>
        <table border=5 bordercolor=grey>
          <tr>
            <td>First row of Inner Table</td>
          </tr>
          <tr>
            <td>Second row of Inner Table</td>
          </tr>
        </table>
      </td>
    </tr>
  </table>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 05-12. nested html table ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/05-image012.png"
  title="Nested HTML table"
  alt="Nested HTML table."
  style="width:40%" >
</p>

<!-- end of html tables -->

<h2 id="06-html-lists">06. HTML Lists</h2>
<p>An HTML list is a record of related information used to display the data or 
any information on web pages in the ordered or unordered form.</p>

<h3>HTML List Example</h3>

<h4>Basic Implementation of HTML lists.</h4>

```
<!DOCTYPE html>
<html>

<head>
  <title>GeeksforGeeks</title>
</head>

<body>
  <h2>Welcome To GeeksforGeeks Learning</h2>
  <h5>List of available courses</h5>
  <ul>
    <li>Data Structures & Algorithm</li>
    <li>Web Technology</li>
    <li>Aptitude & Logical Reasoning</li>
    <li>Programming Languages</li>
  </ul>
  <h5>Data Structures topics</h5>
  <ol>
    <li>Array</li>
    <li>Linked List</li>
    <li>Stacks</li>
    <li>Queues</li>
    <li>Trees</li>
    <li>Graphs</li>
  </ol>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 06-01. html list ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/06-image001.png"
  title="HTML List"
  alt="HTML List."
  style="width:40%" >
</p>

<h3>There are three types of lists in HTML:</h3>

<h4>Table of Content</h4>

<ol type="1">
  <li>HTML Unordered List or Bulleted List</li>
  <li>HTML Ordered List</li>
  <li>HTML Description List</li>
</ol>

<h3>HTML List Tags</h3>
<p>Here is the list of all lists tags HTML:</p>

| Tag | Description |
|------|----------------------------------------|
| `<ul>` | Defines an unordered list |
| `<ol>` | Defines an ordered list |
| `<li>` | Defines a list item |
| `<dl>` | Defines a description list |
| `<dt>` | Defines a term in a description list |
| `<dd>` | Details the term in a description list |

<h3>The HTML Unordered List or Bulleted List</h3>

<p>The unordered list items are marked with bullets. It is also known as bulleted 
lists. An unordered list starts with the &lt;ul&gt; tag. Each list item starts with the 
&lt;li&gt; tag.</p>

<h5>Syntax:</h5>

```
<ul>list of items</ul>
```

<p><b>Attribute:</b> This tag contains two attributes which are listed below:</p>

<ul>
  <li>compact: It will render the list smaller.</li>
  <li>type: It specifies which kind of marker is used in the list.</li>
</ul>

<p><b>Example:</b> This example describes the unordered list.</p>

```
<!DOCTYPE html>
<html>

<body>
  <h2>Grocery list</h2>
  <ul>
    <li>Bread</li>
    <li>Eggs</li>
    <li>Milk</li>
    <li>Coffee</li>
  </ul>
</body>

</html>
```

<h4>Output:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 06-02. unordered list ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/06-image002.png"
  title="Unordered List"
  alt="Unordered List."
  style="width:40%" >
</p>

<h3>HTML Ordered List</h3>

<p>In an ordered list, all list items are marked with numbers by default. An 
ordered list starts with the &lt;ol&gt; tag. Each list item starts with the 
"li" tag.</p>

<h4>Syntax:</h4>

```
<ol>
   <li>Item1</li>
   <li>Item2</li>
   <li>Item3</li>
</ol>
```

<h4>Attributes:</h4>

<ul>
  <li>compact: It defines the list should be compacted (compact attribute is not 
    supported in HTML5. Use CSS instead.).</li>
  <li>reversed: It defines that the order will be descending.</li>
  <li>start: It defines from which number or alphabet the order will start.</li>
  <li>type: It defines which type(1, A, a, I, and i) of the order you want in 
    your list of numeric, alphabetic, or roman numbers.</li>
</ul>

<p><b>Example:</b> This example illustrates the use of the reverse attribute, 
control list counting & type attribute.</p>

```
<!DOCTYPE html>
<html>

<head>
  <title>HTML ol tag</title>
</head>

<body>
  <h1 style="color: green">GeeksforGeeks</h1>
  <h3>HTML ol tag</h3>
    
<p>reversed attribute</p>

  <ol reversed>
    <li>HTML</li>
    <li>CSS</li>
    <li>JS</li>
  </ol>
    
<p>start attribute</p>

  <ol start="5">
    <li>HTML</li>
    <li>CSS</li>
    <li>JS</li>
  </ol>
    
<p>type attribute</p>

  <ol type="i">
    <li>HTML</li>
    <li>CSS</li>
    <li>JS</li>
  </ol>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~ 06-03. ordered list with different list style ~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/06-image003.png"
  title="Ordered list with different list style"
  alt="Ordered list with different list style."
  style="width:40%" >
</p>

<h3>HTML Description List</h3>

<p>A description list is a list of terms, with a description of each term. The 
&lt;dl&gt; tag defines the description list, the &lt;dt&gt; tag defines the term name, 
and the &lt;dd&gt; tag describes each term.</p>

<h5>Syntax:</h5>

```
<dl>Contents...</dl>
```

<p>Please refer to the <i>How to add description list of an element using HTML? 
article</i> for further details.</p>

<p><b>Example:</b> This example describes the HTML Description List.</p>

```
<!DOCTYPE html>
<html>

<body>
  <h2>A Description List</h2>
  <dl> 
    <dt>Coffee</dt>
    <dd>- 500 gms</dd>
    <dt>Milk</dt>
    <dd>- 1 ltr Tetra Pack</dd>
  </dl>
</body>

</html>
```

<h5>Output:</h5>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 06-04. description list ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
<img class="displayed"
  src="./images/06-image004.png"
  title="Description list"
  alt="Description list."
  style="width:40%" >
</p>

<h4>Conclusion</h4>

<p>HTML lists provide a way to display a structured collection of items. In this 
tutorial, we have explained three types of lists- ordered lists, unordered lists, 
and definition list. We have explained all three list types with examples.</p>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="07-html-iframes">07. HTML iFrames</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!DOCTYPE html>
<html>
<body>

<h2>Remove the Iframe Border</h2>
<p>To remove the default border of the iframe, use CSS:</p>

```
<iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>
```

</body>
</html>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="08-html-url">08. HTML URL</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
A Uniform Resource Locator (URL) is simply the address of a website to access the website 
content like www.geeksforgeeks.org. But certain characters are allowed to be used in the 
URL like alphabets A-Z and a-z, numbers 0-9, and a few special characters. They can be 
used as it is but the rest of the characters that are not in this list are used after 
encoding them to a suitable form. URL Encoding is the process of converting the URL into 
a valid format that is accepted by web browsers. 

URL Encoding takes place by replacing all the characters that are not allowed by a % sign 
followed by two hexadecimal digits. These two hexadecimal values represent the numerical 
values of the character in the ASCII character set. For example, a space is not acceptable 
in a URL and is replaced by a ‘%20’ or a ‘+’ sign while encoding. Similarly, a $ sign is 
replaced by ‘%24’. 

Syntax:
A web address follows these syntax rules:

scheme://prefix.domain:port/path/filename

<!-- Example -->

<a href="https://www.geeksforgeeks.org/">Example Geeks for Geeks</a>
Scheme: It specifies the protocol used for communication, such as “https://” for secure 
communication or “http://” for unsecured communication.
Prefix: It is an optional subdomain or www indicating the location of the resource within the domain.
Domain: Identifies the website’s primary address, like “example.com”, indicating its unique 
location on the Internet.
Port: Optional and signifies a specific endpoint for communication. Common values are 80 for 
HTTP and 443 for HTTPS.
Path:It specifies the location or directory on the server where the resource is located.
Filename: It refers to the specific file or resource within the specified path.
Table of Content

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="09-html-svg">09. HTML SVG</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="10-html-canvas">10. HTML Canvas</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="11-html-storage">11. HTML Storage</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="12-html-apis">12. HTML APIs</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="13-html-dragndrop">13. HTML Drag 'n Drop</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="14-html-webworker">14. HTML Web Worker</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="15-html-access">15. HTML Accessibility</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="16-misc">16. Miscellaneous</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<div align="right">
  <b><a href="#toc">↥ back to top</a></b>
</div>



