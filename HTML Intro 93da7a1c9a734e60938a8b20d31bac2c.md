# HTML Intro

Created: November 18, 2023 9:33 AM
Class: Web technologies
Reviewed: No

## Headings(h1-h6)

```html
<h1></h1>
```

## Map

The **`<map>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element is used with `[<area>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/area)` elements to define an image map (a clickable link area).

```html
<map name="">
  <area/>
</map>
```

## Area

The **`<area>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element defines an area inside an image map that has predefined clickable areas

```html
<area shape="" cords="" href="" alt="" target=""/>
```

## Menu

a semantic alternative to `[<ul>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul).` It represents an unordered list of items (which are represented by `[<li>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li)` elements).

```html
<menu>
  <li>Hello</li>
</menu>
```

## **The Bidirectional Isolate element**

The **`<bdi>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element tells the browser's bidirectional algorithm to treat the text it contains in isolation from its surrounding text.

```html
<h1>World wrestling championships</h1>

<ul>
  <li><bdi class="name">Evil Steven</bdi>: 1st place</li>
  <li><bdi class="name">François fatale</bdi>: 2nd place</li>
  <li><span class="name">سما</span>: 3rd place</li>
  <li><bdi class="name">الرجل القوي إيان</bdi>: 4th place</li>
  <li><span class="name" dir="auto">سما</span>: 5th place</li>
</ul>
```

## HTML File Paths

![Untitled](HTML%20Intro%2093da7a1c9a734e60938a8b20d31bac2c/Untitled.png)

## **The Bidirectional Text Override element**

The **`<bdo>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element overrides the current directionality of text, so that the text within is rendered in a different direction.

```html
<h1>Famous seaside songs</h1>

<p>The English song "Oh I do like to be beside the seaside"</p>

<p>Looks like this in Hebrew: <span dir="rtl">אה, אני אוהב להיות ליד חוף הים</span></p>

<p>In the computer's memory, this is stored as <bdo dir="ltr">אה, אני אוהב להיות ליד חוף הים</bdo></p>
```

## **The Table Caption element**

The **`<caption>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element specifies the caption (or title) of a table.

```html
<table>
  <caption>
    He-Man and Skeletor facts
  </caption>
  <tr>
    <td> </td>
    <th scope="col" class="heman">He-Man</th>
    <th scope="col" class="skeletor">Skeletor</th>
  </tr>
  <tr>
    <th scope="row">Role</th>
    <td>Hero</td>
    <td>Villain</td>
  </tr>
  <tr>
    <th scope="row">Weapon</th>
    <td>Power Sword</td>
    <td>Havoc Staff</td>
  </tr>
  <tr>
    <th scope="row">Dark secret</th>
    <td>Expert florist</td>
    <td>Cries at romcoms</td>
  </tr>
</table>
```

## **The Content Division element**

The **`<div>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element is the generic container for flow content. It has no effect on the content or layout until styled in some way using [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS) (e.g. styling is directly applied to it, or some kind of layout model like [Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout) is applied to its parent element).

```html
div class="warning">
  <img src="/media/examples/leopard.jpg" alt="An intimidating leopard." />
  <p>Beware of the leopard</p>
</div>
```

```css
.warning {
  border: 10px ridge #f00;
  background-color: #ff0;
  padding: 0.5rem;
  display: flex;
  flex-direction: column;
}

.warning img {
  width: 100%;
}

.warning p {
  font: small-caps bold 1.2rem sans-serif;
  text-align: center;
}
```

## **The Inline Frame element**

The **`<iframe>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element represents a nested [browsing context](https://developer.mozilla.org/en-US/docs/Glossary/Browsing_context), embedding another HTML page into the current one.

```html
<iframe
  id="inlineFrameExample"
  title="Inline Frame Example"
  width="300"
  height="200"
  src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&layer=mapnik">
</iframe>
```

## **<hgroup>**

The **`<hgroup>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element represents a heading and related content. It groups a single `[<h1>–<h6>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)` element with one or more `[<p>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)`.

```html
<hgroup>
  <h1>Frankenstein</h1>
  <p>Or: The Modern Prometheus</p>
</hgroup>
<p>
  Victor Frankenstein, a Swiss scientist, has a great ambition: to create intelligent life. But when his creature first
  stirs, he realizes he has made a monster. A monster which, abandoned by his master and shunned by everyone who sees
  it, follows Dr Frankenstein to the very ends of the earth.
</p>
```

## HTML Form

The **`<form>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element represents a document section containing interactive controls for submitting information. The HTML `<form>` element is used to create an HTML form for user input:

```html
<form>
.
form elements
.
</form>
```

## **The <input> Element**

The HTML `<input>` element is the most used form element.

An `<input>` element can be displayed in many ways, depending on the `type` attribute.

![Untitled](HTML%20Intro%2093da7a1c9a734e60938a8b20d31bac2c/Untitled%201.png)

# **Text Fields**

The `<input type="text">` defines a single-line input field for text input.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

## **The <label> Element**

The `<label>` tag defines a label for many form elements.

The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focuses on the input element.

The `<label>` element also helps users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the `<label>` element, it toggles the radio button/checkbox.

The `for` attribute of the `<label>` tag should be equal to the `id` attribute of the `<input>` element to bind them together.

## **Radio Buttons**

The `<input type="radio">` defines a radio button.

Radio buttons let a user select ONE of a limited number of choices.

```html
<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

## **Checkboxes**

The `<input type="checkbox">` defines a **checkbox**.

Checkboxes let a user select ZERO or MORE options of a limited number of choices.

```html
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
```

## **The Submit Button**

The `<input type="submit">` defines a button for submitting the form data to a form-handler.

The form-handler is typically a file on the server with a script for processing input data.

The form-handler is specified in the form's `action` attribute.

```html
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

## **The Name Attribute for <input>**

Notice that each input field must have a `name` attribute to be submitted.

If the `name` attribute is omitted, the value of the input field will not be sent at all.

```html
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form>
```