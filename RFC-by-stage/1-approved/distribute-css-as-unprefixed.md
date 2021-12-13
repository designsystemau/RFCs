---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Distribute CSS unminified and unprefixed

## The issue to be solved

CSS is currently being distributed as minified and vendor-prefixed assets.

This is unnecessary since users (developing apps using npm) process styles for minification and vendor-prefixing, therefore css "as modules" should ship without being processed. This issue was raised by @liamfiddler [here](https://github.com/designsystemau/RFCs/pull/11#discussion_r724769922).

Where users want to consume full CSS however, they may still expect the asset to be vendor prefixed and minified. This scenario might be handled better by delivering styles from a CDN like [UNPKG](https://unpkg.com/).

This work should ship with pancake being removed [#1](https://github.com/designsystemau/RFCs/pull/1).

## A short description of the desired outcome or solution

- Npm packages should contain unprocessed CSS assets
- New package "design-system" is created which provides minified + vendor-prefixed CSS **and** an unprocessed version, ie `gold.min.css` and `gold.css`
- Usage of the new package is documented

## Technical details

Assuming that pancake has been removed.

1. Create a new package "design-system", (gold-design-system/packages/design-system) to generate a full CSS
2. In the design-system package, minified + vendor-prefixed assets **and** an unprocessed version CSS are published
3. Remove minifier and vendor prefix from other packages
