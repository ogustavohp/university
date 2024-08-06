# HTML #

HTML is based on the concept of hypertext, which involves sets of elements interconnected by links, such as words, images, videos, audio, and documents. These interconnected elements form an extensive network of information.

The primary goal of HTML is to structure the content of a web page, enabling the creation of various types of links to other pages and files, as well as allowing for the construction of forms, tables, lists, and more. When we visit a website and click on a page, we are essentially accessing an HTML document.

HTML serves as the fundamental language for creating web pages, allowing you to organize content and embed multimedia elements such as images and videos. The `<img>` tag is used to add images, requiring the `src` attribute to specify the image’s location and the `alt` attribute to provide descriptive text. This alternative text is essential for accessibility and for displaying if the image fails to load.

To incorporate videos into HTML pages, the `<video>` tag is used. Within the `<video>` tag, the `<source>` element’s `src` attribute specifies the video file path, while the `type` attribute defines the video format. By including multiple `<source>` elements, you can support various video formats, ensuring compatibility across different browsers.

Lists are vital for organizing information on web pages. HTML provides three list types: unordered (`<ul>`), ordered (`<ol>`), and description (`<dl>`). Unordered lists present items with bullet points, ordered lists use numbers or letters in sequence, and description lists are used to display terms alongside their definitions.

Accessibility is a key consideration in web development, ensuring that all users, including those with disabilities, can access and understand content. The `alt` attribute in the `<img>` tag is an example of an accessibility feature, offering a textual description of the image for users who are unable to view it.

Browser compatibility is also crucial. Since not all browsers support the same video formats, it is important to provide multiple video formats using the `<source>` tag within the `<video>` tag. This approach helps ensure that the video can be played across various browsers.

HTML5 introduced new semantic elements, such as the `<figure>` tag for displaying figures and the `<figcaption>` tag for captions. These elements help structure content more meaningfully, making it easier for developers and accessibility tools to understand the code.

The `<video>` tag includes several attributes to control playback, such as `controls` for adding playback controls, `autoplay` for starting the video automatically, and `muted` for turning off the audio.

Lists can be styled with CSS to alter the appearance of bullets, numbers, or letters. You can use different marker styles, such as discs, circles, or squares, and customize colors, sizes, and other properties.

The `<a>` tag, when used with the `<li>` tag, can create links within list items, enabling navigation to different pages or sections of a site. This combination is commonly used to build navigation menus.


# Tags #

## `<img/>` ##

```bash
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```
The `<img>` tag is used to embed an image in an HTML page.

Images are not directly inserted into a web page; instead, they are linked to the page. The `<img>` tag creates a space for the referenced image to be displayed.

The `<img>` tag has two required attributes: `alt` and `src`

`Note`: Always specify the width and height attributes for an image. Omitting these attributes may cause the page to flicker as the image loads.

**Attributes `<img/>`**

- `src*`: Specifies the path to the image file.

- `alt*`: Specifies alternate text for the image, displayed if the image cannot be shown.

- `crossorigin`: Defines how the browser should handle cross-origin requests for images. Possible values:
  - `anonymous`: Requests the image without sending credentials.
  - `use-credentials`: Requests the image with credentials (such as cookies).

- `height`: Specifies the height of the image in pixels.

- `ismap`: Specifies that the image is a server-side image map, allowing for server-side processing of click areas.

- `loading`: Specifies whether the browser should load the image immediately or defer loading until certain conditions are met. Possible values:
  - `eager`: Loads the image immediately.
  - `lazy`: Defers loading the image until it is needed (e.g., when it comes into the viewport).

- `longdesc`: Provides a URL to a detailed description of the image, often used for accessibility purposes.

- `referrerpolicy`: Determines which referrer information is sent when fetching an image. Possible values:
  - `no-referrer`
  - `no-referrer-when-downgrade`
  - `origin`
  - `origin-when-cross-origin`
  - `unsafe-url`

- `sizes`: Specifies image sizes for different page layouts, helping the browser select the appropriate image file based on the viewport.

- `srcset`: Provides a list of image files to use in different situations, such as varying resolutions or screen sizes.

- `usemap`: Associates the image with a client-side image map, allowing for interactive areas within the image. The value should be `#mapname`, where `mapname` corresponds to the `name` attribute of the `<map>` element.

- `width`: Specifies the width of the image in pixels.

## `<figure/> & <figcaption>` ##

```bash
<figure>
  <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>
```

The `<figure>` tag specifies self-contained content, such as illustrations, diagrams, photos, or code listings.

Although the content within the `<figure>` element is related to the main flow of the document, its positioning is independent of the main flow. Removing it should not affect the overall structure of the document.

**Tip:** Use the `<figcaption>` element to add a caption to the `<figure>` element.



## `<video/> & <source>` ##

```bash
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

The `<video>` tag contains one or more `<source>` tags with different video sources. The browser will choose the first source it supports.

The text between the `<video>` and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.

It is recommended to set the height and width attributes on the `<video>` tag because, if not defined, the page may flicker in some browsers while the video loads. Setting these attributes helps allocate the necessary space for the video in the page layout, preventing reflow (rearrangement of elements) or layout shift when the video is loaded.

**Attributes `<video/>`**

- `controls`: Specifies that video controls, such as play, pause, and volume buttons, should be displayed
- `src`: Specifies the URL of the video file.
- `width`: Specifies the width of the video player in pixels.
- `height`: Specifies the height of the video player in pixels.
- `autoplay`: Specifies that the video will start playing automatically as soon as it is ready.
- `loop`: Specifies that the video will start over again every time it finishes.
- `muted`: Specifies that the audio output of the video should be muted.
- `poster`: Specifies an image to be displayed while the video is downloading or until the user hits the play button.
- `preload`: Specifies how the video should be loaded when the page loads. Possible values are:

  - `auto`: The browser should load the entire video when the page loads.
  -  `metadata`: The browser should load only the video's metadata (e.g., dimensions, duration).
  - `none`: The browser should not preload the video.

**Attributes `<source/>`**

- `media`: Accepts any valid media query that would normally be defined in CSS. It allows you to specify different media resources based on conditions such as screen size or device type.

- `sizes`: Specifies image sizes for different page layouts. This attribute helps browsers choose the most appropriate image source based on the layout and viewport size.

- `src`: Required when using `<source>` in `<audio>` and `<video>`. Specifies the URL of the media file.

- `srcset`: Required when using `<source>` in `<picture>`. Specifies the URL of the image to use in different situations, such as varying resolutions or screen sizes.

- `type`: Specifies the MIME type of the resource. This helps the browser understand the format of the media and ensure proper playback.

## `<ul/>, <ol/>, <li/>, <dl/>, <dt/> & <dd/>` ##

The `<ul>` tag defines an unordered (bulleted) list.

Use the `<ul>` tag in conjunction with the `<li>` tag to create a list where items are presented with bullet points.

The `<li>` tag defines a list item.

It is used inside ordered lists (`<ol>`), unordered lists (`<ul>`), and menu lists (`<menu>`).


```bash
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
*result:*
- Coffee
- Tea
- Milk

```bash
<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
*result:*

50. Coffee
51. Tea
52. Milk

The `<dl>` tag defines a description list.

The `<dl>` tag is used in conjunction with the `<dt>` tag, which defines terms or names, and the `<dd>` tag, which provides descriptions for each term or name.


```bash
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```
*result:*

Coffee

&nbsp;&nbsp;&nbsp;&nbsp;Black hot drink

Milk

&nbsp;&nbsp;&nbsp;&nbsp;White cold drink

## `<nav/>` ##

The `<nav>` tag defines a set of navigation links.

It's important to note that not all links in a document should be placed inside a `<nav>` element. The `<nav>` element is intended specifically for major blocks of navigation links, such as menus or site-wide navigation.

Browsers and assistive technologies, such as screen readers, can use the `<nav>` element to identify and manage the rendering of navigation content, helping users with disabilities by allowing them to skip directly to main navigation sections.

```bash
<nav>
  <a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/python/">Python</a>
</nav>
```

## `<hr>` ##

The `<hr>` tag defines a thematic break in an HTML page, such as a shift in topic or a separation of content.

The `<hr>` element is most commonly displayed as a horizontal rule, which visually separates sections or indicates a change in the content of the page.