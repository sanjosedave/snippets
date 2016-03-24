# snippets

engagement-autoplay.js

Meant to add an autoplay toggle to the player, this should be been forked from:
https://github.com/theonion/videojs-autoplay-toggle

Logic:
Increment the view counter in localStorage each time a "play" event is received from the player.

On each player load & play, check to see if the autoplay button has been toggled on by the user OR the view counter in localStorage is gt; 10.  If gt; 10, toggle the autoplay button, and store that in the original key value in localStorage.
