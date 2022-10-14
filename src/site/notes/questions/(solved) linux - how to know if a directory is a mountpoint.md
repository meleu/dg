---
{"dg-publish":true,"permalink":"/questions/solved-linux-how-to-know-if-a-directory-is-a-mountpoint/","dgHomeLink":true,"dgPassFrontmatter":false,"dgShowBacklinks":true,"dgShowLocalGraph":true}
---


# linux - how to know if a directory is a mountpoint?

Pretty straightforward: use the command `mountpoint`

example:
```console
$ mountpoint gdrive
gdrive is a mountpoint

$ mountpoint src/
src/ is not a mountpoint
```