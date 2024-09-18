# Stage 2: Basic HTML Elements
In this stage of the workshop, you will learn about HTML elements in order to construct a basic functional web page.

You should have already completed the [previous stage](./stage1.md).

## What is an HTML element?
The ``html``, ``head``, and ``body`` sections that you created above are HTML elements, which are simply parts of a web page. An element may contain things such as text, an image, or nothing. Your typical element has an opening tag, some inner content, and a closing tag.

![anatomy-image](https://developer.mozilla.org/en-US/docs/Glossary/Element/anatomy-of-an-html-element.png)

[source](https://developer.mozilla.org/en-US/docs/Glossary/Element)

## Adding Elements
1. Open the ``index.html`` in the root of your local copy of this repository in a text editor of your choice.
2. In the body section, add a header element:
   ```html
   <body>
       <h1></h1>
   </body>
   ```
   - The header element is used for section headings.
   - There are six levels in total; ``h1``, ``h2``, ``h3``, ``h4``, ``h5``, ``h6``.
   - ``h1`` is the biggest while ``h6`` is the smallest.
3. Inside of the header element, insert your name:
   ```html
   <h1>John</h1>
   ```
4. Below the header element, create a new line, and insert a paragraph element with a short introduction.
   ```html
   <p>Hello! My name is John. It's nice to meet you!</p>
   ```
   - The paragraph element is used for paragraphs of text.
5. Save the file.

## Viewing the Page
As it is now, the web page is functional!
1. In a file explorer, navigate to the location of your ``index.html`` file.
2. Double click on it and open it in your preferred web browser.
3. The page should now open in your web browser and show your name & introduction!

## Lists
Let's add a list of your hobbies to the page now.
1. Open the ``index.html`` in the root of your local copy of this repository in a text editor of your choice.
2. On a new line below the ``<p>`` paragraph element that contains your introduction, place a 2nd header element with ``Hobbies`` as its content.
   ```html
   <h2>Hobbies</h2>
   ```
3. On a new line below the ``<h2>`` header element place the unordered list element.
   ```html
   <ul>
   </ul>
   ```
   - There is also an ordered list element ``<ol>`` for unordered data.
4. Inside the unordered list element, place multiple list item ``<li>`` elements containing your hobbies.
   ```html
   <ul>
     <li>Designing web pages</li>
     <li>Listening to music</li>
     <li>Going to the park</li>
   </ul>
   ```
5. Once you have added your hobbies, you can now save and reopen the ``index.html`` file in a web browser to view your changes.
   
## Final Code
Your ``index.html`` file should look like the following:
```html
<!DOCTYPE html>
<html>
    <head>
        
    </head>
    <body>
        <h1>John</h1>
        <p>Hello! My name is John. It's nice to meet you!</p>
        <h2>Hobbies</h2>
        <ul>
            <li>Designing web pages</li>
            <li>Listening to music</li>
            <li>Going to the park</li>
        </ul>
    </body>
</html>
```

## Stage Conclusion
You have now successfully added some HTML elements to your web page, making it functional!

In the next stage, you will add more HTML elements; images and hyperlinks.

[Next Stage](./stage3.md)