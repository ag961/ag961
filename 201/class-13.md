# Local Storage

source:
>Pilgrim, M. *Dive into HTML5: the past. present and future of local storage for web applications.* Retrieved from: http://diveinto.html5doctor.com/storage.html

**HTML5 Storage** (also "Local Storage or "DOM Storage") is a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server.

I JavaScript code HTML5 Storage is accessed through the **localStorage** object on the global **window** object.

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. After retrieving data from storage, it needs to be converted manually back to its original type.


-----

[**<== BACK**](201-toc.md)
