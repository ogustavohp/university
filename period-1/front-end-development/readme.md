missing: tag: div

# HTML #


HTML is based on the concept of hypertext, which involves sets of elements interconnected by links, such as words, images, videos, audio, and documents. These interconnected elements form an extensive network of information.

The primary goal of HTML is to structure the content of a web page, enabling the creation of various types of links to other pages and files, as well as allowing for the construction of forms, tables, lists, and more. When we visit a website and click on a page, we are essentially accessing an HTML document.

### **Media** ###

HTML serves as the fundamental language for creating web pages, allowing you to organize content and embed multimedia elements such as images and videos. The `<img>` tag is used to add images, requiring the `src` attribute to specify the image’s location and the `alt` attribute to provide descriptive text. This alternative text is essential for accessibility and for displaying if the image fails to load.

To incorporate videos into HTML pages, the `<video>` tag is used. Within the `<video>` tag, the `<source>` element’s `src` attribute specifies the video file path, while the `type` attribute defines the video format. By including multiple `<source>` elements, you can support various video formats, ensuring compatibility across different browsers.

Lists are vital for organizing information on web pages. HTML provides three list types: unordered (`<ul>`), ordered (`<ol>`), and description (`<dl>`). Unordered lists present items with bullet points, ordered lists use numbers or letters in sequence, and description lists are used to display terms alongside their definitions.

Accessibility is a key consideration in web development, ensuring that all users, including those with disabilities, can access and understand content. The `alt` attribute in the `<img>` tag is an example of an accessibility feature, offering a textual description of the image for users who are unable to view it.

Browser compatibility is also crucial. Since not all browsers support the same video formats, it is important to provide multiple video formats using the `<source>` tag within the `<video>` tag. This approach helps ensure that the video can be played across various browsers.

HTML5 introduced new semantic elements, such as the `<figure>` tag for displaying figures and the `<figcaption>` tag for captions. These elements help structure content more meaningfully, making it easier for developers and accessibility tools to understand the code.

The `<video>` tag includes several attributes to control playback, such as `controls` for adding playback controls, `autoplay` for starting the video automatically, and `muted` for turning off the audio.

Lists can be styled with CSS to alter the appearance of bullets, numbers, or letters. You can use different marker styles, such as discs, circles, or squares, and customize colors, sizes, and other properties.

The `<a>` tag, when used with the `<li>` tag, can create links within list items, enabling navigation to different pages or sections of a site. This combination is commonly used to build navigation menus.

### **Table** ###

HTML tables are essential tools for organizing and presenting structured data on web pages. They allow information to be displayed in rows and columns, facilitating easier reading and data comparison for users. To create an HTML table, we use the `<table>` tag, which marks the beginning and end of the table. Within the table, each row is defined by the `<tr>` (table row) tag, and each cell within a row is defined by the `<td>` (table data) tag.

For column headers, typically displayed in bold and centered, we use the `<th>` (table header) tag instead of `<td>`. `<th>` helps highlight column titles, enhancing table readability. In addition to the basic structure, HTML5 introduced semantic elements that add meaning and structure to tables, making them more accessible and optimized for search engines.

The `<caption>` tag is used to add a caption to the table, providing a brief description of its content. This caption is beneficial for screen readers, which can read the table description before users decide to navigate its data.

While tables are powerful for organizing data, it's important to use them solely for this purpose. In the past, tables were often used for website layout, but this practice is now discouraged. Using tables for layout can hinder website accessibility for visually impaired users and make HTML code more complex and harder to maintain.

Semantic tags like `<thead>` (table head), `<tbody>` (table body), and `<tfoot>` (table foot) do not change the visual appearance of the table by default but provide crucial information for browsers, screen readers, and search engines. These tags help structure the table logically, making it easier to understand and process.

### Form ###

HTML forms are fundamental elements in web development, facilitating user interaction with websites and applications. They provide a structured way to collect user data such as names, email addresses, and messages, which is then sent to a server for processing. This processing could involve actions like sending an email, storing data in a database, or performing computations.

To create HTML forms, the `<form>` tag is used as a container for all form elements. Within the `<form>` tag, various input fields can be utilized, each designed to capture a specific type of information.

Every form field should include a `name` attribute, which is essential for identifying the field and its value when data is submitted to the server. Additionally, the `label` attribute is used to provide a descriptive label for the field, enhancing both accessibility and usability.

The `<select>` tag is employed to create dropdown lists, allowing users to choose an option from a predefined set. Options within the dropdown are specified using the `<option>` tag.

Form data can be transmitted to the server using two primary HTTP methods: GET and POST. The GET method appends data to the URL, making it visible in the browser’s address bar. This method is suitable for non-sensitive data and has limitations on the amount of data that can be sent.

Conversely, the POST method sends data in the body of the HTTP request, keeping it hidden from the URL. This method is preferred for transmitting sensitive information, such as passwords, and does not have the size limitations of GET.

Form validation is an important aspect of web development, ensuring that user input is formatted correctly and meets specific criteria. This can be achieved through HTML attributes like `required` for mandatory fields and client-side scripting languages such as JavaScript.

In summary, HTML forms are crucial for user interaction on the web, enabling data submission to web servers and supporting a variety of functionalities from simple message submissions to complex transactions.

Checkboxes allow users to select multiple options from a list, with each checkbox functioning independently. Users can check or uncheck each option as needed. In contrast, radio buttons restrict selection to a single option within a group. Selecting a radio button in a group will automatically deselect any previously chosen button in that group.

Dropdown lists, also known as select boxes, provide a compact way to display a list of options. They are particularly useful when there are many choices, as they conserve screen space. Users can click on the dropdown to view and select the desired option. To organize input fields more logically and aesthetically, the 'fieldset' element can be used. The 'fieldset' wraps a group of related input fields, making the form easier to understand and complete.

Understanding the attributes that control the behavior and appearance of form fields is also crucial. The 'name' attribute identifies the input field when the form data is submitted. The 'value' attribute specifies the value sent to the server upon form submission. For checkboxes and radio buttons, the 'value' attribute is especially important as it determines the value associated with the selected option.

Designing effective forms involves more than just technical details; it also requires a focus on user experience. Well-designed forms should be intuitive, user-friendly, and provide clear feedback. Utilizing elements like 'labels' for input field descriptions and informative error messages can greatly enhance the user experience.

Mastering different input field types, their attributes, and best practices for form design is essential for creating interactive and efficient web applications. The quality of your forms significantly impacts your site's usability, so it’s important to invest time and effort in understanding them thoroughly.

The W3Schools documentation is a valuable resource for deepening your knowledge of HTML forms. It offers detailed information on various input field types, their attributes, and practical usage examples.


## Tags ##

### `<img/>` ###

```bash
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```
The `<img>` tag is used to embed an image in an HTML page.

Images are not directly inserted into a web page; instead, they are linked to the page. The `<img>` tag creates a space for the referenced image to be displayed.

The `<img>` tag has two required attributes: `alt` and `src`

`Note`: Always specify the width and height attributes for an image. Omitting these attributes may cause the page to flicker as the image loads.

**Attributes `<img/>`**

- **src***: Specifies the path to the image file.

- **alt***: Specifies alternate text for the image, displayed if the image cannot be shown.

- **crossorigin**: Defines how the browser should handle cross-origin requests for images. Possible values:
  - **anonymous**: Requests the image without sending credentials.
  - **use-credentials**: Requests the image with credentials (such as cookies).

- **height**: Specifies the height of the image in pixels.

- **ismap**: Specifies that the image is a server-side image map, allowing for server-side processing of click areas.

- **loading**: Specifies whether the browser should load the image immediately or defer loading until certain conditions are met. Possible values:
  - **eager**: Loads the image immediately.
  - **lazy**: Defers loading the image until it is needed (e.g., when it comes into the viewport).

- **longdesc**: Provides a URL to a detailed description of the image, often used for accessibility purposes.

- **referrerpolicy**: Determines which referrer information is sent when fetching an image. Possible values:
  - **no-referrer**
  - **no-referrer-when-downgrade**
  - **origin**
  - **origin-when-cross-origin**
  - **unsafe-url**

- **sizes**: Specifies image sizes for different page layouts, helping the browser select the appropriate image file based on the viewport.

- **srcset**: Provides a list of image files to use in different situations, such as varying resolutions or screen sizes.

- **usemap**: Associates the image with a client-side image map, allowing for interactive areas within the image. The value should be `#mapname`, where `mapname` corresponds to the `name` attribute of the `<map>` element.

- ****width****: Specifies the width of the image in pixels.

### `<figure/> & <figcaption>` ###

```bash
<figure>
  <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>
```

The `<figure>` tag specifies self-contained content, such as illustrations, diagrams, photos, or code listings.

Although the content within the `<figure>` element is related to the main flow of the document, its positioning is independent of the main flow. Removing it should not affect the overall structure of the document.

**Tip:** Use the `<figcaption>` element to add a caption to the `<figure>` element.



### `<video/> & <source>` ###

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

- ****controls****: Specifies that video controls, such as play, pause, and volume buttons, should be displayed
- ****src****: Specifies the URL of the video file.
- ****width****: Specifies the width of the video player in pixels.
- ****height****: Specifies the height of the video player in pixels.
- ****autoplay****: Specifies that the video will start playing automatically as soon as it is ready.
- ****loop****: Specifies that the video will start over again every time it finishes.
- ****muted****: Specifies that the audio output of the video should be muted.
- ****poster****: Specifies an image to be displayed while the video is downloading or until the user hits the play button.
- ****preload****: Specifies how the video should be loaded when the page loads. Possible values are:

  - ****auto****: The browser should load the entire video when the page loads.
  -  ****metadata****: The browser should load only the video's metadata (e.g., dimensions, duration).
  - ****none****: The browser should not preload the video.

**Attributes `<source/>`**

- ****media****: Accepts any valid media query that would normally be defined in CSS. It allows you to specify different media resources based on conditions such as screen size or device type.

- ****sizes****: Specifies image sizes for different page layouts. This attribute helps browsers choose the most appropriate image source based on the layout and viewport size.

- ****src****: Required when using `<source>` in `<audio>` and `<video>`. Specifies the URL of the media file.

- ****srcset****: Required when using `<source>` in `<picture>`. Specifies the URL of the image to use in different situations, such as varying resolutions or screen sizes.

- ****type****: Specifies the MIME type of the resource. This helps the browser understand the format of the media and ensure proper playback.

### `<ul/>, <ol/>, <li/>, <dl/>, <dt/> & <dd/>` ###

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

### `<nav/>` ###

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

### `<hr>` ###

The `<hr>` tag defines a thematic break in an HTML page, such as a shift in topic or a separation of content.

The `<hr>` element is most commonly displayed as a horizontal rule, which visually separates sections or indicates a change in the content of the page.

### `<table/>` ###

The `<table>` tag defines an HTML table.

An HTML table is made up of one `<table>` element and can include one or more `<tr>`, `<th>`, and `<td>` elements. 

- The `<tr>`: element defines a table row. 
- The `<th>` element defines a table header cell. 
- The `<td>` element defines a standard table cell.

In addition, an HTML table may also include optional elements such as `<caption>`, `<colgroup>`, `<thead>`, `<tfoot>`, and `<tbody>` to provide additional structure and information.

- The `<thead>`element groups the header content in a table.
- The `<tbody>`element groups the body content in a table.
- The `<tfoot>`element groups the footer content in a table.
- The `<caption>` element provides a title or explanation for the table.
- The `<colgroup>` element specifies a group of one or more columns in a table for formatting.

Note: The `<colgroup>` tag must be a child of a `<table>` element, placed after any `<caption>` elements and before any `<thead>`, `<tbody>`, `<tfoot>`, and `<tr>` elements.



```bash
<table>
  <caption>Title or description</caption>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
      <th>Test</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
      <td>Test</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
      <td>Test</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sum</td>
      <td>$180</td>
      <td>Test</td>
    </tr>
  </tfoot>
</table>
```

### `<form/>` ###

The `<form>` tag is used to create an HTML form for user input.

The `<form>` element can contain one or more of the following form elements:

- `<input>`: Used to create various types of input fields.
- `<textarea>`: Used to create a multi-line text input field.
- `<button>`: Used to create a clickable button.
- `<select>`: Used to create a drop-down list.
- `<option>`: Used to define an option within a `<select>` element.
- `<optgroup>`: Used to group related options within a `<select>` element.
- `<fieldset>`: Used to group related elements within a form.
- `<label>`: Used to define a label for an `<input>` element.
- `<output>`: Used to represent the result of a calculation or user action.

```bash
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname">
  <input type="submit" value="Submit">
</form>
```

**Attributes `<form/>`**

- **accept-charset**: `character_set`  
  Specifies the character encodings that the server should use to process the form data. For example, `UTF-8` ensures that the form data is encoded using the UTF-8 character set.

- **action**: `URL`  
  Defines the URL where the form data will be sent when the form is submitted. For instance, `https://example.com/submit` directs the form submission to this endpoint.

- **autocomplete**: `on`, `off`  
  Determines whether the browser should automatically complete form fields based on past inputs. `on` enables autocomplete, while `off` disables it.

- **enctype**: `application/x-www-form-urlencoded`, `multipart/form-data`, `text/plain`  
  Specifies the encoding type for the form data when it is sent to the server. 
  - `application/x-www-form-urlencoded`: Encodes form data as key-value pairs, suitable for simple forms.
  - `multipart/form-data`: Used for forms that include file uploads.
  - `text/plain`: Sends form data as plain text, with no encoding.

- **method**: `get`, `post`  
  Defines the HTTP method used to send the form data.
  - `get`: Appends form data to the URL as query parameters. Suitable for retrieving data.
  - `post`: Sends form data in the body of the HTTP request. Suitable for submitting data.

- **name**: `text`  
  Assigns a name to the form. This name can be used to reference the form in scripts or for identification purposes.

- **novalidate**: `novalidate`  
  Indicates that the form should bypass the browser's built-in validation checks. This is useful when custom validation is implemented or when validation is not desired.

- **rel**: `external`, `help`, `license`, `next`, `nofollow`, `noopener`, `noreferrer`, `opener`, `prev`, `search`  
  Specifies the relationship between the current document and a linked resource.
  - `external`: Indicates the link points to an external site.
  - `help`: The link provides help or documentation.
  - `license`: The link refers to licensing information.
  - `next`: Points to the next document in a sequence.
  - `nofollow`: Instructs search engines not to follow the link.
  - `noopener`: Ensures that the linked page cannot access the linking page's `window` object.
  - `noreferrer`: Prevents the browser from sending the referrer header to the linked resource.
  - `opener`: Allows the linked page to access the linking page’s `window` object.
  - `prev`: Points to the previous document in a sequence.
  - `search`: Indicates the link provides a search function.

- **target**: `_blank`, `_self`, `_parent`, `_top`  
  Defines where to display the response after the form is submitted.
  - `_blank`: Opens the response in a new tab or window.
  - `_self`: Opens the response in the same frame or window (default behavior).
  - `_parent`: Opens the response in the parent frame of the current frame.
  - `_top`: Opens the response in the full window or tab, replacing any frames.


### `<label/>, <input> & <textarea/>` ###

**Label**

The `<label>` tag in HTML is used to define a label for form elements such as:

- `<input type="checkbox">`
- `<input type="color">`
- `<input type="date">`
- `<input type="datetime-local">`
- `<input type="email">`
- `<input type="file">`
- `<input type="month">`
- `<input type="number">`
- `<input type="password">`
- `<input type="radio">`
- `<input type="range">`
- `<input type="search">`
- `<input type="tel">`
- `<input type="text">`
- `<input type="time">`
- `<input type="url">`
- `<input type="week">`
- `<meter>`
- `<progress>`
- `<select>`
- `<textarea>`

Properly using `<label>` with these elements provides several benefits:

- **Screen Reader Users**: Screen readers will read out the label text when the user is focused on the corresponding form element, enhancing accessibility.
- **Increased Click Area**: Labels improve usability for users with difficulty clicking on small areas, such as checkboxes. Clicking the label text toggles the associated input, making it easier to interact with.

**Tip**: To properly bind a label to its related element, use the `for` attribute of the `<label>` tag, which should match the `id` of the associated element. Alternatively, placing the form element inside the `<label>` element also links them together.

**Input**

The `<input>` tag defines an input field for user data entry and is a fundamental element in HTML forms. 

The `<input>` element's appearance and behavior vary based on its `type` attribute. Some common input types include:

- **`type="text"`**: Creates a single-line text input field.
- **`type="checkbox"`**: Displays a checkbox that can be toggled on or off.
- **`type="radio"`**: Shows a radio button, allowing the selection of one option from a group.
- **`type="file"`**: Opens a file selection dialog for uploading files.
- **`type="password"`**: Masks the input characters, suitable for entering sensitive information.

**Tip**: Always use the `<label>` tag to associate labels with `<input>` elements like text, checkbox, radio, file, and password fields. This practice enhances accessibility and improves the user interface by making it easier to understand and interact with the form elements.

**Attributes `<input>`**

- **accept**: `file_extension`  
  Specifies the types of files that can be selected in a file input dialog. For example, `audio/*`, `video/*`, `image/*`.

- **alt**: `text`  
  Provides alternative text for images. This attribute is used only with `type="image"`.

- **autocomplete**: `on`, `off`  
  Determines whether autocomplete is enabled or disabled for the input field.

- **autofocus**: `autofocus`  
  Indicates that the input field should automatically receive focus when the page loads.

- **checked**: `checked`  
  Sets the input field to be pre-selected by default. This is used with `type="checkbox"` and `type="radio"`.

- **dirname**: `inputname.dir`  
  Submits the text direction of the input field's value.

- **disabled**: `disabled`  
  Disables the input field, making it unmodifiable by the user.

- **form**: `form_id`  
  Associates the input field with a specific `<form>` element.

- **formaction**: `URL`  
  Defines the URL where the form data should be sent when the form is submitted. Used with `type="submit"` and `type="image"`.

- **formenctype**: `application/x-www-form-urlencoded`, `multipart/form-data`, `text/plain`  
  Specifies how the form-data should be encoded when submitting to the server. Used with `type="submit"` and `type="image"`.

- **formmethod**: `get`, `post`  
  Defines the HTTP method to be used when sending form-data to the action URL. Used with `type="submit"` and `type="image"`.

- **formnovalidate**: `formnovalidate`  
  Indicates that the form should not be validated upon submission. Used with `type="submit"` and `type="image"`.

- **formtarget**: `_blank`, `_self`, `_parent`, `_top`, `framename`  
  Specifies where to display the response after form submission. Used with `type="submit"` and `type="image"`.

- **height**: `pixels`  
  Defines the height of an input element. Used only with `type="image"`.

- **list**: `datalist_id`  
  Refers to a `<datalist>` element that contains predefined options for the input field.

- **max**: `number`, `date`  
  Specifies the maximum allowable value for the input field.

- **maxlength**: `number`  
  Sets the maximum number of characters allowed in the input field.

- **min**: `number`, `date`  
  Specifies the minimum allowable value for the input field.

- **minlength**: `number`  
  Sets the minimum number of characters required in the input field.

- **multiple**: `multiple`  
  Allows multiple values to be entered or selected in the input field.

- **name**: `text`  
  Specifies the name of the input field, which is used to identify it when submitting form data.

- **pattern**: `regexp`  
  Defines a regular expression that the input field's value must match.

- **placeholder**: `text`  
  Provides a short hint or description of the expected value in the input field.

- **popovertarget**: `element_id`  
  Specifies which popover element to invoke. Used only with `type="button"`.

- **popovertargetaction**: `hide`, `show`, `toggle`  
  Defines the action on the popover element when the button is clicked. Used only with `type="button"`.

- **readonly**: `readonly`  
  Makes the input field read-only, preventing any modifications by the user.

- **required**: `required`  
  Indicates that the input field must be filled out before submitting the form.

- **size**: `number`  
  Specifies the width of the input field in characters.

- **src**: `URL`  
  Specifies the URL of the image used as a submit button. Used only with `type="image"`.

- **step**: `number`, `any`  
  Defines the interval between valid values in the input field.

- **type**: `button`, `checkbox`, `color`, `date`, `datetime-local`, `email`, `file`, `hidden`, `image`, `month`, `number`, `password`, `radio`, `range`, `reset`, `search`, `submit`, `tel`, `text`, `time`, `url`, `week`  
  Specifies the type of input field to display.

- **value**: `text`  
  Defines the value of the input field.

- **width**: `pixels`  
  Specifies the width of an input element. Used only with `type="image"`.

**Textarea**

The `<textarea>` tag creates a multi-line text input field.

This element is commonly used in forms to gather user input such as comments or reviews.

A `<textarea>` can accommodate an unlimited number of characters .

The `name` attribute is crucial for linking the form data to the submitted form; without it, the text area’s data won’t be included in the form submission.

The `id` attribute is used to connect the `<textarea>` with a `<label>` for better accessibility.

**Tip**: For optimal accessibility, always use the `<label>` tag to clearly define the purpose of the `<textarea>`.

```bash
<label for="nameForThisFieldId">x:</label>

<textarea id="nameForThisFieldId" name="nameForThisFieldId" rows="4" cols="50">
lorem lorem lorem
</textarea>
```

**Attributes `<textarea/>`**

- **autofocus**: `autofocus`  
  Indicates that the `<textarea>` should automatically receive focus when the page loads.

- **cols**: `number`  
  Specifies the number of visible characters in a single line of the `<textarea>`.

- **dirname**: `textareaname.dir`  
  Determines that the text direction of the `<textarea>` will be submitted with the form data.

- **disabled**: `disabled`  
  Marks the `<textarea>` as disabled, preventing user interaction.

- **form**: `form_id`  
  Links the `<textarea>` to a specific form, allowing it to be submitted with that form.

- **maxlength**: `number`  
  Sets the maximum number of characters that the `<textarea>` can accept.

- **name**: `text`  
  Provides a name for the `<textarea>`, which is used to reference the data when the form is submitted.

- **placeholder**: `text`  
  Displays a short hint or description inside the `<textarea>` when it is empty, guiding the user on what to input.

- **readonly**: `readonly`  
  Makes the `<textarea>` read-only, preventing users from modifying its content.

- **required**: `required`  
  Indicates that the `<textarea>` must be filled out before the form can be submitted.

- **rows**: `number`  
  Defines the number of visible text lines in the `<textarea>`.

- **wrap**: `hard`, `soft`  
  Specifies how the text should be wrapped when submitted with the form.
  - `hard`: Wraps text at the end of each line before submitting it.
  - `soft`: Keeps text formatting as entered by the user, without enforcing line breaks.

### `<fieldset/>` ###

The `<fieldset>` tag is used to group related elements within a form. It creates a box around these elements, visually separating them from other parts of the form. This helps organize and group related form controls together, improving the form's structure and readability.

```bash
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br><br>
    <label for="birthday">Birthday:</label>
    <input type="date" id="birthday" name="birthday"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

### `<legend/>` ###

The `<legend>` tag provides a caption or title for the `<fieldset>` element. It helps describe the group of form controls contained within the `<fieldset>`, enhancing accessibility and improving the overall organization of the form.

### `<select/> & <option/>` ###

**Select**

The `<select>` element creates a drop-down list, commonly used in forms to collect user input. 

The `name` attribute is essential for referencing the selected data after form submission; omitting this attribute will prevent data from being sent. The `id` attribute connects the drop-down list with a label for better accessibility.

The available options within the drop-down list are defined using `<option>` tags nested inside the `<select>` element.

**Tip:** For optimal accessibility, always use the `<label>` tag with the `<select>` element.

```bash
<label for="cars">Choose a car:</label>

<select id="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```

**Attributes `<select/>`**

- **autofocus**: `autofocus`  
  Specifies that the drop-down list should automatically receive focus when the page loads.

- **disabled**: `disabled`  
  Indicates that the drop-down list should be disabled, preventing user interaction.

- **form**: `form_id`  
  Defines the form to which the drop-down list belongs, allowing it to be associated with a specific form.

- **multiple**: `multiple`  
  Allows users to select more than one option from the drop-down list.

- **name**: `name`  
  Provides a name for the drop-down list, which is used to reference the data in the form submission.

- **required**: `required`  
  Specifies that a selection must be made from the drop-down list before the form can be submitted.

- **size**: `number`  
  Sets the number of visible options that will be displayed in the drop-down list.

**Option**

The `<option>` tag defines an individual choice within a select list.

It is used inside a `<select>`, `<optgroup>`, or `<datalist>` element.

**Note:** While the `<option>` tag can be used without attributes, the `value` attribute is typically necessary as it specifies the value sent to the server when the form is submitted.

**Tip:** For long lists of options, group related choices using the `<optgroup>` tag to improve organization and user experience.

**Attributes `<option/>`**

- **disabled**: `disabled`  
  Indicates that the option should be disabled, preventing the user from selecting it.

- **label**: `text`  
  Provides a shorter label for the option, which can be useful for displaying a more user-friendly name.

- **selected**: `selected`  
  Marks the option as pre-selected when the page loads, making it the default choice in the list.

- **value**: `text`  
  Defines the value that will be sent to the server when the form is submitted.


# CSS #

**CSS**, which stands for Cascading Style Sheets, is a crucial language in web development used to define the appearance and layout of HTML pages. Developed in 1996 by the World Wide Web Consortium (W3C), CSS separates style from content, making website creation and maintenance much more efficient. Before CSS, developers had to use HTML tags, like the `<font>` tag, to style each element individually, leading to complex and hard-to-manage code. With CSS, you can control various visual aspects of a site, such as colors, fonts, spacing, positioning, and more, all from a single file or specific code snippets.

CSS syntax consists of three main components: the selector, the property, and the value. The selector identifies the HTML element you want to style, the property defines which characteristic of the element will be modified, and the value determines the new appearance of the property. For example, to change the text color of all paragraphs to red, the selector would be "p", the property would be "color", and the value would be "red". This simple and intuitive structure makes CSS relatively easy to learn and use, even for beginners in web development.

There are three main ways to add CSS to an HTML document: inline, internal, and external. Inline CSS is applied directly to a specific HTML element via the "style" attribute. This approach is useful for one-off changes but can make the code difficult to maintain if used extensively. Internal CSS is defined within the `<style>` tag in the `<head>` section of the HTML document. This method is more organized than inline CSS and allows you to apply styles to multiple elements on the page. External CSS is the most recommended and organized method. It involves creating a separate CSS file and linking it to the HTML document using the `<link>` tag, also located in the `<head>` section.

```bash
<head>
  <link rel="stylesheet" href="style.css">
<head>
```

The major advantage of external CSS is the ability to reuse the same stylesheet across multiple HTML pages, ensuring visual consistency across the site and making maintenance easier. Additionally, external CSS allows for more structured style organization, separating styles by sections or element types, which makes the code more readable and easier to understand. This modular approach also helps in identifying and fixing errors, making the development process more efficient.

The term "cascading" in CSS refers to how styles are applied to HTML elements. CSS operates based on a hierarchy of styles, where more specific styles take precedence over more general ones. For instance, an inline style for an element will override styles defined internally or externally for the same element. This feature enables the creation of complex and customized styles, allowing precise control over the appearance of each page element.

Mastering CSS is essential for anyone looking to work in web development, whether it's for creating websites, blogs, landing pages, or more complex web applications. With CSS, you can transform a simple HTML document into a visually appealing, responsive, and user-friendly page.

To deepen your CSS knowledge, there are numerous online resources available, such as tutorials, courses, documentation, and developer communities. A valuable tip is to use the W3C CSS Validation Service, a free online tool that checks if your CSS code conforms to language standards, helping identify and fix syntax errors and other issues.

CSS properties control various aspects of formatting, such as color, size, font, spacing, positioning, and more.

One of CSS's important properties is `font-family`, which allows defining the font family for text. It's recommended to specify a list of fonts separated by commas to ensure text displays correctly across different devices and browsers. Additionally, custom fonts can be used via the `@font-face` rule.

Another fundamental property is `color`, which sets the text color. Colors can be specified using predefined names like "red," "green," and "blue," or hexadecimal codes such as "#FF0000," "#00FF00," and "#0000FF."

CSS also allows styling HTML lists, transforming them into navigation menus. To achieve this, we can remove the default list markers using `list-style: none;` and arrange items horizontally using `float: left;`. Moreover, spacing between items can be added with the `padding` property, and links can have their underline removed with `text-decoration: none;`.

HTML tables can also be styled using CSS, using specific selectors for rows, columns, and cells. Pseudoclasses like `:nth-child(even)` and `:nth-child(odd)` can be used to apply alternating styles to table rows, creating a zebra-striping effect.

Divs are generic block-level elements used to group other HTML elements and apply styles to them. Classes and IDs can be assigned to divs for identification and specific styling. Classes are reusable, while IDs must be unique within an HTML document.

To select a specific element by ID in CSS, we use the `#` character followed by the ID name. For example, to select an element with the ID "demo," we use the selector `#demo`. To select elements with a specific class, we use the `.` character followed by the class name. For example, to select elements with the class "test," we use the selector `.test`.

The `text-decoration` property is used to add or remove text decorations such as underline, overline, and line-through. To remove the underline from a hyperlink, for instance, we use `text-decoration: none;`.


## Bootstrap ##