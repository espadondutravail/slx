#Silex, live web creation.

##About Silex

Silex, is a free and open source website buidler in the cloud. Create websites directly in the browser without writing code. And it is suitable for professional designers to produce great websites without constraints. Silex is also known as the HTML5 editor.

Brought to you by Silex Labs team, promoting free software.

Current version: v2.0.0alpha3

* http://www.silex.io/

More info on Silex Labs website

* http://www.silexlabs.org/silex/

Questions and answers

* http://graphicdesign.stackexchange.com/questions/tagged/silex

Discussions

* Facebook http://www.facebook.com/silexlabs
* Twitter https://twitter.com/silexlabs
* Google plus https://plus.google.com/communities/107373636457908189681

News and tutorials

* blog http://www.silexlabs.org/category/the-blog/blog-silex/
* subscribe by email http://eepurl.com/F48q5

GPL license

* http://www.silexlabs.org/silex/silex-licensing/

##Installation on your local computer (developers only)

Developers you can clone this repository and start the serveur (unifile), the back end of Silex, with nodejs. See instructions bellow.

Clone this repository, and do not forget the sub modules (cloud-explorer and unifile)

Then install node.js http://nodejs.org/

Start the server with "node cloud-explorer/unifile/lib/app.js"

And open http://localhost:5000/ in a browser

##Distribution/packages

You can use Silex online on www.silex.io or locally or on your server.

This is how Silex is distributed:

* Hosted free
  No install, just go to http://www.silex.io/ and do design
  Edit HTML pages in your drobbox, gdrive...  Your site is visible only by people with whom you share it.
  Tech note: host cloud explorer @silexlabs (silex.html on SL dedicated server and nodejs on heroku)
* Hosted pro
  Comming soon
  Purchase a hosting plan, go to http://www.silex.pro/ and do design
  You edit your site from an online location. Your site accessible to everyone 24/7.
  Paid, no setup, no need to know anything about hosting.
  Tech note: PHP file explorer hosted @arvixe, silex.html on SL dedicated server (use arvixe.silex.io ??)
* Hosted anywhere
  Purchase a stadard shared hosting, and use Scriptaculous automatic install to install Silex in a folder.
  You can manage multiple separated sites with different instances of Silex to edit the site.
  Tech note: silex.html and PHP file explorer hosted by the user's hosting company
* Hosted by you, front and back
  Download Silex and host it with its nodejs server.
  Offer Silex "Hosted free" version to your users, on your domain name.
  Your users go to your URL and use Silex from there to edit their files from their cloud services.
  Tech note: node server, silex in the unifile server

##dependencies

* unifile https://github.com/silexlabs/unifile
  wich uses nodejs and the modules: express, dbox, express, googleapis, logger, node-oauth, oauth, path
* cloud explorer https://github.com/silexlabs/cloud-explorer
  which uses angular.js
* ace http://ace.c9.io/
* google closure library and compiler
* jquery and jquery UI
* handlebars.js

##Development

To install Silex, client and server on your local computer, follow the instructions bellow.

###install node and npm
https://gist.github.com/isaacs/579814

###install foreman
http://blog.daviddollar.org/2011/05/06/introducing-foreman.html

###get silex and start the server
cd /home/
git clone git@bitbucket.org:lexoyo/silex.git
cd silex/server/
./start-server.sh

##Road map

###v2.0.0alpha4

WYSIWYG

* shortcuts (suppr, arrows, save, new, open)
* set as default page (drag drop pages and change order)
* analytics to analyse the use of the editor

Properties

* UI sounds?
* shadows
* font-*
* cursor
* scroll?

Texte

* difference entre typo dans l’editeur text et sur la scene
* detecter la couleur de fond (chercher le background color ou image dans les parents)

Components

* media (image, audio, video)
* nav bar

File

* group images on the same drive as the html page?
* export (cleanup html, make zip with .html, .js, .css, all media)? + host on github or other free hosts?

###v2.0.0alpha5

Edition

* copy/cut/paste
* undo/redo
* autosave
* multiple selection
* better text editor?
  http://www.webdesignerdepot.com/2008/12/20-excellent-free-rich-text-editors/
  http://mindmup.github.io/bootstrap-wysiwyg/

File properties

* background
* title and description and keywords
* favicon

Contextual menu on the elements (menu bar under the menu like google?)

* delete
* lock/unlock
* up/down (z-index)
* rotation

###v2.0.0beta1

Continuous integration

* jshint, PhantomJS, jenkins, Selenium
* unit tests
* functional tests

Profesionnal installation

* bower?

Unifile archi

* Should be a nodejs module
* Silex ande CE would use it as a middleware
* No more strange system for config in unifle?

Debuging

Validation

* http://validator.w3.org/

Nice to have :

* file://localhost/Users/lexa/Dropbox/fdt-workspace/Silex/libs/closure/goog/demos/onlinehandler.html
* file://localhost/Users/lexa/Dropbox/fdt-workspace/Silex/libs/closure/goog/demos/fpsdisplay.html

###v2.0.x

Packaging / distribution

* App.js ?
* chrome app http://developer.chrome.com/apps/about_apps.html
* arvixe like service
* add "multiple ftp" to file browser
* newsletter editor or postcard editor
* mainstream CMS page, article or theme editor
* mockup tool
* banner editor


###other features and ideas for plugins

* edit local website

  * http://devcenter.kinvey.com/nodejs/guides/users
  * http://stackoverflow.com/questions/11534412/any-good-user-management-framework-for-node-js
  * http://usercake.com/docs.php#3
  * http://labs.bittorrent.com/experiments/sync/technology.htm

* edit ftp

  * http://www.goodsync.com/how-to-sync/ftp
  * https://github.com/FTPbox

* analytics

  * google, yahoo, piwik
  * track links http://www.seosite.co.uk/outgoing-links-on-google-analytics


* mobile optimized version of Silex editor

* sites dynamiques ou administrables
Google mbaas
Ou un cms backend only

