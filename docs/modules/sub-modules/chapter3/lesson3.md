# Lesson \#3 - CSS

Now that we know how we can fill out the content of our webpages, let's take a look at how we can style our webpages and create something more pleasing to the eye.

Start by creating a new HTML file and opening it in VS Code.

Paste the following code and save your file.

```html
<!DOCTYPE html>
<html lang="en-us">

<head>
  <meta charset="UTF-8">
  <title>Basic CSS Example</title>
  <link rel="stylesheet" href="style.css">  
</head>

<body>

  <h1>Awesome Header</h1>
  <h2>Smaller Awesome Header</h2>
  <h3>Even Smaller Header</h3>

  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>

  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>

  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>

  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>

  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>

  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>


</body>

</html>
```

Open the file in Chrome. Your page should look like this:

<p align="center">
     <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/html-basic.PNG" width="800" title="html-basic">
</p>

Now create a new file called `style.css`. Before we can add code to our CSS file, we need to include a special tag to tell our HTML page to load the CSS from our newly created file.

Add the following tag inside the `head` section of your HTML.

```html
<link rel="stylesheet" href="style.css">  
```

The head should now look like this:

```html
<head>
  <meta charset="UTF-8">
  <title>Basic CSS Example</title>
  <link rel="stylesheet" href="style.css">  
</head>
```

Now you can customize the look of your sites. Each rule in the style tag changes the appearance of its associated element.

CSS syntax has the form: 

```css
selector {
  property-name: value;
}
```

Add the following code to `style.css`, save the file, then refresh or reload the page in your Browser.

```css
body {
  background-color: #F5DEB3;
  font-family: Arial, Helvetica, sans-serif;
}

h1 {
  text-align: center;
  color: maroon;
  font-size: 48px;
  text-decoration: underline;
}

p {
  color: limegreen;
}
```

What changed?

Notice how each rule names an element from the HTML body.

There is a lot going on here so let's break it down piece-by-piece!

```css
body {
  background-color: #F5DEB3;
  font-family: Arial, Helvetica, sans-serif;
}
```

We start by targeting the body. The body actually refers to our `body` tags in our HTML! So this is a way of targeting everything that shows up on our browser.

While targeting the `body`, we are passing in two CSS properties. `background-color` is setting the background color of our `body`. After the colon, we are telling our CSS to use the hex code, F5DEB3 (<http://www.99colors.net/name/wheat>). The second CSS property, `font-family` allows us to set the text font. The reason there are three font types is that if CSS is unable to find and apply `Arial`, it will then try to apply `Helvetica`. If it cannot find that either, it will find `sans-serif` and apply that.

```css
h1 {
  text-align: center;
  color: maroon;
  font-size: 48px;
  text-decoration: underline;
}
```

For this next block of CSS code, we start by targeting all `h1` tags. The `text-align` CSS property allows us to align the text. In this case, we are centering it by passing in `center`. Next, we set the color of the text to maroon, give it a font size of 48 pixels, and apply a text decoration of `underline`. This means that the text will be underlined.

```css
p {
  color: limegreen;
}
```

Finally, we target all `p` tags and give that text color of lime green.

As you may have guessed, there are *a lot* of CSS properties! We'll only cover a few, but knowing how to find and use documentation is an extremely important part of developing. For your reference, you can find a list of all CSS properties here: <https://developer.mozilla.org/en-US/docs/Web/CSS/Reference>.

Now we'll dive into how CSS can hook into a specific element or set of elements using IDs or Classes. So far you've only learned how to target all of a specific tag such as `h1`, `p`, or even the entire `body`.

To demonstrate this we'll add a class of `orange` to a few paragraphs. We can add a class by setting it as an attribute of our HTML element.

```html
<p class="orange">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>
```

Notice the addition of `class="orange"` _inside_ the `p` tag.

Now, add the CSS below to `style.css` and refresh/reload your browser.

```css 
.orange {
  color: darkorange;
}
```

What changed?

Notice that this time, to reference our `orange` class, we prefixed the class name with a period (`.`).

Classes can be used to identify a subset of elements, but IDs are only for a single element. Each ID should be used only once per page.

Add an `id` attribute with the value of `fancy` to one of your `p` elements.

```html
<p id="fancy">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem consequatur unde aut dolores odio hic, accusamus recusandae ipsam illum enim voluptatibus obcaecati totam tempora eum quod sapiente. Corporis, quidem, culpa?</p>
```

Again, notice that we added this by simply putting `id="fancy"` inside the `p` tag.

Now, add an `id` of `ugly` to a different `p` element, then add the following code inside of `style.css`

```css
#fancy {
  font-family: "Brush Script MT", "Brush Script Std", cursive;
  color: deeppink;
}

#ugly {
  font-family: "Comic Sans MS";
  color: olive; 
}
```

Refresh or reload your browser again. What changed?

Just like how we referenced our classes with a leading `.`, we can reference ids with a leading `#`.

You can think of CSS specificity as a hierarchy! Your CSS properties will overlap based on those hierarchies.

For instance, let's say you have an `h1` element with the class of `new-text`.

```html
<h1 class="new-text">Specificity!<h1>
```

In your CSS, if you applied the color blue to the tag, `h1` and applied the color red to the class `new-text`

```css
.new-text {
    color: red;
}

h1 {
    color: blue;
}
```

Take a second to consider what color you think the word `Specificity!` will be.

<details>
  <summary>Click here to see the answer</summary>

  <p>We see the color red because targeting `classes` are more specific than `elements`.</p>

</details>

What would happen if we added an `id` of `green` to our example, and applied the color green to the tag?

```css
#green {
  color: green;
}
```

This would result in the word `Specificity!` being green.

This is because an `id` is a more specific reference to an element than a `class` is.

For more about CSS specificity, check out this [resource](https://www.w3schools.com/css/css_specificity.asp)!

---

### Assignment

For this assignment, we'll be creating an entirely new GitHub repository! Start by creating a new repository called, `prework-css`. Then clone the new repository to your local machine. Finally, copy and paste the HTML file from `prework-html`, the previous assignment.

Next, create a `style.css` file and link to it in your `<head>` section using a `<link>` tag.

Now, complete the following steps:

1. Add an `id` of `bio-image` to your image element.
2. Create a new `div` element with a class of `container`.
3. Move all of the code currently inside the `body` to be inside the new `div` you just created. Your code should have this general format:

```html
<!DOCTYPE html>
<head>
  <!-- meta, title, and link tags live here -->
</head>
<body>
  <div class="container">
    <!-- All of the HTML you created should be here -->
  </div>
</body>
```

**STOP**. We're finished modifying our HTML for this webpage. Take a breather before continuing on.

Now, we're going to add some CSS to our webpage. We'll add CSS section by section.

Create the following CSS to be applied to the `body`:

1. The background color is `#efeee7`.
2. The font used is `Georgia,"Times New Roman",Times,serif;`.
3. The font color is `#333333`.
4. Be sure to zero out the body margins and padding so the page is flush to the top of the page:
```css
body {
  margin: 0;
  padding: 0;
}
```

**STOP**. Take a deep breath. Refresh your page and see how the changes you've made have altered the style of your page.

When you're ready, continue on.

Create the following CSS to be applied to `h1` elements:

1. The background color is `#333333`.
2. The font color is `#eee`.
3. The font size is `28px`.
4. The margin is `0`.
5. The padding is `20px`.

**STOP**. We're rapidly getting there. Just a few more changes to make.

Create the following CSS to be applied to the following elements:

`h2` element specifications:

1. The font size is `24px`.

`a` element specifications:

1. The font color is `#d21034`.

`container` class specifications:

1. The width is `1024px`.
2. Set the margin to `0 auto`.

`bio-image` id specifications:

1. The width is `200px`.
2. The height is `200px`.

**STOP**. Open your page in Google Chrome. It should now look like this:

<p align="center">
     <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/css-activity.png" width="800" title="css-activity">
</p>

If it does, awesome work! If it doesn't, check back over the instructions and make sure you completed every step.

If you're having trouble, don't worry! This is brand new stuff, and you'll have lots of opportunities to perfect it. Just try to get it as close as you can.

Once you're satisfied with your webpage, we need to commit our changes with git and update our GitHub repository.

Remember, we do this by adding, committing, and pushing our changes.

1. `git add -A`
2. `git commit -m "Some message"`
3. `git push origin master`
