# Figma’s widget API creates an extensible, composable, sharable infinite canvas environment

[[Figma is a surprisingly general-purpose infinite canvas]], but the recent addition of a widget API adds an interesting range of extensibility to its palette.

Widgets are custom interface elements which can be placed onto the Figma 2D canvas. Like any other canvas object, they’re shared seamlessly between all users, including any internal state they might define. Their presentation is defined in terms of typical Figma nodes. You can implement simple interactive interfaces via click handlers and text input. As a simple example, you could make a poll widget which any user can vote (once) on.

Perhaps the most interesting property of widgets is that they can be “stickable”. That is, when you place them on another node, they move along that node on the canvas. For example, you could implement a voting interaction using a “gold star” stickable widget. Users could place gold stars on their favorite artboards, then a separate widget could display a realtime leaderboard.

A few properties which seem core to widgets-as-medium:

  * they’re spatial, tactile, positional
  * they’re composable with other elements (through stickability or through proximity)
  * they’re shared, multiplayer
  * they’re interactive (not just placeable—can include buttons, text fields)
  * interaction lives on-canvas (popping out a modal iframe is an anti-pattern)

## Notes from API documentation

Figma offers APIs for both “plugins” and “widgets”. They’re related but distinct. Plugins are installed and controlled by an individual user. Conceptually, they’re attached to the application. If they present an interface, it’ll be in a floating window, rather than on the canvas.

By contrast, widgets are attached to a canvas and are therefore shared between all users of that document. They may have persistent state, which will be synchronized like other canvas object data. (As of [[2022-10-17]], widgets cannot have any transient local state—all state is synced)

Widgets may execute code in response to interactive elements (clicks, text editing) on its surface, via a “property menu” which all widgets may offer, via stickable callbacks (more later), or via messages from iframes.

Widgets may be _stickable_ : that is, widgets may define special behaviors which occur when they’re attached to particular elements. Widgets may may also define what happens when other widgets are attached to them (as a “stickable host”). Note, however: ==widgets cannot be both a stickable and a stickable host==. And, alas, ==widgets can only be stickable in FigJam, not in the Figma editor.==

Authors of widgets may end up using the plugin API, for instance to modify elements on the canvas, or to open a modal interface.

Widget code runs in two distinct execution environments: rendering, and state updating. When in the rendering environment, execution must depend only on the widget’s state (i.e. not on other document state), and widget state cannot be modified. By contrast, state updating is executed asynchronously and has read/write access to the document and widget state. (In particular, the plugin API can only be used in event handlers and hooks)

While a widget’s interface is defined in code via JSX, Figma offers a “Widget Code Generator” plugin which translates an on-canvas design into JSX.

I’d hoped that I could maybe use a widget with a text input to make keyboard input work in a Figma prototype, but as of [[2022-10-18]] widget interactions are disabled when presenting.

[[To make a network request]], you must make an invisible iframe (i.e. to access the browser’s networking APIs).

## References

Conversations with [[Taylor Rogalski]] on [[2022-08-21]] and [[2022-10-17]] were essential to my thinking on this topic.
