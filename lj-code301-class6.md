# LJ Code 301 - Day 6

Today we learned about AJAX and JSON and how they work with each other.
AJAX stands for Asynchronous Javascript and XML, which is a mechanism used to launch asynchronous HTTP requests to a server using JavaScript. The most common way to retrieve data from the server is in JSON format. JavaScript reads the file and converts it into data objects.

```
$.getJSON( "ajax/test.json", function( data ) {  //how you can request JSON file.
};
```
```
{
  "one": "string",
  "two": "more strings" // how JSON file looks like, a lot like the object literal
}
```

Use XMLHttpRequest objects to interact with servers. You can retrieve data from a URL without having to do a full page refresh. This enables a Web page to update just part of a page without disrupting what the user is doing.  XMLHttpRequest is used heavily in Ajax programming.
