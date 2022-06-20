---
{"dg-publish":true,"permalink":"/questions/linux-how-to-synchronize-two-directories-to-have-the-same-contents/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# linux - how to synchronize two directories to have the same contents?

## Unidirectional
[[notes/rsync|rsync]] is the right tool for mirroring (one directory is the source and the other one is the target).

But a question persists: **How to know when a file was changed?**.


## Bidirectional
Another interesting tool that synchronizes directories in a bidirectional way is [[unison|unison]].

> [!warning]
> When installing **unison** with `apt install` it doesn't come with the file system monitoring tool.
>
> The solution is to download the binaries from the github releases page.

## See also

[[notes/Google Drive on Linux#^f67779|Google Drive on Linux > Synchronizing]]
