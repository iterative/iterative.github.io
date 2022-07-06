---
layout: default
permalink: /
redirect_to: https://iterative.ai
---
# Iterative GitHub Pages

This repository tells GitHub to set the default pages root of all org repos to https://docs.iterative.ai/.

For example, enabling GH pages in `https://github.com/iterative/SOME_REPO/settings/pages` will render the site at `https://docs.iterative.ai/SOME_REPO/` (and also redirect from `https://iterative.github.io/SOME_REPO`) unless overridden. To override with a custom domain:

1. run these commands:

```bash
cd SOME_REPO
git checkout GH_PAGES_BRANCH
echo PREFIX.DOMAIN.COM > CNAME
git add CNAME
git commit
git push
```

2. add a `CNAME` record to `DOMAIN.COM` DNS. Name: `PREFIX`, value: `iterative.github.io`.
