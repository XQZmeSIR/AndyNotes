# Applications don’t reliably maintain scroll positions

Interfaces with long scrollable regions (e.g. long texts, message histories) feel disorienting and fragile in part because application developers don’t regard scroll positions as an important piece of application state.

If a user stars a message, or chooses a filter, that’s likely to be persisted; loss of that choice is likely to be regarded as data loss. By contrast, common actions in interfaces routinely lose scroll positions.

One challenge here is that while scrolling behaviors are usually implemented via a common system-level component, the _semantic_ interpretation of scroll position as application state is interface-specific. For example, the same viewport might be reused to display several different threads of conversation. In some cases, it makes sense to persist and restore the most recently viewed conversation’s scroll position; in other cases, it makes sense to persist scroll positions independently for each conversation. So persisting this state can’t take place at the layer which would ordinarily be its model.

Related:

  * [[Continuous-scroll digital reading uncomfortably disrupts object permanence]]
  * [[Digital file systems don’t represent order]]

* * *

Q. Why don’t applications reliably maintain scroll positions of interface viewports? A. Developers don’t think of scroll positions as important parts of the interface’s state.

Q. What are some challenges to persisting scroll positions as pieces of application state? A. (e.g. normally the UI framework wants to be the “model”, semantic interpretation of viewport identity varies subtly, etc)

* * *

## References

[[Omar Rizwan on Twitter: “i fear and resent scrolling (e.g. scrolling way up to see chat history) b/c i know application developers don’t take it seriously as app statelike I’ll click on another chat, then back to the chat where I’d scrolled way up, and the app’ll have thrown away my scroll position”]]
