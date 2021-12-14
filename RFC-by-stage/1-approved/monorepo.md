---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Simplify the monorepo

## The issue to be solved

The tool [lerna](https://lerna.js.org/) we have been using to power the monorepo has become incredibly slow and difficult to deal with.
We need to simplify the structure to allow us to fix things faster.

## A short description of the solution

I propose we remove lerna, move to [npm workspaces](https://docs.npmjs.com/cli/v8/using-npm/workspaces)
and de-tangle the reasons the `bootstrap` process is currently so dependent on a very specific order
at which what dependency has to be installed.

## Technical details

This RFC depends on [Remove pancake #1](https://github.com/designsystemau/RFCs/pull/1).

Once we have done away with the build of pancake we can de-tangle the install process and since there won't
be any more `postinstall` scripts per component we will be able to install the dependencies per component
without having to worry about the order of what is installed when.

We will still have the test sites we have now running as those do not require any changes and don't depend on anything.
That means we can leave the testing infrastructure in place which is good.

It does however also include the inclusion of the below tools:

- [prettier](https://prettier.io/)
- [manypkgs](https://github.com/Thinkmill/manypkg)
- [preconstruct](https://preconstruct.tools/)
- The docs website

The docs website will be included into this monorepo so that docs are drawn from the readme of each component.
That way we won't have to deal duplicating docs in two places.

This depends on [Docs site improvements #4](https://github.com/designsystemau/RFCs/pull/4).
