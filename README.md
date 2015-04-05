#Introduction

Tools to generate charts, graphs, plots are quite popular these days, and for good reason. They can help turn millions of numbers into something more tangible and understandable. [Knowledgent](http://knowledgent.com/infographics/data-viz-101/), a data analysis firm, says the following about data visualization:

```
A well-crafted data visualization helps uncover trends,
realize insights, explore sources, and tell stories.
```

Let's look at an example here. Of the two following (1) or (2), which one *appears* to be more meaningful than the other?:

(1)
```ruby
preferences =
{"beer1"=>[24, 25],
 "beer2"=>[57, 59],
 "beer3"=>[41, 38],
 "beer4"=>[46, 48],
 "beer5"=>[77, 80],
 "beer6"=>[72, 67],
 "beer7"=>[14, 11],
 "beer8"=>[84, 79],
 "beer9"=>[34, 39],
 "beer10"=>[20, 19],
 "beer11"=>[21, 16],
 "beer12"=>[73, 69],
 "beer13"=>[35, 40],
 "beer14"=>[83, 85],
 "beer15"=>[40, 45],
 "beer16"=>[10, 11],
 "beer17"=>[71, 68],
 "beer18"=>[45, 50],
 "beer19"=>[56, 54],
 "beer20"=>[20, 23]}
```

(2)
![alt](http://i.imgur.com/wpG6PCp.png)

Each point in the scatter plot is a comparison of two user's beer ratings of a particular beer. The *x* coordinate is the rating of a particular beer for me and the *y* coordinate is the rating for that particular beer for you. Looks like we both like `beer8` (which is probably some really hoppy IPA if you're like me) a lot. Unless you have some impressive mental data visualization tools at your cognitive disposal, (2) provides some meaningful analysis quickly. Without (2), we would be harder pressed to glean something important from (1). Even though (1) and (2) *contain* the same data, the *representation* of that data makes the difference. Imagine if we had 1,000 beers to compare between one another or if we had a database of 1,000,000 users! Which approach would could help us say something meaningful? Let's figure out how we can take advantage of the data visualization tools out there.

This tutorial will cover the following

* What tools can I use to visualize data with html?
* How do I make a Rails API to deliver data I care about?
* How do I visualize the data from my Rails API?

##Part 1 - Scalable Vector Graphics
This section covers SVG, or *scalable vector graphics*, as an introduction to graphing data with html.

[Making Graphs Manually with SVG](01-svg.md)

##Part 2 - The Highcharts Javascript Charting Library
This section is an introduction to the [Highcharts](http://www.highcharts.com/) Javascript library and how we can use it to make nice looking charts from simple ones like bar charts to more complex ones like scatter plots.

[Highcharts](02-highcharts.md)

##Part 3 - Making a Rails API
This section will explain how to create a simple Rails API with the Rails API gem and ActiveModel Serializers. It reviews the basics of creating models, controllers and migrations but in the context of a namespaced API.

[Making a Rails API](03-rails-api.md)

##Part 4 - Highcharts with a Rails API
This section highlights connecting a Rails API with Highcharts. It covers data manipulation on both the server and client side to generate both bar and scatter plots from our Rails API.

[Hooking up your Rails API with Highcharts](04-rails-api-highcharts.md)
