# Chart.js and Canvas

## Index

 [Home](README.md)  
 [JavaScript Canvas](#javascript-canvas)  
 [Chart.js Documentation](#chartjs-documentation)  
 [Easily Create Stunning Animated Charts with Chart.js](#easily-create-stunning-animated-charts-with-chartjs)  

## [JavaScript Canvas](https://www.javascripttutorial.net/web-apis/javascript-canvas/)

1. What does the `<canvas>` allow a developer to acheive?
   - 2D Charts and graphs.
2. What is the importance of the closing `</canvas>` tag?
   - Any content between the opening and closing tags is fallback content that will display only if the browser doesn’t support the `<canvas>` element.
3. Explain what the `getContext()` method does.
   - The `<canvas>` element features the `getContext()` method that returns a render context object.  
   The `getContext()` takes one argument which is the type of context. For example, you use the `2d` to get a 2D rendering context object, which is an instance of the `CanvasRenderingContext2D` interface.  
   The 2D rendering context allows you to draw shapes, text, images, and other objects.  
   The following example shows how to select the canvas element using the `querySelector()` method and access the drawing context by calling its `getContext()` method:

   ```js
   let canvas = document.querySelector('#canvas');
   let ctx = main.getContext('2d');
   ```

## [Chart.js Documentation](http://www.chartjs.org/docs/)

1. What is Chart.js and how it can be brought into your project?
   - Chart.js is a free JavaScript Library used to make HTML-based charts. You can get the latest version of Chart.js from [npm](https://www.npmjs.com/package/chart.js) , the [GitHub releases](https://github.com/chartjs/Chart.js/releases/tag/v3.8.2), or use a [Chart.js CDN](https://www.jsdelivr.com/package/npm/chart.js). Detailed installation instructions can be found on the [installation page](https://www.chartjs.org/docs/latest/getting-started/installation.html).
2. List 3 different Chart types you can create using Chart.js.
   - [Area Chart](https://www.chartjs.org/docs/latest/charts/area.html)
   - [Bar Chart](https://www.chartjs.org/docs/latest/charts/bar.html)
   - [Bubble Chart](https://www.chartjs.org/docs/latest/charts/bubble.html)
   - [Doughnut and Pie Charts](https://www.chartjs.org/docs/latest/charts/doughnut.html)
   - [Line Chart](https://www.chartjs.org/docs/latest/charts/line.html)
   - [Mixed Chart Types](https://www.chartjs.org/docs/latest/charts/mixed.html)
   - [Polar Area Chart](https://www.chartjs.org/docs/latest/charts/polar.html)
   - [Radar Chart](https://www.chartjs.org/docs/latest/charts/radar.html)
   - [Scatter Chart](https://www.chartjs.org/docs/latest/charts/scatter.html)

## [Easily Create Stunning Animated Charts with Chart.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

1. What are some advantages to displaying data via a chart over a table?
   - Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly.
2. How could Chart.js aid your previously created applications visually?
   - When creating the tables for sales data in the cookie-stand project, charts could have greatly imporoved the understanding of the data.  The totals were easy to derive but the comparisons between the different stores were nearly impossible to make without first studying the information. Charts could make that understanding come quick as a whip.

[Back to Top](#index)
