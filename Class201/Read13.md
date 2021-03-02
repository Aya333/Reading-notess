# Local storages:
![LOCAL-STORAGE](images/Local.jpg)


Local storages are provided by operating systems to store and retrieve data. Back in the days when web was first inveted web applications did not have any local storages but instead they used cookies which were early in the game. But that wasn't very useful 
as it was used for small amounts of data and it has a few problems
that made it in efficient such as:

 1- Cookies were included with every request to the server which has made the process slower than ever as it sends the same data over &over again.

 2- Following the previous problem data were sent unencrypted over the web unless they were sent over the **Secure Socket Layer** so, basically your data was not secured and if it continued in our current days things would have been much easier to steal.

 3- Limited to about 4kb of data which slowed down the whole process.

 ## Before HTML5:
  In the beginnig Microsoft has invented Internet Explorer with many features embeded inside of it as it wasn't just a web browser One of these things was called DHTML Behaviors, and one of these behaviors was called userData.
      
      - Userdata: Allows webpages to store up to 64KB of data  & up to 10 times in trusted domains such as intranet. Also it doesn't display permission forms therefore it is lighter to load.

  In 2002 Adobe had invented "Flash6" and it was introduced by others as "Flash cookies"; it allowed webpages to store up to 100KB of data per-domain, as the owner of adobe Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System), but it was limited by some of Flash’s design quirks." By 2006, due to the rapid changes in technology and the web world Brad re-wrote his "AMASS" and integrated it into "DojoToolkit". It provides free 100KB of data storage for each single domain.

  In 2007 Google launched "Gears"; which provided an API to embed SQL data bases in the browser which in return can store unlimited amounts of data.

  In 2009 Brad Neuberg and others kept working on improving dojox.storage until it was able to provide a unified interface on top and auto-detect Adobe Flash, Gears, Adobe AIR from the browsers;

  After HTML5 Storage was introduced which was a part of the HTML5 specification but it was split later on into it's own specification. Also called "Local storage & DOM storage" in some browsers, it's almost a database on the clients' side to store specific data in pairs (key&value). It keeps on persisting even after you exit your browser & unlike cookies it is not transmitted remotely.

  ## How to use HTML5 storage:
   1- HTML5 storages only store string data so in case you wanted to store anything that is not a string then you need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

   2- Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null.

   3- To remove a value you can use the following function:
   interface Storage {
   deleter void removeItem(in DOMString key);
   void clear();
   };

   4- To get the total number of values in the storage area then you will need to se the following function:
    interface Storage {
    readonly attribute unsigned long length;
    getter DOMString key(in unsigned long index);
    };

    5- To keep track of the changes made on your local storage "Programmatically" you can use the storage events:
      if (window.addEventListener) {
      window.addEventListener("storage", handle_storage, false);
       } else {
      window.attachEvent("onstorage", handle_storage);
      }; 
      
      And to handle it you can use:
      function handle_storage(e) {
      if (!e) { e = window.event; }
      }

   We can check whether the data is stored in local storage by using the developer tools that comes with the browsers. For instance, in Chrome, right click on the browser and select Inspect Element. Select Resources tab and then click on the local storage item. We can see the user selected data stored in the form of key/value pairs.

   The web page can be reloaded with the background and font size values set by the user. The getItem(‘Key’) helps in retrieving the data stored In the database.
 
 ## And that was it for this summary.
