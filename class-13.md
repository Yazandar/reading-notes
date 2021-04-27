## Local Storage For Web Application

* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.

* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).

* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

* ```userData``` allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.

* ```HTML5 Storage``` is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons.

* ```HTML5 Storage``` it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server.

* From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object.

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

* HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like ```parseInt()``` or ```parseFloat()``` to coerce your retrieved data into the expected JavaScript datatype.

* If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever ```setItem()```, ```removeItem()```, or ```clear()``` is called and actually changes something.

* ```5 megabytes``` is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification.

* ```QUOTA_EXCEEDED_ERR``` is the exception that will get thrown if you exceed your storage quota of 5 megabytes.

* One vision is an acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:

```
openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});
```

* Most of the action resides in the string you pass to the ```executeSql``` method. This string can be any supported SQL statement, including ```SELECT```, ```UPDATE```, ```INSERT```, and ```DELETE``` statements. It’s just like backend database programming, except you’re doing it from JavaScript.

* ```SQL``` is more of a marketing term than a hard-and-fast standard. (Some would say the same of “HTML5,” but never mind that.) Sure, there is an actual SQL specification (it’s called SQL-92), but there is no database server in the world that conforms to that and only that specification. There’s Oracle’s SQL, Microsoft’s SQL, MySQL’s SQL, PostgreSQL’s SQL, and SQLite’s SQL. Indeed, each of these products adds new SQL features over time.

* The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database. There are ```databases``` with ```records```, and each record has a set number of ```fields```. Each field has a specific datatype, which is defined when the database is created. You can select a subset of records, then enumerate them with a ```cursor```. Changes to the object store are handled within ```transactions```.

* The primary difference is that the object store has no structured query language. You don’t construct a statement like ```SELECT * from USERS where ACTIVE = 'Y'```. Instead, you use methods provided by the object store to open a cursor on the database named “USERS,” enumerate through the records, filter out records for inactive users, and use accessor methods to get the values of each field in the remaining records.

[Back to Home](README.md)