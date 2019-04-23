# Lesson \#2 - HTML

HTML documents are made up of tags. Most come in pairs, opening, and closing, but some are self-closing. 

Let's start by opening up an HTML file in VS Code and use emmet by typing `!` and pressing enter. Don't be alarmed by all of the text this created! In fact, only the elements inside the `<body>` tag will actually appear on the page. 

Let's dive right into some basic HTML tags starting with heading tags.

`h1` - `h6` are used to display headings. `h1` is the most important heading, `h2` would be sub-heading, and `h3` would be a sub-sub-heading. 

```html
<h1>Title</h1>
<h2>Sub-title</h2>
<h3>Caption</h3>
```

To test this out, right-click on your HTML file in the VS code workspace browser (located on the left). Select `copy path`, open a browser of your choosing and paste the path in the address bar!

By default, content written within `h1` tags will be the largest and content written within `h6` tags will be the smallest. But don't focus too much on the font sizes as we'll be able to change that later on with CSS. Instead, think of the heading tags in terms of importance! `h1` would be the most important and `h6` would be the least important.

Thinking of HTML tags in this way helps in a couple of different ways. For example, many people use screen readers and search engines like Google use bots that read websites and use the information they gather to index sites. It is *vital* that your HTML conveys the meaning of their content properly for these services to work correctly. 

Next, let's dive into a few more common tags: `p`, `ul`, `ol`, `li`, and `div`.

To start, `p` tags denote paragraphs. This is where you will house main content.

```html
<p>Hello World!</p>
```

For creating lists, we have `ul` and `ol` tags. `ul` or unordered tags will create a list of items using bullet points by default. `ol` or ordered tags will create a list of items that are automatically numbered starting from 1.

In order for you to add items to lists, you'll have to use the `li` tag which stands for list item. Ensure that as you add `li` tags that they are always wrapped within `ul` or `ol` tags.

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

Next, let's talk about the `div` tag. `div` or division tags are a way for us to tell HTML that we are creating a division or section within our HTML. This is a bit of a conceptual thing as `div` tags will not appear on our pages until we have actual content within the `div` tags!

```html
<body>
  <div>
    <p> This is where our Navigation bar will go!</p>
  </div>

  <div>
    <p>This is where our main content will go!</p>
  </div>

  <div>
    <p>This is where our footer will go!</p>
  </div>
</body>
```

As you can see, `div` tags helps us to keep our HTML separated and organized!

Now let's discuss links! We can create links by using what's known as anchor tags, `<a>`.

This particular HTML tag, however, requires an additional attribute. In other words, we need to tell our `<a>` tag where to send the user when they click on the link!

We do this by passing in an `href` attribute followed by the URL of the destination website.

```html
<a href="https://www.google.com">Click here to go to Google.com!</a>
```

Finally, let's discuss images.

Images in HTML are as simple as using the `<img>` tag. Just like the `<a>` tag, we'll need to pass in a special attribute. Specifically, that special attribute will handle the URL of the source image or a path to the image if we have downloaded an image to use.

```html
<img src='https://upload.wikimedia.org/wikipedia/commons/3/30/Googlelogo.png'>
```

Do you remember when we mentioned that many users utilize screen readers? What happens when a screen reader stumbles upon a picture? Will it simply read off the image URL or file path? Instead, we can use the `alt` attribute tag which stands for the alternate. Using the `alt` attribute we can describe what the image is!

```html
<img src='https://upload.wikimedia.org/wikipedia/commons/3/30/Googlelogo.png' alt='google-logo'>
```

Finally, there may be another thing you've noticed about the `img` tag. It doesn't have a closing tag! Remember when we said that most HTML tags come in pairs? Well, this is one of the exceptions. And as mentioned before, these are called `self-closing` HTML tags.

---

### Assignment

#### Instructions

Whew! Congratulations, you've just learned a ton of HTML! But now you'll be taking what you've learned and practicing it by completing an assignment.

Before you get started on the assignment, create a GitHub repository to store it. This is how you'll submit the assignment during class. But don't worry about sumbitting these assignments. They are here to help you practice what is covered during the prework!

As a reminder, these are the steps to create and clone a repository.

1. Create a new repository named `prework-html`. When creating the repository remember to make sure that the `Initialize this repository with a README` box is checked! By default it is unchecked.
2. Click on the green `Clone or download` button. Be sure that `Use HTTPS` is toggled. Then copy the link provided.
3. In terminal or GitBash, `cd` into the directory where you want your repo to live
4. Clone the repo using `git clone <repo name>`.

In the directory that you just cloned, create a basic HTML page with your own information that looks similar to the design below.

<p align="center">
     <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/prework-bio.png" width="600" title="demo">
</p>

Once you have the file created, commit your changes and push them to GitHub.

1. Open your terminal or GitBash if it's not already open
2. `cd` into the repo.
3. Stage the changes using `git add -A`
4. Commit the changes using `git commit -m "some message"`
5. Push the changes using `git push origin master`

If you're getting stuck on the GitHub section, be sure to look back at the video from our earlier lesson.

<p align="center">
  <a href="https://www.youtube.com/watch?v=seICQOd2qsY" target="_blank"><img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/git_thumb.png" width='400px'></a>
</p>
