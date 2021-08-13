---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Simplify the monorepo

## The issue to be solved

The tool [lerna](https://lerna.js.org/) we have been using to power the monorepo has become incredibly slow and difficult to deal with.
We need to simplify the structure to allow us to fix things faster.

## A short description of the solution

I propose we remove lerna, move to [yarn v1 workspaces](https://classic.yarnpkg.com/en/docs/workspaces/) and de-tangle the reasons the `bootstrap` process is currently so dependent on a very specific order at which what dependency has to be installed.

## Technical details

TODO 😬
