DUCK HUNT JS v2.0 - MIT License
created by Matthew Surabian
http://mattsurabian.com/duckhunt

This is an implementation of DuckHunt in javascript using HTML5 audio.

This project uses the following JS Libraries:

    -jquery
      -jquery.color
      -jquery.spritely
    -underscore

All of the game logic is in the duckhunt directory.  This project uses grunt to build two concatenated js files;
one representing all of our game logic the other representing necessary javascript library dependencies.

This refactor of the game relies on custom events to control game flow which has cut down a bit on the "animation callback hell"
faced in version 1.

To work with this project on your own simply clone this git repo into a directory, and run "npm install" inside that
directory.  The package.json file included in this repo helps npm install all the necessary node module dependencies.  Make your edits
to the code and run "grunt".  The default grunt task will lint the javascript, concatenate, and minify it into the build
directory.  To generate an even smaller gzipped build run "grunt compress".

TODO:
Implement new weapons (like a shotgun)
Clean up graphics (some sprites have artifacts)
