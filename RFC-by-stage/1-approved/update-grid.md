---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Update Grid 12 to use Flexbox

## The issue to be solved

Grid 12 is how the Design System does layout.

Grid 12 was based on Bootstrap 3 (I think, it might be v4) and uses the box model to handle layout. Bootstrap v3 Grid docs here https://getbootstrap.com/docs/3.3/css/#grid and v4 here https://getbootstrap.com/docs/4.0/layout/overview/.

However, Bootstrap is now at v5.1 and has moved to Flexbox, see https://getbootstrap.com/docs/5.1/layout/grid/, which is a good signal that we should too.

There are increased benefits of using Flexbox - such as easier vertical centering, which would add capability to Grid 12.

A downside is that this would limit browser compatibility, however, Flexbox is highly supported by browsers nowadays, see https://caniuse.com/flexbox.

## A short description of the desired outcome or solution

I propose we keep a similar API design, but replace the internals of Grid 12 to use Flexbox.   


## Technical details

* Rewrite Grid 12 module
