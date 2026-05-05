---
title: "Headings"
weight: 1
chapter: false
---

Let's dive a little deeper into headings.

So far we've just used an `h1`.
This is what we would call the **top level** heading, and there is usually only one of these on the page.
We use this tag to show the main title for the page.

To break up the page into further sections, we can use the rest of the heading elements, `h2`, `h3`, `h4`, `h5` and `h6`.

`h1` is used for the title of our page, for example, “About Us”.
`h2` headings are often used for sections (e.g. Mission, Values, Vision) and so on.
A sub-heading under ‘Values’ would use an `h3` heading element. 

For example:

```html

<body> <!-- Your content goes under here -->
    <main>
        <h2>2026</h2>
        <h3>Personal Goals</h3>
    </main>
</body>
</html>

```

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Try adding the above `h2` and `h3` headings to your page.

{{% /notice %}}

This should be the resulting page:

![Screenshot of webpage with h1, h2 and h3 elements.](../../images/moodboard-screenshot.png)

## Paragraph text

Let's add some text to our site. The `<p>` tag is one of the most used HTML elements, and represents paragraph text. If your text isn't a heading, it should probably be wrapped in a `<p>` tag.

Let's add a line of paragraph text in our `<header>`. This should go directly under the `<h1>` we wrote earlier.

```html

<p>A place for inspiration and creativity</p>

```

A bit further down let's add some text into our `main` replacing our `h3` 

```html
<p>“Creativity takes courage.”</p>

```

## Check your code

```html 

<head>
    <meta charset="UTF-8">
    <title>She Codes</title>
    <link rel="stylesheet" href="./styles.css">
</head>

<body> <!-- Your content goes under here -->
    <header>
        <h1>[Your Name] Mood Board ❤</h1>
        <p>A place for inspiration and creativity</p>
    </header>

    <main>
        <h2>2026 IS MY YEAR</h2>
        <p>“Creativity takes courage.”</p>
    </main>

    <footer>
        <p>Created with ❤ by [Your Name]</p>
    </footer>

</body>

</html>

```


