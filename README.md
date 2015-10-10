## Website Performance Optimization portfolio project

#### Part 1:
- How to run:
  1. Check out the repository
  1. Run a local server

    ```bash
    $> cd /path/to/your-project-folder
    $> python -m SimpleHTTPServer 8000
    ```

  1. Open a browser and visit http://localhost:8000
  1. Download and install [ngrok](https://ngrok.com/) to make a public link to localhost temporarily

    ``` bash
    $> ngrok 8000
    ```

  1. Copy the public link to [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) and analyze it

- Optimizations
  * Resized images
  * Minimized images
  * Minimized CSS and make style.css and Google Fonts CSS inline
  * Added media attribute to print.css
  * Minimized JS
  * Put JS just before the end of body tag
  * Added async attribute to analytics.js



#### Part 2:
- How to run:
  1. Check out the repository
  1. Run a local server

    ```bash
    $> cd /path/to/your-project-folder
    $> python -m SimpleHTTPServer 8000
    ```

  1. Open a browser and visit http://localhost:8000/views/pizza.html
  
- Optimizations
  * Query `#randomPizzas` outside the loop
  * Get the `document.body.scrollTop` outside the loop
  * Query all `.randomPizzasContainer` outside the loop
  * Optimized `changePizzaSizes()` function by finding the size using simple switch case and assign to all `.randomPizzasContainer`
  * Added `will-change: left;` to `.mover` style
  * Query `#movingPizzas1` outside the loop

- Extra
  * Added X-Large to Pizza size