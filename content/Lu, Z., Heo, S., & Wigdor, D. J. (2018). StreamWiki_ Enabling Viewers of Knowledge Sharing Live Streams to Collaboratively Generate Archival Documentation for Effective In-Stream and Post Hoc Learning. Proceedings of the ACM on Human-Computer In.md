# Lu, Z., Heo, S., & Wigdor, D. J. (2018). StreamWiki: Enabling Viewers of Knowledge Sharing Live Streams to Collaboratively Generate Archival Documentation for Effective In-Stream and Post Hoc Learning. Proceedings of the ACM on Human-Computer Interaction, 2(CSCW), 112:1-112:26

The authors design a CSCW system for crowd summarization, tagging, and collaborative filtering in instructional livestreams.

Some interesting affordances:

  * the streamer or the moderator can ask the crowd to summarize a topic that was just discussed
    * social voting highlights the best summaries
    * other readers can suggest improvements to summaries, vote on suggested improvements
  * social voting on comments controls whether they’re archived and how they appear in the archive
    * conversations can continue in the archive via replies
  * highly-upvoted comments will be pinned to the top of the comments area or even scroll across the video (Danmaku)

Danmaku are archived on summary cards intersecting that timestamp

  * timeline-based histogram of comments

  * TF/IDF-significant tags extracted from comments / summaries and mapped visually on timeline; hover interactions link tags to comments and moments on timeline

![](F61EE949-FF67-4A3F-B09C-FFB466032483.png) ![](9E8E6126-0A2D-4435-86F9-A869EFFD85B4.png)

In practice, the researchers struggled with cold start, had trouble getting viewers to participate as they’d hoped.

Q. Term for comments / annotation text scrolling across videos, particularly on Asian video platforms? A. Danmaku
