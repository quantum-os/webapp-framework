WebApp framework for Papyros
===============================

**Warning: this is very much an initial working concept. There is a lot to implement, and the project is not structured at all yet. Stay tuned for further progress!**

To use this in QML:

`import Material.WebApps 0.1` *or*

if just want to create the most basic webapp, you can create a JSON with the following fields:

 - **title** - the name of the WebApp/Site ex. Inbox, Soundcloud, Yahoo, Outlook
 - **url** (self-explanatory)
 - **loadingImage** - a banner, this is shown at startup until the web site loads, should be relative to the current directory ex. `images/banner.png`
 - **color** - the dark color (700 of 500 if the website's main color matches one of the material design ones)

and then just run the `make_webapp.py` script into your project's directory.
Usage: make_webapp.py (build|install|run)

build: Build the web app, looking for a webapp.json file into your directory, the webapp will not be regenerate if it already exists, except if you include a --force option.

install: Install your webapp into the Linux system

run: Run your webapp, using qmlscene
