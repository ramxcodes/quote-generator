### Quote Generator

The "Quote Generator" web page allows users to view random quotes and their respective authors. The page has a simple and clean design with a quote icon and a button to generate a new quote.

#### HTML Structure

1. `<!DOCTYPE html>`: The document type declaration.
2. `<html dir='ltr' lang='en-GB' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>`: The opening tag for the HTML document, with the language set to English (en-GB) and some additional namespaces.
3. `<head>`: Contains meta-information about the document and links to external resources.
   - `<meta content='width=device-width, initial-scale=1' name='viewport'/>`: Sets the viewport for mobile devices.
   - `<link ...>`: Link to the Font Awesome CSS file (version 6.0.0-beta2) hosted on the Cloudflare CDN, used for icons.
   - `<title>Quote Generator by Ram</title>`: The title of the web page, displayed in the browser's title bar.
   - `<style ...>`: Contains the CSS styles for the page, including styles for the quote container, content, and button.
   - `<script ...>`: Includes the Clipboard.js library for copying content to the clipboard.
   - `<meta ...>`: Various meta tags for the page's metadata and Google AdSense configuration.

4. `<body>`: Contains the visible content of the web page.
   - `<div class='header no-items section' id='www.jobianstechie.tk'></div>`: A header section with no items and an ID attribute.
   - `<div class='quote-container'>`: A container for the quote and its related elements.
     - `<div class='quote'>`: Contains the quote content, author, and the "New Quote" button.
       - `<div class='quote-icon'>`: An SVG icon (quote icon) displayed beside the quote.
       - `<div class='quote-content'>`: Displays the quote content. Initially, it shows "Loading Quote... Created By Ram".
       - `<div class='quote-author'>`: Displays the author of the quote.
       - `<button class='new-quote-btn'>`: The "New Quote" button.
         - `<span></span>`: Four empty spans used for animation effects on the button.

5. `<p id="footer">`: A paragraph displaying credits and a link to the author's portfolio.
   - `Made with 💖 <a href="https://ramxcodes.github.io/portfolio/" target="_blank"><span style="color: #02d81e; "><b>Ram</b></span></a>`: The text "Made with 💖" and a link to the author's portfolio with the name "Ram".

6. `<script>`: Contains JavaScript code responsible for fetching and displaying random quotes.
   - The script uses the quotable.io API to fetch random quotes (with a maximum length of 100 characters).
   - The "New Quote" button triggers the nextQuote() function to fetch and display a new quote.
   - The JavaScript code makes use of the Clipboard.js library for copy functionality (not used in the provided code).

7. `<script>`: Loads the Blogger widgets and sets the data context for the page.

#### JavaScript Code

The provided JavaScript code is responsible for generating and displaying random quotes. It uses the quotable.io API to fetch a random quote (with a maximum length of 100 characters) and displays it on the web page.

The code initializes the quote content and the author's name, and when the "New Quote" button is clicked, it fetches a new random quote from the API and updates the content and author.

Note: The JavaScript code uses a font-awesome quote icon (a small SVG icon) and makes use of the Clipboard.js library for copying content to the clipboard (not used in the provided code).

The "Quote Generator" web page is designed to generate random quotes and provide users with a new quote on each button click. It also includes links to the author's portfolio and social media profiles in the footer.
