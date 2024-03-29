---
{"dg-publish":true,"permalink":"/notes/open-source-projects-i-m-proud-of/"}
---

# Open Source projects I'm proud of

---

- [[notes/Open Source projects I'm proud of#RetroAchievements - project/community management\|RetroAchievements - project/community management]]
- [[notes/Open Source projects I'm proud of#RADocs - docs & docs website pipeline\|RADocs - docs & docs website pipeline]]
- [[notes/Open Source projects I'm proud of#RANews - webdesign/webdevelopment\|RANews - webdesign/webdevelopment]]
- [[notes/Open Source projects I'm proud of#RABot - Discord Bot\|RABot - Discord Bot]]

---


## RetroAchievements - project/community management

**NOTE**: I'm **not** the creator of this project.

- website: <https://retroachievements.org>

What I did:

- contributed with the implementation of the RetroAchievements feature in the RetroArch (building/testing implementation in various architectures).
- contributed with code for the [backend](https://github.com/RetroAchievements/RAWeb).
- server maintenance (Linux/NginX).
- created the [documentation project](https://docs.retroachievements.org/).
- community management


## RADocs - docs & docs website pipeline

- website: <https://docs.retroachievements.org>

Documentation for the RetroAchievements project.

I created this project using the following technologies:

- [GitHub wiki](https://github.com/RetroAchievements/docs/wiki/), as the place where contributors can create/update contents for the website.
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) for converting the markdown files from the wiki into the website's pages.
- [Some scripts](https://github.com/RetroAchievements/docs) I created to glue things together.
- [GitHub Actions](https://github.com/RetroAchievements/docs/blob/master/.github/workflows/deploy-radocs.yml), to easily deploy the website.


## RANews - webdesign/webdevelopment

- website: <https://news.retroachievements.org>

A monthly web-zine, bringing news about the RetroAchievements scene.

I designed the website from scratch (that was my first website built from scratch).

Technologies used

- HTML/CSS only (I opted to not use JavaScript).
- [Jekyll](https://jekyllrb.com/), as the Static Site Generator.


## RABot - Discord Bot

A Discord bot for the RetroAchievements community.

- Accessible in the [RA Discord Server](https://discord.gg/dq2E4hE).
- Code available [here](https://github.com/RetroAchievements/RABot).

Technologies used:

- JavaScript/NodeJS
- [DiscordJS](https://discord.js.org/#/)
- A bunch 3rd party APIs.
