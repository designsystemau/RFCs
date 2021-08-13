---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Build a simpler docs site

## The issue to be solved

The current docs site, while static and well designed, is outdated and not driven with the same pace as the components.
Co-location of docs and components will also solve the issue of features that are being developed having to include docs (changes) in the same piece of work making the definition of done more transparent.
Another issue is that the current tool is too niche and it's hard to use. We should use something as simple as possible to be able to focus on the content.
We need to retain the static nature of the docs site so we can continue to rely on free static hosting like GitHub pages or Netlify etc.
the information of the pages are also outdated not that the components have moved into the Design System Au group.

## A short description of the solution

We should co-locate the docs site into the same repo as the components and drive the documentation of each component from a docs file that sites in the same folder as the component itself. Preferably a README.md file that can be digested by the docs site.
We should strip other irrelevant pages from the site as well and perhaps add pages describing this groups efforts.

## Technical details

Prior art here: https://github.com/dominikwilkowski/ds-workshop

MORE DETAILS COMING 😬
