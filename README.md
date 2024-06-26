# Eigenwhat?

This repository contains the source for [*Eigenwhat?*](https://eigenwhat.tigyog.app),
an interactive course on TigYog.app.

To use this as a starting point for your own course, you can:

1. Fork this repository.
1. On your GitHub repository, [add a `TY_SESSION` secret for your TigYog account](https://github.com/tigyog/tigyog-cli#publishing-from-git).
1. Remove the `id`s from the files in this course,
   then run `tigyog fmt` to generate your own `id`s.

## Writing locally

Initial setup:

```bash
git clone git@github.com:tigyog/eigenwhat.git
cd eigenwhat
npm i
npx tigyog login sessiontoken
```

Editing and publishing:

```bash
# Edit files in src/
npm run fmt
# Commit any changes
npm run publish
```
