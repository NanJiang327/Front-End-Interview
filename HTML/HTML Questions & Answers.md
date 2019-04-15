## HTML Questions & Answers

* [What does a doctype do?](#what-does-a-doctype-do)
* [How do you serve a page with content in multiple languages?](#how-do-you-serve-a-page-with-content-in-multiple-languages)
* [What are `data-` attributes good for?](#what-are-data--attributes-good-for)
* [Consider HTML5 as an open web platform. What are the building blocks of HTML5?](#consider-html5-as-an-open-web-platform-what-are-the-building-blocks-of-html5)
* [Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.](#describe-the-difference-between-a-cookie-sessionstorage-and-localstorage)
* [Describe the difference between `<script>`, `<script async>` and `<script defer>`.](#describe-the-difference-between-script-script-async-and-script-defer)
* [Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?](#why-is-it-generally-a-good-idea-to-position-css-links-between-headhead-and-js-scripts-just-before-body-do-you-know-any-exceptions)
* [What is progressive rendering?](#what-is-progressive-rendering)
* [Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.](#why-you-would-use-a-srcset-attribute-in-an-image-tag-explain-the-process-the-browser-uses-when-evaluating-the-content-of-this-attribute)
* [Have you used different HTML templating languages before?](#have-you-used-different-html-templating-languages-before)

---

### What does a DOCTYPE do?
#### Simple answer 
==It specifies which markup standard the page is using. With the information, the browser determines how to render the page according to the page's source code.==
#### Details
DOCTYPE is an abbreviation for Document TYPE.
A DOCTYPE is always associated to a DTD - for Document Type Definition.

A DTD defines how documents of a certain type should be structured (i.e. button can contain a span but not a div)

For webpages, the DOCTYPE declaration is required. It is used to tell user agents what version of the HTML specifications your document respects.

Once a user agent has recognized a correct DOCTYPE, it will trigger the no-quirks mode matching the DOCTYPE for reading the document.

If a user agent doesn't recognize a correct DOCTYPE, it will trigger the quirks mode.

The HTML5 DOCTYPE declaration is `<!DOCTYPE html>`

### How do you serve a page with content in the multiple languages?
When an HTTP request is made to server, the requesting user agent usually sends information about language preferences, such as in the Accept-Language header. The server can then use this information to return a version of the document in the appropriate language if such an alternative is available. The returned HTML document should also declare the lang attribute in the `<html>` tag, such as `<html lang="en">..</html>`.

In the back end, the HTML markup will contain i18n placeholders and content for the specific language stored in YML or JSON formats. The server then dynamically generates the HTML page with content in that particular language, usually with the help of a back end framework.

### What are data- attributes good for?
#### Simple answer
==It makes HTML elements contain extra information without using non-standard attributes, or other hacks like that.==
#### Details
Before JavaScript frameworks became popular, front end developers used `data-` attributes to store extra data within the DOM itself, without other hacks such as non-standard attributes, extra properties on the DOM. It is intended to store custom data private to the page of application, for which there are no more appropriate attributes or elements.

These days, using `data-` attributes is not encouraged. One reason is that users can modify the data attribute easily by using inspect element in the browser. The data model is better stored within JavaScript itself and stay updated with the DOM via data binding possibly through a library or a framework.

### Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

All the above-mentioned technologies are key-value storage mechanisms on the client side. They are only able to store values as strings.

|attributes         | `cookie`     | `localStorage` | `sessionStorage` |
| -------------------------------------- | -------------------------------------------------------- | -------------- | ---------------- |
| Initiator (由谁初始化)                             | Client or server. Server can use `Set-Cookie` header     | Client         | Client           |
| Expiry                                 | Manually set                                             | Forever        | On tab close     |
| Persistent across browser sessions (在当前浏览器会话（browser sessions）中是否保持不变)     | Depends on whether expiration is set                     | Yes            | No               |
| Sent to server with every HTTP request (是否随着每个 HTTP 请求发送给服务器) | Cookies are automatically being sent via `Cookie` header | No             | No               |
| Capacity (per domain)                  | 4kb                                                      | 5MB            | 5MB              |
| Accessibility (访问权限)                         | Any window                                               | Any window     | Same tab         |


### Describe the difference between `<script>`, `<script async>` and `<script defer>`
#### simple answer
- `<script>` stops rendering process, and download and run a script.
- `<script async>` don't stop rendering process while asynchronously downloading a script. When finishing download, it stops rendering and runs the script.
- `<script defer>` don't stop rendering process while asynchronously downloading a script. When finishing rendering, it runs the script.

#### detail
- `<script>` - HTML parsing is blocked, the script is fetched and executed immediately, HTML parsing continue after the script is executed
- `<script async>` - The script will be fetched in parallel to HTML parsing and executed as soon as it's available (potentially before HTML parsing completeds). Use `async` when the script is independent of any other scripts on the page, for example, analytics.
- `<script defer>` - The script will be fetched in parallel to HTML parsing and executed when the page has finished parsing. If there are multiple of them, each deferred script is executed in the order they were encountered in the document. If a script relies on a fully-parsed DOM, the defer attribute will be useful in ensuring that the HTML is fully parsed before executing. There is not much difference in putting a normal `<script>` at the end of `<body>`. A deferred script must no contain document.write.

Note: The async and defer attributes are ignored for scripts that have no src attribute.


### Why is is generally a good idea to postion CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
- Placing `<link>`s  in the `<head>`

Putting`<link>`s in the head is part of proper specification in building an optimized website. When a page first loads, HTML and CSS are being parsed simultaneously; HTML creates the DOM (Doucment Object Model) and CSS creates the CSSOM (CSS Object Model). Both are needed to create the visuals in a website, allowing for a quick 'first meaningful paint' timing. This progressive rendering is category optimization sites are measured in their performance scores. Putting stylessheets near the bottom of the document is what prohibits progressive rendering in many browsers. Some browsers block rendering to avoid having to repaint elements of the page if their style change. The user is then stuck viewing a blank white page. Other times there can be flashes of unstyled content, which can shows a webpage with no styling applied

- Placing `<script>`s just before `</body>`

`<script>`s block HTML parsing while they are being downloaded and executed. Placing the scripts at the bottom will allow the HTML to be parsed and displayed to the user first.

An exception for positioning of `<script>`s at the bottom is when your script contains `document.write()`, but these days it is not a good practice to use it. Also, placing `<script>`s at the bottom means that the browser cannot start downloading the script until the entire document is parsed. This is ensure your code that needs to manipulate DOM elements will not throw and error and halt the entire script. If you need to put `<script>` in the `<head>`, use defer attribute, which will achieve the same effect of downloading and running the script only after the HTML is parsed.

### What is progressive rendering?
Progressive rendering is the name given to techniques used to improve the performance of a webpage to render content for display as quickly as possible.

It used to be much more prevalent in the days before broadband internet but it is still used in modern development as mobile data connections are becoming increasingly popular.

Examples of such techniques:

- Lazy loading of images - Images on the page are not loaded all at once. JavaScript will be used to load an image when the user scrolls into the part of the page that displays the image.
- Prioritizing visible content - Include only the minimum CSS/content/Scripts necessary for the amount of page that would be rendered in the users browser first to display as quickly as possible, you an then use deferred scripts or listen for the DOMContentLoaded / load event to load in other resources and content.
- Async HTML fragments. - Flusing parts of the HTML to the browser as the page is constructed on the back end.

### Why you would use a srcset attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.
You would use the srcset attribute when you want to serve different images to users depending on their device display width - serve higher quality images to devices with retina display enhances the user experience while serving lower resolution images to low-end devices increase performance and decrease data wastage. For example: `img srcset="small.jpg 500w, medium.jpg 1000w, large.jpg 2000w" src="..." alt="">` tells the browser to display the small, medium or large jpg depending on the client's resolution. The first value is the image name and the second is the width of the image in pixels. For a device width of 320px, the following calculations are made:
- 500 /320 = 1.5625
- 1000 / 320 = 3.125
- 2000 / 320 = 6.25

If the client's resolution is 1x, 1.5625 is the closest, and 500w corresponding to small.jpg will be selected by the browser.

If the resolution is retina (2x), the browser will use the closest resolution above the minimum. Meaning it will not choose the 500w (1.5625) because it is greater than 1 and the image might look bad. The browser would then choose the image with a resulting ratio closer to 2 which is 1000w (3.125).

srcsets solve the problem whereby you want to serve smaller image files to narrow screen devices, as they don't need huge images like desktop displays do — and also optionally that you want to serve different resolution images to high density/low-density screens.

### Have you used different HTML template language before?
Yes. Jade and EJS in node.js.  In my opinion, they are more or less the same and provide similar functionality of escaping content and helpful filters for manipulating the data to be displayed. Most template engines will also allow you to inject your own filters in the event you need custom processing before display.