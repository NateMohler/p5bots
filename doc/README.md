# Welcome to p5bots!

* [How Does This Work?](#how-does-this-work)
* [p5.Serial](#p5-serial)
* [p5.Board](#p5-board)
* [Getting Started](#getting-started)
* [Issues](#issues)
* [Contributing](#contributing)


<h2 id="how-does-this-work">How Does This Work?</h2>
p5bots is a library that works to send messages from your browser, where you are running p5.js, to your microcontroller, most likely an Arduino. To do this, it uses the `socket.io` library and `node.js` to send messages between the two devices, in a language each device can understand.

This way, you can click on a sketch to light an LED or use temperature data to drive a sketch — or more.

![diagram of client, server, and microcontroller](img/how-it-works.png)

p5bots comprises two sets of files: the client file, called `p5bots.js`, which is included in the `index.html` along with `p5.js` and your sketch; and the server files, called `p5bots-server`, which can be downloaded from [npm](https://www.npmjs.com/package/p5bots-server).

If all this sounds a little too manual, you can also use p5bots from the [p5.js IDE](https://github.com/processing/p5.js-editor).

<h2 id="p5-serial">p5.Serial</h2>
p5bots has a [serial method](doc/module-Serial.html) that can be used in combination with an Arduino sketch listening for serial, much in the same way the Processing serial library can.

For more details on this module, see [the p5.Serial reference page](doc/module-Serial.html).

If you use serial only, you do not need to install Firmata on your board.

<h2 id="p5-board">p5.Board</h2>
The majority of p5bots functionality lives within p5.Board. Inspired by [Johnny-Five](http://johnny-five.io/), p5.Board provides a number of hardware-specific methods in addition to plain digital, analog, and pwm read/write methods.

Details for these methods, plus examples can be found in the module pages. Example sketches and hardware diagrams are also available in [the examples directory on the p5bots Github](https://github.com/sarahgp/p5bots/tree/master/examples).

<h2 id="getting-started">Getting Started</h2>
Ready to go? Good entry points include:
* [the Hello, World tutorial]()
* [checking out examples on the method pages, say RGB LED]()
* reading about [the client API](https://github.com/sarahgp/p5bots) and [p5bots-server](https://github.com/sarahgp/p5bots/tree/master/src/p5bots-server) on Github
* or, [heading over to p5.js to learn more about the drawing library](http://p5js.org/)

<h2 id="issues">Issues</h2>
[Report issues on Github.](https://github.com/sarahgp/p5bots/issues)

<h2 id="contributing">Contributing</h2>
Want to fix an issue you've identified? Looking to create some functionality we have yet to add? Check out the [p5bots repo on Github](https://github.com/sarahgp/p5bots) and, particularly, [CONTRIBUTING.md](https://github.com/sarahgp/p5bots/blob/master/CONTRIBUTING.md).