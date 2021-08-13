# GOLD Design System RFCs

> A place where we submit, discuss and host Request for Comments (RFCs)

## What are RFCs?

An RFC (Request for Comments) is a document, in our case a markdown file, that seeks to suggest a change to a software, in our case the [GOLD Design System](https://github.com/designsystemau/design-system-components), by outlining:

- The problem it seeks to fix
- An overview of the proposed change
- Technical description

## How do I submit an RFC?

If you have identified a change you'd like to see in the [GOLD Design System](https://github.com/designsystemau/design-system-components) then please submit an RFC to [this repository](https://github.com/designsystemau/RFCs).
Open a [new PR](https://github.com/designsystemau/RFCs/compare) to this repository and use [the template](RFCs/1-approved/_RFC-template.md) as a starting point and fill it with the information you have.

(💡 The template comes with hints and sections to help you navigate it.)

Make sure you:

- Duplicate the `RFCs/1-approved/_RFC-template.md` file
- Name your new markdown file appropriately
- Fill out all the sections
- Do not change the status at the top of the file
- Do not remove the `_RFC-template.md` file
- Submit your PR

## What are the stages of an RFC?

A new RFC may be merged when it has at least an absolute majority of approvals from [the maintainers](https://github.com/designsystemau/maintainers).

1. The first stage a new RFC will be in is `draft` while it is being discussed in the PR stage.
2. The second stage is called `approved` after it is merged into the `RFCs/1-approved/` folder.
3. The third stage is called `ready-for-implementation` which means the RFC is looking for people to implement it. Come here if you're looking to contribute.
4. The forth stage is called `being-implemented` and this is where all RFCs land that have not been finished but have dedicated people working on it already. The people implementing will be noted at the top of the RFC
5. The fifth stage is called `implemented` and that's where all RFCs land that have been finished and are live.

## How will my RFC be approved?

The group of [maintainers](https://github.com/designsystemau/maintainers) will look at your RFC and discuss it in your PR.
An RFC may be merged once it has at least an absolute majority of PR approvals of all maintainers.
Make sure you check the [list of maintainers](https://github.com/designsystemau/maintainers), since the number of maintainers may vary.

## Who will implement my RFC?

Anyone may pick up an RFC and ask to implement it.
To raise your hands to implement an RFC submit a PR to the RFC document and add your name to the `Implementer: ` section at the top.
