## URSSI Conceptualization plan

<!-- badges: start -->
[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
[![GitHub Actions Workflow for commits to master](https://github.com/si2-urssi/plan/workflows/bookdown/badge.svg)](https://github.com/si2-urssi/plan/actions?query=workflow%3ARender-Book-from-master)
<!-- badges: end -->


## Instructions for editing the git book
To update chapters, edit the text for any of the `Rmd` files in the repository. The syntax is standard markdown. References are in Pandoc format (e.g. `[@ref-key]`). Copy your references to any new bib file (to avoid conflicts) and use this `yml` at the top of your chapter

```
---
bibliography: ["references.bib"]
biblio-style: "apalike"
link-citations: true
---
```

Replace `references.bib` with the name of your bib file.

### Building the book

GitHub actions will build the book. It takes ~4-10 minutes to build and you can see progress by clicking on the [Actions tab](https://github.com/si2-urssi/plan/actions?query=workflow%3Abookdown) and navigating to the current build.

## Branches

Only commit to master. Never commit to `gh-pages`. The actions will automatically push to that orphan branch.