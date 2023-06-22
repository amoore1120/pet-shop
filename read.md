#   ** Pet Shop project while @ Kable Academy **

##   ** Requirements **
  __ NavBar & Footer should be the same on all pages
  __ contact page
  __ landing/home page 
  __ about me page

#   ** font-awesome icons **
cart        <i class="fa-solid fa-cart-shopping"></i>
shop        <i class="fa-solid fa-shop"></i>
dog         <i class="fa-solid fa-dog"></i>
text        <i class="fa-solid fa-message-text"></i>
call        <i class="fa-solid fa-phone"></i>
map W/dot   <i class="fa-solid fa-map-location-dot"></i>







#   ** max height & width **
If you want to use the body element as a smaller container and let the HTML element fill the page, you could set a max-width value on the body.

Here's an example:

html { background-color: #000; } 
body {
    min-height: 100vh;
    max-width: 400px;
    background-color: papayawhip; 
    margin: 0 auto;
}



###   ** How to Set the Page for Full Width **
Maybe just don't.

Not setting a width on the HTML and body elements will default to the full size of the screen. If you do set a width value other than auto, consider utilizing a CSS reset first.

Remember, by default the body element has 8px of margin on all sides.

A CSS reset removes this. Otherwise, setting the width to 100% before removing the margins will cause the body element to overflow. Here's the CSS reset I use:

* { 
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

##   ** How to Set Width to Your Preference **
While it may not always be necessary to set a width, I usually do.

It may simply be a habit.

If you set the width to 100% on the body element you will have a full page width. This is essentially equivalent to not setting a width value and allowing the default.

If you want to use the body element as a smaller container and let the HTML element fill the page, you could set a max-width value on the body.

Here's an example:

html { background-color: #000; } 
body {
    min-height: 100vh;
    max-width: 400px;
    background-color: papayawhip; 
    margin: 0 auto;
}
Conclusion
With no height value provided for the HTML element, setting the height and/or min-height of the body element to 100% results in no height (before you add content).

However, with no width value provided for the HTML element, setting the width of the body element to 100% results in full page width.

This can be counterintuitive and confusing.

For a responsive full page height, set the body element min-height to 100vh.

If you set a page width, choose 100% over 100vw to avoid surprise horizontal scrollbars.






##   ** Sticky Footer using Flexbox **
 <body class="d-flex flex-column">
        <div id="page-content">
          <div class="container text-center">
            <div class="row justify-content-center">
              <div class="col-md-7">
                <h1 class="fw-light mt-4 text-white">Sticky Footer using Flexbox</h1>
                <p class="lead text-white-50">Use just two Bootstrap utility classes and three custom CSS rules and you will have a flexbox enabled sticky footer for your website!</p>
              </div>
            </div>
          </div>
        </div>
        <footer id="sticky-footer" class="flex-shrink-0 py-4 bg-dark text-white-50">
          <div class="container text-center">
            <small>Copyright &copy; Creature Comfort Pawtique</small>
          </div>
        </footer>
      </body>