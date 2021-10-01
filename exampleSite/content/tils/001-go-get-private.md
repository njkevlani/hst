+++
title = "Go Get Private"
date = 2021-09-21T22:37:54+05:30
tags = ["go"]
tiltags = ["go"]
+++
There is no proper way to do this.

These are the options:

- `git clone` repositories in GOPATH at proper location and the do `go get`. Not a sane option as one might have to clone all the private dependancies.
- Configure `git` to always use ssh. This also isn't a perfect solution. Due to this, you will always need to use ssh for cloning repositories even if they are not private.

```bash
$ git config --global url.git@github.com:.insteadOf https://github.com/
```
