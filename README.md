# Game of Life

Yet another Game of Life remake. This one is in Javascript and has a few more features than most, but definitely isn't as good as what you can find on http://www.conwaylife.com/

It isn't very efficient right now, so I wouldn't suggest using large cell counts. This implementation is better at editing than it is running large games. Another thing about this is that 
it is a bounded implementation. Anything out of bounds of the grid counts as being an alive cell this has some interesting consequences.

[Try it out online!](https://adambertrandberger.github.io/gol/play/index.html)

## Usage
To use this on your own HTML pages you can import the script (found in the `dist` folder) using a `script` tag. Then call:

```
gol(document.getElementById('game'));
```

You'll have to create some parent HTML element for the game to be put into. In this case I expected there to be some HTML element named "game". It could be as simple has having: `<div id="game"></div>` somewhere.

## Hot-keys
`p` or `d`: Enter drawing mode (for filling in cells)

`e`: Enter eraser mode (for unfilling cells)

`q`: Enter panning mode (for moving the camera around)

`s`: Save the current screen to the browser's localStorage

`l`: Load the last saved screen from the browser's localStorage

`f`: Load the currently selected prefab

`c`: Clear all cells on the screen

`n`: Run the next generation

`r`: Toggle the loop (loop's speed can be configured with the sliding bar input)

`g`: Toggle showing/hiding the grid


