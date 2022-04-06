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
- [ ] [create an access token](https://github.com/settings/tokens/new?scopes=repo) on github **and copy it in a safe place**

## in obsidian
- [ ] install the obsidian-digital-garden community plugin
- [ ] in obsidian "Digital Garden" options, fill in
    - [ ] github username
    - [ ] the name of the repo (you created it right after "Deploy to netlify")
    - [ ] the github access token


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


---

## bug report

**Checking `<ul>`:**

- item1
- item2
- item with a sublist
    - subitem1
    - subitem2
    - subitem3
- itemN


**Checking `<ol>`:**

1. list
1. item1
1. item2
1. item with a sublist
    1. subitem1
    1. subitem2
    1. subitem3
1. itemN



