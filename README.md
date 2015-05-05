# Grooveshark Backup List
A simple HTML for view the backup of the collection of songs from Grooveshark.

This is a simple web page with a table artist-ordered of the collection songs from Grooveshark, need before run the script of https://gist.github.com/simonc/ec00955845e23046f6d8 :

```javascript
var libraryKey = Object.keys(localStorage).filter(function(key) {
  return key.match(/library\d/)
});
var lib = localStorage[libraryKey];
lib;
```

The steps are:
1. Go to http://grooveshark.com

2. Open your browser devtools, go to the Console tab and type the content of the JS script above.

3. You'll get a big JSON blob copy it (without the begin and end quotes).

4. Paste the result in the backup.js file.

5. Open the index.html in a browser.
