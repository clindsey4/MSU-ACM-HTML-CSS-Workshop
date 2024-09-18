# Stage 4: Styling Pages
In this stage of the workshop, you will learn how to style web pages using CSS.

You should have already completed the [previous stage](./stage3.md).

## Creating a CSS File
1. Navigate to your local copy of this repository.
2. In the same location as where the ``index.html`` file is located, create a new text file.
3. Rename the file to ``styles.css``.
   - Make sure that the file is a CSS file, and not just a text file with the name ``styles.css``

## Writing a CSS Rule
1. Open the ``styles.css`` file in a text editor of your choice.
2. Insert the following text into the file:
   ```css
   body {
       background-color: #242424;
   }
   ```
   - In English, this rule says "Set the background color of every element of type ``body`` to ``#242424``."
   - We use an HTML color here, which translates to a dark gray.
3. If you save the file and open ``index.html`` in a web browser, you will notice that nothing has changed. This is because we haven't linked the HTML and CSS files together yet.

## Linking CSS to HTML
1. Open the ``index.html`` file in a text editor of your choice.
2. At the top of the file, inside of the ``head`` element, add a ``<link>`` element.
   ```html
   <head>
       <link rel="stylesheet" href="index.css">
   </head>
   ```
   - The ``rel`` attribute tells the element what kind of relation to the HTML document the link is.
   - The ``href`` attribute is the location of this link. In our case, it is the relative path to the ``index.css`` file.
3. If you save the file and open it in a web browser again, you will notice that the background of the page is no longer white.

## CSS Specificity
When writing CSS rules, you can rein in your rules to be more specific by making use of specificity operators.

Earlier, we used ``body``, which will apply the rule you write to every HTML element of type ``body``. However, there are other specificity operators you can use.

- ``#`` ID Specificity
  - Every HTML element can have an ``id`` attribute.
  - IDs are unique, meaning only one element on the entire page should have a specific id.
  - For example, if we make an element that has a picture of a plant.
    ```html
    <img id='plant-picture' src='<path to plant picture>' alt='A picture of a potted plant.'/>
    ```
  - In CSS, we can write a rule that will only apply to this specific element like so:
    ```css
    #plant-picture {
        max-width: 256px;
    }
    ```
- ``.`` Class Specificity
  - Every HTML element can have a ``class`` attribute.
  - Classes are very similar to IDs, but multiple elements can share the same class. They are not unique.
  - You can use class specificity like so:
    ```css
    .plant-pictures {
        max-width: 256px;
    }
    ```

## Changing Text Colors
Now that the background of the page is darker, the text on the page is difficult to read.
1. Open the ``styles.css`` file in a text editor of your choice.
2. On a new line, create a new rule targeting ``h1``, ``h2``, ``p``, ``li``, and ``a`` elements.
   ```css
   h1, h2, p, li, a {
       color: white;
   }
   ```
   - This rule uses multiple selectors chained together with commas, and sets the color of any matching HTML elements to white.
3. Save the file and open ``index.html`` in a web browser, the text on the page should now be white.

## Inheritance
Some CSS properties are inherited from HTML elements' parents and ancestors.

In the previous step, we chained together multiple selectors to change the color of all of the text on the page, but what if we added an ``h3`` element to the page? We would have to manually go in and change the CSS.

We can avoid this using inheritance.
1. Open the ``styles.css`` file in a text editor of your choice.
2. Navigate to where you created the previous rule, and replace ``h1, h2, p, li, a`` with ``body``
   ```css
   body {
       color: white;
   }
   ```
   - Since all of the text on the page are a descendant of the ``body`` element, they will inherit this rule.
3. Save the file and open ``index.html`` in a web browser, the text on the page should still be white despite this change.
4. Since we already have a rule that changes the background color of the body, merge the two rules together.
   ```css
   body {
       background-color: #242424;
       color: white;
   }
   ```
   - After this, you should only have 1 rule in your ``style.css`` file.

## Modifying Text
Let's make your name stand out on the web page.
1. Open the ``index.html`` file in a text editor of your choice.
2. Navigate to the ``h1`` element where you have your name written.
3. Give the ``h1`` element a new ``id`` attribute with the value ``my-name``
   ```html
   <h1 id="my-name">John</h1>
   ```
4. Save the ``index.html`` file and open the ``styles.css`` file in a text editor of your choice.
5. On a new line, create a new rule targeting the element with the ``my-name`` ID which changes font size.
   ```css
   #my-name {
       font-size: 5em;
       font-family: "Arial";
   }
   ```
   - This rule changes the font size of an element that has an ID attribute with the value ``my-name`` to 5em and change its font to Arial.

## Final Code
Your ``index.html`` file should look like the following:
```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="index.css">
    </head>
    <body>
        <img src="https://www.vangoghgallery.com/img/starry_night_full.jpg" alt="The Starry Night by Vincent Van Gogh." width="256"/>
        <img src="assets/acm-logo.png" alt="An image depicting the logo of the ACM."/>
        <h1 id="my-name">John</h1>
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

Your ``index.css`` file should look like the following:
```css
body {
    background-color: #242424;
    color: white;
}

#my-name {
    font-size: 5em;
    font-family: "Arial";
}
```

## Learn More
There are hundreds more CSS properties you can change outside of the ones that we just covered.

If you want to learn more about CSS in order to style your page more, visit [Mozilla's CSS reference page](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

## Workshop Conclusion
You have now successfully learned the basics of HTML & CSS!

Feel free to make further changes to your page as you desire!

If you want to continue, here are some page ideas:
- A resume.
- A page showing how to make your favorite recipe.
- An informational page about your favorite game.
- A guide to one of your hobbies.

[Back Home](../README.md)

