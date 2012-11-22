PHYLO
=====
Phylo is a gaming framework developed by McGill CSB.  Its use for harnessing the computing power of man kind to solve a common problem in DNA; Multiple Sequence Alignment.

Getting Started
=====
Master Branch contains the most recent experimental release

feature/integration Branch is used for integration testing 

Production Branch contains the most recent stable release

We are using Model - View - Controller + Observer Design Pattern

All versions contains an offline mode with dummy data for development 

If you are using chrome for development, you will need to execute this in your terminal : 

	open /Applications/Google\ Chrome.app --args --allow-file-access-from-files --allow-access-control-allow-origin

This will tackle the cross domain issue when working locally. 

This build includes options, it can be found at controller/options_template.js

	window.DEBUG //enables debug log
	window.guest //tell us its anoymous
	window.DEV.disableMenu //disables Menu
	window.DEV.disableSplash //disables Splash 
	window.DEV.disableMusic //disables the background music
	window.DEV.enableTabletMode //forces browsers to load tablet mode.

To enable options w/ .gitignore, make sure the .gitignore is under the directory of options_template.js and it contains the value of - options.js, now in terminal

	cd controller
	cp options_template.js options.js
	
Now you can edit options.js to modify the development options

Note: Do not delete options_template.js

if options.js is tracked, ie - meaning git is tracking the changes, in terminal

	git rm --cache options.js
	git commit -a -m 'untrack options.js'

<b>Please refer to js/README.md for further explanation / crash course<b>

Hot deploy branches
=====
[Under Master Branch]
PHYLO - DNA 
http://phylo.cs.mcgill.ca/master/index.html#!play

[Under feature/RNA Branch]
PHYLO - RNA in pre-Alpha
http://phylo.cs.mcgill.ca/feature/RNA/index.html#!rna

- If want your own hot deploy branch can message me @alfredkam

Devices Supported
=====
Current version supports all major browsers (except IE 6-8) and tablet browsers with screen size bigger than 1024px * 768px.  Tablets have their own custome UX

I want to contribute!
=====
That is awesome! Just fork the project on github.  Create a topic branch, write some code and let us know!


