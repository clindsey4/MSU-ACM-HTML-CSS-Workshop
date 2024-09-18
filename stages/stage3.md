# Stage 3: Images & Links
In this stage of the workshop, you will learn about the anchor and image HTML elements.

You should have already completed the [previous stage](./stage2.md).

## Links
The two elements we will be creating in this stage of the workshop will require a link to be provided to them.

This link can either be a direct link to a location on the internet, or a relative path (to a local file).

## Local Image Elements
1. Open the ``index.html`` in the root of your local copy of this repository in a text editor of your choice.
2. Above the ``<h1>`` element with your name, create a new line and type the following to create an image embed.
   ```html
   <img src="assets/acm-logo.png" alt="An image depicting the logo of the ACM."/>
   ```
   - The ``<img>`` is a kind of element that doesn't require a closing tag, since it doesn't have any inner content.
   - The ``src`` attribute is the path to the image that you want to embed.
   - The ``alt`` attribute is shown when the image is loading/failed to load. It also is useful for screen readers and accessibility.
3. Save and open the ``index.html`` file in a web browser, you should see the ACM logo at the top of the page above your name.

## Internet Image Elements
1. Open the ``index.html`` in the root of your local copy of this repository in a text editor of your choice.
2. Above the previous image with the ACM's logo, create a new line and type the following to create an image embed.
   ```html
   <img src="https://www.vangoghgallery.com/img/starry_night_full.jpg" alt="The Starry Night by Vincent Van Gogh." width="256"/>
   ```
   - The ``width`` attribute defines the width (in pixels) of the image.
3. Save and open the ``index.html`` file in a web browser, you should see "The Starry Night" at the top of the page.

## Anchor Elements
1. Open the ``index.html`` in the root of your local copy of this repository in a text editor of your choice.
2. Below and outside of the ``<ul>`` element where you added your hobbies, create a new line.
3. Create an anchor element and set the value of the ``href`` attribute to a link to your favorite website.
   ```html
   <a href="https://www.google.com">My Favorite Website</a>
   ```
4. Save and open the ``index.html`` file in a web browser.
5. If you click on the text at the bottom of the page that says ``My Favorite Website``, you should be navigated to your favorite website.

## Final Code
Your ``index.html`` file should look like the following:
```html
<!DOCTYPE html>
<html>
    <head>

    </head>
    <body>
        <img src="https://www.vangoghgallery.com/img/starry_night_full.jpg" alt="The Starry Night by Vincent Van Gogh." width="256"/>
        <img src="assets/acm-logo.png" alt="An image depicting the logo of the ACM."/>
        <h1>John</h1>
        <p>Hello! My name is John. It's nice to meet you!</p>
        <h2>Hobbies</h2>
        <ul>
            <li>Designing web pages</li>
            <li>Listening to music</li>
            <li>Going to the park</li>
        </ul>
        <a href="https://www.google.com">My Favorite Website</a>
    </body>
</html>
```

## Learn More
If you are interested in adding more elements to your page outside of the ones covered in this workshop, visit [Mozilla's HTML elements reference page](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) which contains descriptions and examples for a wide array of HTML elements.

## Stage Conclusion
You have now successfully added some images and a hyperlink to your web page!

In the next stage, you will learn how to style your web page with CSS.

[Next Stage](./stage4.md)

