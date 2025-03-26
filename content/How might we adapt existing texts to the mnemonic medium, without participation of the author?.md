# How might we adapt existing texts to the mnemonic medium, without participation of the author?

[[Mass adoption of the mnemonic medium seems to require mass adoption of web publishing]]. Furthermore: lots of important books aren’t available in any digital form at all; many people prefer hard-copy books and e-ink readers. Technical audiences will continue to use PDFs for ages. What about [[Audiobooks]] and video? It would be very powerful if we could “hoist” existing media into the medium without sacrificing its power.

None of these approaches below are actually good, but perhaps iterations on them could be?

## “Companion reader” app

You have a paper book open in front of you; you put your phone next to it and open the Mnemonic Companion app. You scan the book’s barcode, and it displays a table of contents (perhaps partially-redacted for legal reasons) and page number selector. You tell the app that you’re reading page 312. The screen displays a stack of questions and a big header that says: “answer these at the section break on page 314.” You start reading the physical book, highlighting and sticky noting, and you tackle the questions at the appropriate spot. The app moves along to the next breakpoint, and you continue reading.

This approach is a huge kludge. It requires readers to remember where they’re supposed to stop, monitor for that point, and switch back and forth between the two media. That sounds like a pain. I suspect compliance rates would be much lower than on Quantum Country.

But it’s a very flexible approach which could be adapted to basically any prior media form. It doesn’t require author/publisher cooperation, and the questions could be sourced from a variety of producers (related:[[Audiobooks are produced under a wide variety of business models]]).

Separately, the distribution channel is terrible: someone who’s reading a book has to decide to separately seek out additional material around it, check our app for support, and possibly pay separately for that material. Discussion of a book/PDF on Twitter doesn’t point people towards this companion. There aren’t any meaningful network effects.

## Browser extension page for web books

For books already hosted online (like [[Cell Biology by the Numbers]]), they could be augmented via a browser extension. I don’t love this—it’s a huge ask for users. It’d be neat if we could just wrap the page in an iframe and manipulate it cross-domain, but of course no browser will allow that.

## Content transformation proxy

A “non-transparent” web proxy can re-serve the target web page, with the addition of an extra `<script>` tag. At least for new-user usage patterns, this is a much lighter-weight way of achieving the same results as a browser extension-based solution. You can make a linkable URL!

[[Hypothes.is]] uses one of these to make its sharable links work: via.hypothes.is injects the target URL.

This… actually seems pretty doable!

### Implementation considerations

There’s even a W3C article! <https://www.w3.org/TR/ct-guidelines/> (It’s a “Working Group Note”, not a ratified document).

    
    
If a proxy alters the response then: 1. It must add a Warning 214 Transformation Applied HTTP header field;

See [[warning codes]].

    
    
Proxies **should** indicate their ability to transform content by including a comment in the Via HTTP header field consisting of the URI “http://www.w3.org/ns/ct”.

Note security issues around link rewriting: a rewriting proxy can accidentally make two different sites be same-origin (i.e. that of the proxy). This can introduce vulnerabilities. Also:

    
    
The practice of intercepting HTTPS links is strongly NOT RECOMMENDED.
    
If a proxy rewrites HTTPS links, it must advise the user of the security implications of doing so and must provide the option to bypass it and to communicate with the server directly. ... When forwarding responses from servers proxies must notify the user of invalid server certificates.

Basically all links are HTTPS these days, so this more or less amounts to “don’t rewrite links”! Or at least: be _extremely_ careful.

See also the HTTP 1.1 RFC’s [[comments on intermediary transformations]].

    
    
A proxy that transforms the payload of a 200 (OK) response can further inform downstream recipients that a transformation has been applied by changing the response status code to 203 (Non-Authoritative Information)

See also this preliminary [[Content Transformation Landscape 1.0]]

## Custom PDF / EPUB reader

We could make our own PDF or EPUB reader apps which add these elements inline to those existing media forms. Or maybe it’s a web-based viewer, bookmarklet- style: prepend any PDF URL with “<http://mnemonic.com”> to read it in this form, etc.

Doing this for EPUBs isn’t really viable while DRM remains pervasive. Legally- purchased ebook couldn’t be opened in our reader. So doing this for ebooks would require us becoming an ebook store. Yuck.

This would be a ton of work. Big distribution channel problems here.

Honestly, a better approach to PDFs is probably through one of the myriad “PDF-to-web page” tools. Take the academic PDF; turn it into a web publication; _then_ enhance it (e.g. via [[Turning any web page into the mnemonic medium]]).

## AR glasses

If we’re all wearing AR glasses in the future, we can magically enhance books in all kinds of interesting ways. Too far off to consider seriously? If the rumors about Apple’s 2022 glasses offering are true, AR overlays might become quite mainstream soon…
