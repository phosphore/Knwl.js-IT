Knwl.js it-IT 
=======
Trova date, ore, emails, numeri telefonici, links, tempi di lettura, persino emozioni nel testo, o controlla se è spam. Knwl.js rende possibile scansionare grandi quantità di testo cercando dati che potrebbero essere interessanti.

####Cenny.js Plugin
For those interested in version of Knwl.js that has basic Cenny.js functionality (early development), look here: https://github.com/loadfive/cenny.js/tree/master/plugins

###Demo: http://byteaspect.com/knwlDemo

##How to use

Add **Knwl.js** to the ```<head>```

Create a new instance of the Knwl object:
```javascript
var x = new Knwl();
```

Initiate crawling of a string:
```javascript
x.init( string );
```

Get data:
```javascript
x.get('dates'); //returns array of dates found: [month,day,year, string snippet]
```

**Types of data that can grabbed:**

```"dates"``` - dates found in string.

```"times"``` - times found in string.

```"links"``` - links found in string.

```"emails"``` - emails found in string.

```"phones"``` - phone numbers found in string.

```"places"``` - places found in string.

```"readingTime"``` - estimated reading time of string.

```"emotion"``` - estimated emotion, works best with shorter strings (comments, etc).

```"spam"``` - checks if text is possibly spam. Returns true or false.


*Please note that Knwl.js is still in early development, and can yield varying results.*

**If you want a real-time, plug 'n play backend to store all the data you find, you might like Cenny.js: http://github.com/loadfive/cenny.js**


###Building

For Node, if uglify-js is installed globally ( `npm install uglify-js -g` ) then 

    uglifyjs -o ./knwl.min.js ./knwl.js

will create *knwl.min.js*. 


###Licence

Project released under an MIT license.

