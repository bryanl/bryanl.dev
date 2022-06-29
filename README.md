# go.bryanl.dev

## Adding a new repository

To create an entry, create a new page. If I want to expose `go.bryanl.dev/dest` and that
lives at `https://github.com/bryanl/go-dest`:

### Create page

`hugo new code/dest.md`

### Update page's frontmatter

```yaml
---
title: "Log"
date: 2022-06-29T08:27:41-04:00
draft: false
vanity: https://github.com/bryanl/go-dest
aliases: []
---
```

If there are other paths, e.g., `go.bryanl.dev/dest/foo`, add those to the aliases:

```yaml
aliases: ["dest/foo"]
```

### Finish up

Commit changes and push them to GitHub. This repository is automatically deployed when
the `main` branch is updated.
