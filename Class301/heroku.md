## My summary of reading Heroku deployment.


# Deploy Your Blog to Heroku:

![Heroku](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQLePfgoRnn618tXPDQQoi3FHrhIcm8pUgR7w&usqp=CAU)

Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications.

1- Create a JavaScript file var http = require(“http”);

  http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
  }).listen(3000);

2- Run at your terminal: node server.js

3- Check it in your browser.

4- $.post(‘/some_requested_resource’, function(data){ console.log(data); });

5- Make it worldwide: heroku login

6- Declare some variables :

     var http = require("http");
     var fs = require("fs");
     var path = require("path");
     var mime = require("mime");

7- npm install

8- Create the HTTP server:

  var server = http.createServer(function(request, response) {
var filePath = false;

 if (request.url == '/') {
 filePath = "public/index.html";
 } else {
 filePath = "public" + request.url;
 }

 var absPath = "./" + filePath;
 serverWorking(response, absPath);
 });   
It’s Heroku time.
Do: git acp
heroku apps:rename myfirstserver
heroku open
# Responsive vs. Adaptive vs. Mobile:
* Responsive generally means to react quickly and positively to any change.

* Adaptive means to be easily modified for a new purpose or situation, such as change.

* Responsive design websites continually and fluidly change based on different factors, such as viewport width.

* Adaptive websites are built to a group of preset factors.

* Mobile means to build a separate website commonly on a new domain solely for mobile users.

# Flexible Layouts:

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.


# Flexible Grid:
Below we have a parent division with the class of container wrapping both the section and aside elements. The goal is to have have the section on the left and the aside on the right, with equal margins between the two.

# Media Queries:
Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.

# Logical Operators in Media Queries:
Logical operators in media queries help build powerful expressions. There are three different logical operators available for use within media queries, including and, not, and only.

# NOTE: START OF FLOAT SUMMARY

# What is “Float”?
Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. Here is an example of that.


# What are floats used for?
Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

# Clearing the Float
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.

# The Great Collapse
One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing. This isn’t always obvious if the parent doesn’t contain any visually noticeable background, but it is important to be aware of.

# Techniques for Clearing Floats
If you are in a situation where you always know what the succeeding element is going to be, you can apply the clear: both; value to that element and go about your business. This is ideal as it requires no fancy hacks and no additional elements making it perfectly semantic. Of course things don’t typically work out that way and we need to have more float-clearing tools in our toolbox.

1- The Empty Div Method is, quite literally, an empty div. <div style="clear: both;"></div> Sometimes you’ll see a <br> element or some other random element used, but div is the most common because it has no browser default styling, doesn’t have any special function, and is unlikely to be generically styled with CSS. This method is scorned by semantic purists since its presence has no contextual meaning at all to the page and is there purely for presentation. Of course in the strictest sense, they are right, but it gets the job done right and doesn’t hurt anybody.


2- The Overflow Method relies on setting the overflow CSS property on a parent element. If this property is set to auto or hidden on the parent element, the parent will expand to contain the floats, effectively clearing it for succeeding elements. This method can be beautifully semantic as it may not require additional elements. However if you find yourself adding a new div just to apply this, it is equally as non-semantic as the empty div method and less adaptable. Also bear in mind that the overflow property isn’t specifically for clearing floats. Be careful not to hide content or trigger unwanted scrollbars.


3- The Easy Clearing Method uses a clever CSS pseudo selector (:after) to clear floats. Rather than setting the overflow on the parent,

# What are floats used for?
Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

![Responsive Designs](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRNY4LAO1jkWpuf5V7yVWWY8Xr4fEWSf8LKrQ&usqp=CAU.)

# And that was it for this summary.