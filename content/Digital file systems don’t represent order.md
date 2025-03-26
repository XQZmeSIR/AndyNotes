# Digital file systems don’t represent order

File system GUIs ostensibly mimics files in folders, but it’s funny to note that _reordering_ is a fundamental verb for physical papers in folders (or in piles on my desk). There’s no way to reorder a list of files in Finder without doing something silly like adding numbers to the front. You can switch to grid view and drag icons around, but that’s a “repositioning” verb, not a “reordering” verb, so doing something like “moving a paper to the top of the pile” is surprisingly awkward.

The file system itself makes this kind of affordance hard. Folders are a bag! How would you even store an ordering portably? Lexically ordered keys as special fs attrs, I guess? You’d probably resort to something like .DS_Store.

This rant came from wondering: why do I feel like I want a special piece of software to manage my reading lists, or my sheet music? Why not just folders of PDFs? (Never mind the fact that most specialized “read it later” software doesn’t let you reorder the queue!)
