# Stage 1: Web Page Structure
In this stage of the workshop, you will learn about the structure of an HTML document.

## Creating an HTML file.
1. Navigate to your local copy of this repository.
2. In the same location as where the ``README.md`` file is located, create a new text file.
3. Rename the file to ``index.html``.
   - Make sure that the file is an HTML file, and not just a text file with the name ``index.html``

## What is HTML?
The file that you just created is an HTML (Hypertext Markup Language) file, which web browsers will read & interpret as a web page.

## HTML Structure
1. Open the ``index.html`` file in a text editor of your choice.
2. At the top of the file, type the following line:
   ```html
   <!DOCTYPE html>
   ```
3. Add the following on a new line below the previous one:
   ```html
   <html>
   
   </html>
   ```
4. On line 3, in-between ``<html>`` and ``</html>``, add the following: 
   ```html
   <head>
   
   </head>
   <body>
   
   </body>
   ```
6. Save the file.
   
## What is this?
You just created the basic structure for an HTML page. Every HTML page requires this basic layout.

- ``<!DOCTYPE html>``
  - This tells anything that is reading this file to expect an HTML document.
- ``<html></html>``
  - Anything in-between these two will be interpreted as part of the HTML document.
- ``<head></head>``
  - Anything in-between these will be metadata for the HTML document.
- ``<body></body>``
  - Anything in-between these will be what is displayed on the web page.

## Final Code
Your ``index.html`` file should look like the following:
```html
<!DOCTYPE html>
<html>
    <head>
    
    </head>
    <body>
    
    </body>
</html>
```

## Stage Conclusion
You have successfully created the skeleton of an HTML page.

In the next stage, you will build on top of this to create a functional web page.

[Next Stage](./stage2.md)