# jCharts v3



Version 3 of jCharts is a complete rewrite from the ground up, with a focus on data flexibility. Key features include:

  - jQuery plugin format
  - Optional data-table conversion for creation
  - Post creation data adjustments

jCharts is a pure javascript implementation of a variety of animated charts and graphs. 

![alt tag](https://raw.githubusercontent.com/dburrell/jCharts/master/images/charts.png)

### Current Status
In Development - no stable releases

### Usage

The most straight forwards usage is to simply give it a table of data to work with and let it do its thing, e.g. given an html table with data as below:

| -     | Maths | History |
|-------|-------|---------|
| Alice | 53    | 78      |  
| Bob   | 90    | 33    |  


You could then use this code:
```sh
var g = $("#dataTable").jChart();   // Automatically convert the table
```

There are then various adjustments that can be made to the data afterwards if required:
```sh
g.addSeries("Chemistry");            //add another data series

g.addRecord("Charlie",[80,23,70]);   // add a whole new record (with optional values)

g.set("Alice","Chemistry",85);       // adjust the (currently null) value of Alice's Chemistry score
g.set("Bob","Chemistry",88);         // adjust the (currently null) value of Bob's Chemistry score
```


Theme
----
It should be noted that the website theme for jcharts.net is based on Jason Long's architect theme (https://github.com/jasonlong/architect-theme) released under creative commons. This is *not* used within the main Jcharts package.


License
----

GNU GPL v2

This project is released *completely free* under the GNU GPL v2 license which, amongst other things, prevents any liability to the creator for any damages caused.
