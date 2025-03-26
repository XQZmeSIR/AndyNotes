# Turning any web page into the mnemonic medium

[[Quantum Country]] is a purpose-built web site; the mechanics are deeply entangled with the essay presentation. But the core interactions of the [[Mnemonic medium]] are separable enough that it should be possible to allow these interactions to be embedded into any web page via simple HTML.

This is a core component of my vision for an [[OS-level spaced repetition system]].

## Web Components

We can define a spec for mnemonic prompts via new HTML tags (e.g. `<card>`). Then we’d provide a (probably open-source) Javascript library which, when added to the page, would “hydrate” those components by replacing them with DOM nodes at runtime. Such [[web components]] are now well-supported in all modern browsers except Edge, and it appears a polyfill exists for that.

This doesn’t necessarily tie the publisher to a specific server for storing user state: our client-side library could offer various server endpoints as they emerge, including client-managed persistent storage (no accounts!).

This approach is flexible: you could swap our client-side library out for another which supported the same web component spec; it can expand to different backend servers in the future; the scope for that JS library could expand to include other features. Publishers could host the JS themselves or serve it from a CDN we control. If JS is disabled or if the script can’t be fetched, the cards would simply be missing. You can even define print stylings for such tags.

This approach does involve a fair amount of abstraction. If we wanted to change the protocol, spec, or state format in some significant way, we’d likely have compatibility issues.

Perhaps more importantly, this approach requires that the author/publisher is meaningfully authoring HTML. This may be challenging to integrate into workflows which e.g. export HTML from InDesign source documents. If the HTML document isn’t the “source of truth,” the card tags will get clobbered whenever the author re-exports from their source document.

We’ll probably still want to make plugins for platforms like Wordpress with this approach.

### Significant barriers to user authentication in third-party contexts

Once a user’s signed in, they should be able to accumulate prompts around the web without having to sign in on every site. This is difficult to achieve!

The hosting site can’t write a cookie that will be readable by any other potential hosting sites: cookies are origin-locked.

We can embed the authentication mechanism in an iframe, hosted on a consistent origin, but these will be “third-party cookies.” In the last couple years, browsers—particularly Safari—have begun to aggressively lock down third-party cookies, since they’re pervasively used for privacy-invading tracking and advertising features.

In general, any mechanism which would allow these embedded prompts to share authentication credentials would also allow us to track that user for privacy- invading purposes. So we’re somewhat permanently in the cross-fire of these browser security features. Chrome and Edge will “just work”, at least for the next couple years, but Safari and Firefox will not. Edge is marked as “implementing” the Storage Access API.

Apple and Mozilla have created a Storage Access API which allows third-party content to request access to its stored credentials in this context. In Safari, it sounds as though this will _always_ require displaying an approval prompt. Yuck. And: Safari may _still_ only allow setting a cookie in this context if the user has already interacted with the site in a first-party context! Wow, brutal. Will likely need to offer a Safari extension to make Safari a reasonable experience.

It appears that Safari is at least adding an API to allow these contexts to determine if the user is logged in. [[Changeset 250944 – WebKit]]

## Parsing and replacing text blocks

Some workflows won’t allow users to add arbitrary HTML tags. For instance, say they’re making a site via some custom blogging software that only offers WYSIWYG.

In these cases, assuming script injection is still possible, we could allow authors to add questions in a similar fashion to [[My implementation of a personal mnemonic medium]], as plaintext, parsed and extracted at runtime by the script.
