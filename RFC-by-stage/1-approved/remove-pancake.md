---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Remove pancake

## The issue to be solved

Pancake has been built (by me) a while ago and solved a couple very specific problems outlined in [this article](https://medium.com/dailyjs/npm-and-the-front-end-950c79fc22ce).
Since 2018 the front end space has evolved significantly and shipping CSS files via npm isn't an issue anymore.
In-fact shipping CSS files that are automatically imported by the prod bundle located inside a `node_modules/` folder causes significant issues to loaders like webpack which now require the CSS loader to be specified and the specifically allow the `node_modules/` path.

## A short description of the solution

We should remove pancake from the `postinstall` npm hook and deliver the CSS separately in the npm payload.
This means consumers can use the CSS file the way they like including via the `<link>` HTML tag.

## Technical details

1. Remove the `postinstall` hook from each packages `package.json`
2. Remove the code that injects the imports automatically from [the helper](https://github.com/designsystemau/design-system-components/blob/master/scripts/helper.js#L432)
3. Document how to use the components and the CSS together
