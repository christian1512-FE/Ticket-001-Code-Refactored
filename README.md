# Ticket-001-Code-Refactored
Module 1 Challenge Project 

## Description

The purpose of this project is to learn how to take existing code and improve it by
refactoring it without changing its functionality. The main problem the original code had were accessibility barriers, in which makes it difficult for people with disabilities to use the website. 

## Usage

Provide instructions and examples for use. Include screenshots as needed.

To add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative file path, add it to your README using the following syntax:

![alt text](assets/images/screenshot.png)

## HTML Code Improvements

In order to improve the codes web accessibities I changed the non-semantic elements to semantic elements, added alt attributes to images, and fixed links that werent working properly on the website.


Modifications to the HTML code. 

Changed the name of the website on the "head" element changed the title of the website to "Horiseon Social Solution Services"

*Added the <header> element in which is used to represent introductory content. 

*Changed <div> tag to <header>

*Changed <h1>Hori<span class="seo">seo</span>n</h1> to <h1>Horiseon</h1>
just a simple header name to help the websites accessiblity. 

*Changed the <div> tag to <nav> element in which is used to provided navigation to links. 

*Added the <main> element in which is used represent the main content on the website.

Changed the <div> class to <section> class the section element in which is used defines a section on the website.

*Changed the <div class="content"> to <section class="content">

*Changed <div class="search-engine-optimization"> to <section id="search-engine-optimization" also added class="search-engine-optimization"> in which it  fixes the link that was not working on the website. 

*Added <alt> attributes to all of the images to increase the websites accessiblity. 

*Added the <aside> element in which represents secondarty content on the website.

*Changed the footers <div class> to <footer class>

*Changed the heading attribute <h2> on footer to <h4> so it falls in sequental order.



## CSS Code Improvements

CSS style sheet modifications. There were several modification I applied to the CSS style sheet such as grouping CSS selectors, deleting some CSS selectors, renaming CSS selectors and organizing the CSS selectors and properties to follow the semantic structure of the HTML elements. 


Renaming CSS selectors. 
As seen on the HTML sheet modifications I changed the <div> HTML element to <nav>.

  BEFORE                                       AFTER 
.header div        ------------------>      .header nav 
.header div ul     ------------------>      .header nav ul
.header div ul li  ------------------>      .header nav ul li 


Consalidated some of the selectors and properties of the CSS style sheet. This is very helpful when it comes time to make site maintance. Instead of having multiple sectors with the same style by grouping them I can apply the same style to different of elements. 

Below are the CSS selectors I combined:

.search-engine-optimization, .online-reputation-management, .social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff; 

.search-engine-optimization img, .online-reputation-management img, .social-media-marketing img {
    max-height: 200px;


.search-engine-optimization h2, .online-reputation-management h2, .social-media-marketing h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.benefit-lead, .benefit-brand, .benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
} 

.benefit-lead h3, .benefit-brand h3, .benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
}


.benefit-lead img, .benefit-brand img, .benefit-cost img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}"

Deleted CSS selectors: 

This CSS selector was used for the <span> element in which is used to color part of the text. As seen on the HTML code improvements I deleted the class "seo" to improve the websites accessiblity. 

.header h1 .seo {
    color: #d9dcd6;
}

This CSS selector was used to give the footer <h4> font-size. Instead I added the font-size to the selector ".footer". 

.footer h2 {
    font-size: 20px;
}


## License

The MIT License (MIT)

Copyright (c) 2022 Christian Mendez

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


