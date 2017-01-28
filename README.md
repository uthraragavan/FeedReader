## FeedReader Testing
In this project I was given a web-based application that reads RSS feeds. This project focuses on writing test cases using Jasmine [Jasmine](http://jasmine.github.io/). The test cases are written in jasmine/spec/feedreader.js

### Packages used
Jasmine 2.1.2

### Setup Instructions to host your own web server
* **Node JS for localhost web server**:  Install Node JS by following instructions from here https://nodejs.org/en/download/
* **Ngrok for webserver over proxy**: Install ngrok by following instructions from here: https://ngrok.com/download
* **Gulp as build configuration tool**: From Node JS command prompt, install gulp by following instructions from here: https://www.npmjs.com/package/gulp-download
* **Gulp modules required to run our web app**: From Node JS command prompt, install the following gulp modules:
    * gulp-uglify
    * gulp-util
    * gulp-rename
    * gulp-clean-css
    * gulp-imagemin
    * gulp-image-resize
    * gulp-htmlmin
    * browser-sync
    * ngrok
    * run-sequence
as defined in package.json by typing the following command:
```
npm install
```

### Starting Web App
##### From github server
* The web app is hosted on https://uthraragavan.github.io/FeedReader

##### Hosting your own web server on ngrok

* **Download the project assets from Github**: https://github.com/uthraragavan/FeedReader
* **Starting web app**: From Node JS command prompt, navigate to the project asset folder on your system and type gulp. This will start the web app over ngrok proxy. A browser window showing index.html from dist folder shows up. The gulp command from command prompt should display something like this:
 ```
[17:44:01] Using gulpfile ~\Desktop\Udacity\FrontEnd\Feed Reader Testing\frontend-nanodegree-feedreader-master\gulpfile.js
[17:44:01] Starting 'webhost'...
[17:44:01] Starting 'browser-sync'...
[17:44:01] Finished 'browser-sync' after 40 ms
[17:44:01] Starting 'ngrok-url'...
serving your tunnel from: https://4f854c81.ngrok.io
[17:44:01] Finished 'ngrok-url' after 560 ms
[17:44:01] Finished 'webhost' after 608 ms
[17:44:01] Starting 'default'...
[17:44:01] Finished 'default' after 10 μs
[BS] Access URLs:
 --------------------------------------
       Local: http://localhost:3000
    External: http://192.168.0.103:3000
 --------------------------------------
          UI: http://localhost:3001
 UI External: http://192.168.0.103:3001
 --------------------------------------
[BS] Serving files from: ./dist
```
The results of the test cases appear in the bottom of index.html.