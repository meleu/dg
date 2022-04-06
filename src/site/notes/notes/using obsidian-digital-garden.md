---
{"dg-publish":true,"permalink":"/notes/using-obsidian-digital-garden/"}
---

# using obsidian-digital-garden

This is my oversimplified version of the plugin's instructions [here](https://github.com/oleeskild/obsidian-digital-garden).

## preliminary work

- [x] github account
- [x] netlify account
- [x] go to [this repo](https://github.com/oleeskild/digitalgarden) 
    - [x] click in "Deploy to netlify"
    - [x] give it a meaningful name
    - [x] follow the steps on netlify
- [x] [create an access token](https://github.com/settings/tokens/new?scopes=repo) on github **and copy it in a safe place**

## in obsidian
- [x] install the obsidian-digital-garden community plugin
- [x] in obsidian "Digital Garden" options, fill in
    - [x] github username
    - [x] the name of the repo (you created it right after "Deploy to netlify")
    - [x] the github access token


## creating notes

The notes you want to see published must have `dg-publish: true` on their frontmatter:

```yaml
---
dg-publish: true
---
```


The one you wanna see as your home page must have this on the frontmatter:

```yaml
---
dg-publish: true
dg-home: true
---
```


## publishing "all" notes

Currently there's no way to publish all notes by default (I opened an [issue with requesting this feature](https://github.com/oleeskild/obsidian-digital-garden/issues/26)).

As a workaround I created a script that works nice for my workflow: <https://gist.github.com/meleu/f9667e76a2744d46686702edeb3cc77c>



---

## bug report

**Checking `<ul>`:** ✅

- item1
- item2
- item with a sublist
    - subitem1
    - subitem2
    - subitem3
- itemN


**Checking `<ol>`:** ✅

1. list
1. item1
1. item2
1. item with a sublist
    1. subitem1
    1. subitem2
    1. subitem3
1. itemN


**Checking `<ul>` with a `[ ]` checkbox:** ❌

- [ ] item1
- [ ] item2
- [ ] item with a sublist
    - [ ] subitem1
    - [ ] subitem2
    - [ ] subitem3
- [ ] itemN



