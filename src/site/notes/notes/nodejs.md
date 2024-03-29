---
{"dg-publish":true,"permalink":"/notes/nodejs/"}
---

# Node JS

## Node Version Manager

It's preferable to use `nvm` instead of installing nodejs from the distro's package manager: <https://github.com/nvm-sh/nvm>

Once it's installed, just run: `nvm install --lts`


## `ERR_FEATURE_UNAVAILABLE_ON_PLATFORM`

I got this error while using node v14 on Linux:
```
TypeError [ERR_FEATURE_UNAVAILABLE_ON_PLATFORM]: The feature watch recursively is unavailable on the current platform, which is being used to run Node.js
```

And it's apparently related to this stackoverflow question: <https://stackoverflow.com/questions/61806341/how-to-fix-the-feature-watch-recursively-is-unavailable-on-the-current-platform>

The problem seems to be related to a breaking change added to NodeJS v14, and one of the solutions proposed is giving the `--poll` argument to `ts-node-dev`.

I decided to just install and use Node v12:
```
nvm install v12.20.0
```


## nice packages/libraries

- express
- multer
- typeorm
- sqlite3
- yup - validation
- monk - talk to the mongodb
- helmet - basic security
- morgan - HTTP request logger
- cors - CORS
- nanoid - URL-friendly unique string ID generator

