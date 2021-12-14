---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Separate components between React, jQuery and Vanilla

## The issue to be solved

We currently share a lot of code between the vanilla, jQuery and React components.
This has led to a bunch of issues including the fact that we're not using each framework to its fullest potential.

## A short description of the solution

I propose we create separate entry-points for each language and maintain a separation for the JavaScript used in each.
We should still re-use the same CSS though or aim to at least use the same token base (which isn't insufficiently separated yet either).

## Technical details

The implementation would be split in separate entry points.
So inside the monorepo we would have a structure like this:

```sh
.
└── packages
    ├── react
    │   └── ... (a folder per component that is supported in react)
    ├── jquery
    │   └── ... (a folder per component that is supported in jquery)
    └── vanilla
        └── ... (a folder per component that is supported in vanilla)
```

This will make it easier to make changes to each entry-point.

we will work to re-use the tokens wherever we can and since the workspaces are visible to each other this should be simple enough.
