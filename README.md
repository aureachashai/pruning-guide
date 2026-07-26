# The Pruning Guide — crew page

The published, crew-facing render of Vancouver Island plant pruning data.
One self-contained HTML file: when to prune each plant, the instruction, and the season it belongs to.

**Every instruction here was read and approved by a human before it was published.**

## This repo is generated — do not edit `index.html` by hand

The source lives in the private `plant-care-system` project. To republish:

```
node scripts/build-calendar.mjs --crew     # writes crew/index.html
cp crew/index.html <this repo>/index.html
git commit -am "update" && git push
```

The crew build refuses to run if any pruning task is still unapproved, so an
unreviewed guess cannot reach this page.
