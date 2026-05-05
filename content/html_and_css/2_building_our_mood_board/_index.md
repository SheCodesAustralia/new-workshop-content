---
title: "Building our Mood Board"
weight: 2
chapter: false
---
Every website on the internet uses HTML. If you're curious, it stands for Hyper Text Markup Language, and it’s the basic building blocks that tell web browsers how to show text, images, and links on a page. It was first created in the early 1990s, and every website you visit today still uses HTML at its core!

We can think of HTML as the structure of our page, letting our browser know where content should be found, and how we want to interact with it. Let's walk through some common **elements**.

Every element has a name, and is (usually) made up of an opening and closing tag, with the content we want displayed on the screen between them.

We've actually already written an element.
"Our First Webpage" used an `h1` tag, otherwise known as a heading tag.

![Annotated HTML Element showing opening and closing tags and content.](../images/element-tags.png)

For this tutorial let's start by adding some structure to our page. Go ahead and copy the below into your codepen window and then let's chat through what's happening.


```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>She Codes</title>
</head>

<body> <!-- Your content goes here -->
    <h1>[Your Name] Mood Board ❤</h1>
</body>
</html>
```
We have:
- A `head` element, to tell the browser **how** to display the page. It includes:
  - Some meta-information used to specify the character set our page will use, how big the browser window will be, etc. Because we're using Codepen, its actually taking a lot of that away from us needing to specify, but its good to get in the habit of for your next website.
  - The title that would be displayed in browser tab if we were publishing our page.
- A `body` element, to hold the code that will define the actual website contents that are displayed to the user.

Let's add some more sections to our website starting with our header.

```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>She Codes</title>
</head>

<body> <!-- Your content goes here -->
    <header> <!-- Your header section -->
        <h1>[Your Name] Mood Board ❤</h1>
    </header>
</body>
</html>
```

The `header` element is used for introductory content.
This is usually the main heading for the page and the navigation bar.

Next let's add a `main` section, which doesn't contain any content yet, but it will soon!!

```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>She Codes</title>
</head>

<body> <!-- Your content goes here -->
    <header> <!-- Your header section -->
        <h1>[Your Name] Mood Board ❤</h1>
    </header>
<main>
</main>

</body>
</html>
```
The `main` element represents the dominant content in the `body` of the page. Typically it would be 50-80% of your page.

Finally lets add in our footer, and we will add some content while we are here. 

```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>She Codes</title>
</head>

<body> <!-- Your content goes here -->
    <header> <!-- Your header section -->
        <h1>[Your Name] Mood Board ❤</h1>
    </header>
<main>
</main>

<footer>
    <p>Created with ❤ by Your Name</p>
</footer>

</body>
</html>
```
The `footer` element is used to identify the footer of a page.
It usually contains the copyright information or navigational elements.

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Try changing Your Name to say your name, your organisation, or leave a sassy message for your viewer. 

{{% /notice %}}

Woohoo! We've got a functional website. Technically we've got all the elements needed for a very basic website but... it's not very exciting. In the next section we will add some content, and then we will make some magic happen in the styling section.








