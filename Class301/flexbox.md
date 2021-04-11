## My summary of reading the First reading about Responisve web designs.


# What is a mustache:

![Mustache](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASwAAACoCAMAAABt9SM9AAAAk1BMVEX/vQAAAAD/wAD/xAD/wgD/vwD/xQD/xwD1twAQCwB3WQDztgD5ugBSPQBGNAD0tgCNagCDYgDPmwDhqACVcACsgQA1JwDBkADUngDrsABzVgCjegAlGwBhSQBPOgC4igDSnQAeFgCbdgBBMQBaQwCBYQBLNwAwIwDdpAB2WAAgGAAXEQBpTwCZcwA5KgC3iQAqHwDvhfQeAAAEPklEQVR4nO3b63qiMBAGYCCToICKHBZRq1211W1dt/d/dQtarRaQABbQ53v/djDJkISEUEUBAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAR2c1XYEK6q/74BY/ohHTI4y028TJaeBGb6pWnETHWRi95XJlLBxLUEYYJ2EG3ri37K9eJiMuKufLrfoDJVhOVvOksIHfV8+8+hZLCeMsXKzP41YBr1Qud27SO4sa+OVrTQNbTbA7iR9k7jgR1p1USZdf/tIqeDgsW2nmJ1MVm4vLEshLDZs6IuOHc2gdo6knk7bpKWX6tKY8pedKVcecf8WRucyK89KGbC4KZx2eH/YzaKO6xWvN3PesHKjq2jyln42yw9RecsjmEoFqNZarKFsjdcIKls/mV3IQCT+zxZyrYd1NwdtE3FCb61f7GjjqLCxSa1L+XM+V+tY5BG5y4tRFodsknLfTfWhKfP9tRXZIcN25MgQ/zfQ41OrmBvZd6XmemVu18VxF1QiiIeEzmXRxEWbO7OcmUVfVpSKHqWuzZB2teKESVlqf3UacrShdSt6g0FhoyCQgbhanQDLUs/LLNfdrujbk6jQT2+6V7sUZjbaS7VfVraA36eBhTrnP+2Vttx25+npu9f2QMS15ozXG3L+/pFsfCXOemJde/VCw5HwUbSrJ9Q57pWnz89URnVZEu2EQks6ItD0iplMYDAtlKmL3Cl7Q9xwzKuqrXKFz958x/fzz2eqteRRe1Nzw/MCJBP5iOCvY7PJ+r+zFP2df7sTe7s4r1ORaNEkzp5mNaNxTS6arE269Np2TLEapfeSP4pr8065Wi/blKsJSXlE1b97KXEWr7kIP/HoU3W7Xh23yN3S1Wlptm9vPUKe+lYIEg1q1ZPiOU4smLr+1Q/BIyG6Bf1q3xEvc2lFYdHPzI55KHQ/UjmsvTWdKVSclz3/q1/hQXLd3xZBEg1WTuRryuxiCJyLjGFXO6qPCxe/PdzMEj5gp9RY9nVNhAWJr99WtDkRQdj2/JrNsqpabu+tWB6SU7CABld2U+ymvl+8Fc4u+H471os6hlUmVUeJMv0W47sif0xzFR9L0XPiymfyZa1tp5OcfQl84fCTH/ha7ahford41SyJlUmSmP25/meyR7CFVUmfi94ApvvR5xterApLOVj+gR0lVjCjo5zc6EpztU0T6d3/fbUd3/AhMp+lu/v56Z170EJE/y//2Bg8xV33HmRJcX9UnPowj62qCu4bD7mjHXBCJznybNdvbZkrD0z5XPvh4cZSHG3/fEFM2k2TCtoGS3kc4M/3EK4z3se/So2fqgBNjoePb495uOv01M7z5Rrv25I/yO4qi++vpx3JleP7IZKzdRxG3Fn9hI+J/yBGM8lvO6fDfO3LRAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABD7DwtxN96coKCFAAAAAElFTkSuQmCC)

Mustache is a simple template system that you can use when building websites and web apps. By using a template system, you can keep your back-end code separate from the markup that displays the front end to the user. This clean separation gives you many advantages. For example, it makes it easy for a designer to work on a website’s visual design without the risk of messing up the site’s code. It also makes it easy for you to change the design at a later point without impacting the back-end code.

# Templating with Mustache
JavaScript templating is a fast and efficient technique to render client-side view templates with JavaScript using a JSON data source
1- Template is HTML markup, with added templating tags that will insert variablesor run programming logic

2- Template engine then replaces variables and instances declared in a template file with actual values at runtime, and 

3- convert the template into an HTML file sent to the client

4- Moustache: a logic-less template syntax, works by expanding tags in a templateusing values provided in a hash or 
object- Logic-less because there are no if statements, else clauses, or for loops, instead there are only tags
mustache.js is implementation of the mustache template system in JavaScript

5- Mustace is not a templating engine, but a specification for a templating language

6- If you use mustache with Node and Express, you can use mustache-expresseans to build a separate website commonly on a new domain solely for mobile users.

# Flexbox:

Flexbox is a single dimensional layout, which means that it lays items in one dimension at a time, either as a row, or as a column, but not both together. This can be opposed to the two-dimensional model - CSS Grid Layout, which lays the items in two dimensions simultaneously (rows and columns together).

* Parent element (flex container)
EXAMPLE

.container {
display: flex; /* or inline-flex */
}

* Child element (flex items)
EXAMPLE

.item {
order: 5; /* default is 0 */
}

# Features of Flexbox
Following are the notable features of Flexbox layout −

1- Direction − You can arrange the items on a web page in any direction such as left to right, right to left, top to bottom, and bottom to top.

2- Order − Using Flexbox, you can rearrange the order of the contents of a web page.

3- Wrap − In case of inconsistent space for the contents of a web page (in single line), you can wrap them to multiple lines (both horizontally) and vertically.

4- Alignment − Using Flexbox, you can align the contents of the webpage with respect to their container.

5- Resize − Using Flexbox, you can increase or decrease the size of the items in the page to fit in available space. 

# The CSS Flexbox Items Properties
align-self Specifies the alignment for a flex item (overrides the flex container’s align-items property) flex A shorthand property for the flex-grow, flex-shrink, and the flex-basis properties flex-basis Specifies the initial length of a flex item flex-grow Specifies how much a flex item will grow relative to the rest of the flex items inside the same container flex-shrink Specifies how much a flex item will shrink relative to the rest of the flex items inside the same container order Specifies the order of the flex items inside the same container



![FLEXBOX](data:image/png;base64,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)

# And that was it for this summary.