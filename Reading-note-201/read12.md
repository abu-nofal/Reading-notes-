# what’s Chart.js? 

Chart.js is a community maintained open-source library (it’s available on GitHub) that helps you easily visualize data using JavaScript. It’s similar to Chartist and Google Charts. It supports 8 different chart types (including bars, lines, & pies), and they’re all responsive. In other words, you set up your chart once, and Chart.js will do the heavy-lifting for you and make sure that it’s always legible (for example by removing some uncritical details if the chart gets smaller).

In a gist, this is what you need to do to draw a chart with Chart.js:

1. Define where on your page to draw the graph.

2. Define what type of graph you want to draw.

3. Supply Chart.js with data, labels, and other options.

…and you’ll get a beautiful, responsive, graph! Although we won’t dig too deep into changing the design of our graph in this tutorial, Chart.js graphs are highly customizable. As a rule, whatever you see you can affect, and although the charts look good without much customization, you’ll likely be able to realize all your (or someone else’s) design visions with some extra effort.

> Step 1: Add Chart.js 

First of we need to add Chart.js to our page so that we can use the library. For this project, I’ve prepared a simple playground with a HTML file with only the essentials. Download the starting point and open the folder, and you should see three files: 

- index.html
- styles.css
- app.js

I’ve added some basic styling to style.css, but script.js is completely empty—this is where we’ll add the code to draw our graph in a moment. For now, open up index.html in a text editor. To use Chart.js we need to link to the library inside of our head. You could download the library and host it yourself, but the easiest (and probably fastest) way is to just use a CDN (content delivery network, in this instance a fancy way of saying “nice people who’re hosting the libraries we need”).

If you go to chartjs.org and click on Documentation, you’ll see a link to their recommended CDN. Follow the link, and look for the URL ending with Chart.min.js. At the time of this writing, the latest version is 2.5.0:

`<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.5.0/Chart.min.js"></script>`

Copy and paste this row onto row 5 in index.html. After pasting, your head should look like so:

> `<body >`
  `<footer></footer>`
  `<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.5.0/Chart.min.js"></script>`
`</body>`

## canvas 
> Step2 :Prepare a place in your HTML to render the chart 

The last thing we need to prepare before we can start visualizing our data is to define an area in our HTML where we want to draw the graph. For Chart.js you do this by adding a **canvas** element, and setting **width** and **height** to define the proportions of your graph.

On row 13 in index.html, copy and paste this row to create your canvas element:

`<canvas id="myChart" width="1600" height="900"></canvas>`


Notice that we’ve added an id (myChart) to the canvas element that we can later use to reference our designated graph element in JavaScript or CSS. What this ID is set to has no significance for Chart.js; you can name it whatever you want. What matters is that you use the exact same ID when you reference it in JavaScript or CSS. If you’re adding several graphs to a page, just make sure that every ID is unique (you could for example give your graphs more specific names, like populationChart or regionChart).

> Step 3: Prepare the data

the data you have and you want to add it into the chart 

> Step 3: Draw a line! 

At last! We’ve arrived at the moment of truth. Visualizing data with Graph.js is pretty straightforward. All we need to do is define what graph we want to draw, and pass in the data that we want to visualize. Let’s start by drawing one single line to see if we can get it to work: below the data that you just pasted into **script.js**, add these lines of JavaScript:

> `let ctx = document.getElementById("myChart");`
`let myChart = new Chart(ctx, {
  type: 'line',
  data: {
    labels: years,
    datasets: [
      { 
        data: africa
      }
    ]
  }
});`

…open up **index.html** in a browser, refresh and… tada! You created a graph! It’s not the prettiest, but hey, it’s rising and it’s looking all professional!

What’s happening in this bit of code? Let’s break it down. First, we locate the canvas element that we added earlier to our index.html file (notice "myChart"):

> `var ctx = document.getElementById("myChart");`

Then, using that **canvas** element, we create a line chart **(type: 'line')**, and pass along some of our **data. labels:** years sets our array of years (that we created earlier) for the labels along the x-axis, and data: africa uses our africa variable to draw the line.

For every line that we want to create, we add another object to the datasets array. On every object we can make a range of adjustments: we can not only pass the data to draw the line, but we can change the name, change the beavior, and change the looks of the line.

Let’s try that right now. You may have noticed that our line is missing a label (it says undefined at the top of the graph), and it’s not very colorful. Boo! Let’s make it ✨👌