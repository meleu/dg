---
{"dg-publish":true,"permalink":"/notes/jq/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# jq

## minify JSON with jq

```
# --compact-output | -c
$ date -c input.json
```

## if with no else

Else is mandatory, but you can use `empty` to make it do nothing.

```
jq 'if CONDITION then SOMETHING else empty end' input.json
```

