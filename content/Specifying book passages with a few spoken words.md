# Specifying book passages with a few spoken words

[[Voice-based interface]] offers one avenue for [[Methods for bringing dynamic mediums to physical reading contexts]]. Many dynamic interactions involving a text will require you to indicate a passage of interest in the text, or to know what you’re looking at. For instance, maybe you’d like to make a note about a passage, or highlight it, or add a memory system prompt about it. How to do that with voice?

Well: probably any point in a book can be uniquely identified with 3-5 words. Likewise, a range can likely be uniquely identified by speaking 3 starting words and 3 ending words, particularly if we can assume that ranges are unlikely to extend more than two pages.

This suggests a voice-based interface which might have functions like:

  * “at ‘John was born in’ highlight”
    * here, only a prefix is given; perhaps the sentence is highlighted
  * “at range ‘John was born in … with his father.’ highlight”
    * Here, a range is given. It’s probably not necessary to explicitly specify the delimiter between the start and end segments—can just try all break points.
  * “at ‘John was born in’ bookmark”
    * “last three bookmarks”
  * “at ’John was born in’ start note… ‘Follow up on this’ end note”
  * “at ‘For more on elaborative encoding see’ open link”
  * “at ‘John was born in’ start prompt When was John born? start response 1942 end response”
  * “at ‘For more on this, see” add todo”
  * “append to last note”
  * “redo last note”
  * “discard last note”
  * etc…

A key design element of this interaction is the feedback: the system needs to let you know that it’s found the spot you’re looking at, and you need to not feel the need to second-guess it. [[Rob Ochshorn]] suggests that with Gentle, the system could perhaps start reading along with you in realtime once it thinks it’s found the spot. That’d be pretty incredible. More straightforwardly, it could speak a page number or the next few words.

You’d want to use a high-specificity model for the control words, a super- biased model for the quote passages, and a general transcription model for the open-ended note input. I think it’s pretty important to treat these things separately. General-purpose transcription models are too slow and too inaccurate for the control words—you don’t want to be second-guessing that limited set. Ideally the control part can feel totally realtime. The general transcription part can be slower, and less accurate. That’s fine, especially if you still have the original audio.

Results and actions from this interaction might display on a companion device, like a phone sitting in the cupholder of the folding chair I often carry to the park. This would give you a bit of external buffer to augment your working memory: I often can’t keep track of more than a couple notes I’ve made.

One thing that’s nice about this model is that it doesn’t require an exact PDF scan of the text on your computer—e.g. as specifying page numbers would. (Though obviously it’s nice to be able to refer to page numbers in the interface) Many contemporary texts are only available digitally as EPUBs. No one’s bothered to scan them yet. We could require that users scan them, of course, but that’s quite a burden.

## References

This idea initially arose in conversation with [[Derrek Chow]] on [[2022-11-29]]; fleshed out a bit more with [[Rob Ochshorn]] later that day.

This interaction owes much to the [[Canon Cat]]’s "Leap" interaction, and its descendants in modern text editors and [[Shortcat]].
