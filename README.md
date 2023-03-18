Jeopardy (using HTML and jQuery)
====

This is a HTML and jQuery based Jeopardy implementation. The mouse is only needed for selecting a tile, everything else is controlled using keyboard commands:

* `1`...`9` select player (buzz)
* `0` reset player (undo buzzing)
* `+` right question was given, add points for current player
* `-` wrong question was given, substract points from current player
* `a` show question
* `n` nobody answered
* `x` hide clue (after accidently clicking it)
* `m` play think music (requires include/think-music.mp3, not included in this repo)
* `s` stop music
* `d` demo mode ("tile runner")
* `F1`...`F12` or `l` lock input

`jeopardy.html` reads the board from JSON files (`board.json` by default, but you can use `jeopardy.html?myboard.json` to use a different file). If you include images, I'd recommend not to specify image dimensions and use CSS max-width/max-height instead.

It's possible to add one or more "daily doubles", see Category1 for 500 in board.json for an example. (Note that the player who picks a daily double needs to buzz nevertheless.)

`print-jeopardy.html` can generate a printable cheat sheet from the JSON files for the game host.

Note that this implementation expects the game host to provide sane input. It has some safety nets for obvious errors, but not for everything.



License and Credits
----
This jeopardy implementation is licensed under the MIT license.


It is based on Ryan McDevitt's [JavaScript Jeopardy](http://mc706.com/tip_trick_snippets/43/javascript-jeopardy/) and uses [jQuery](http://jquery.com/).

