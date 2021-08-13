# Australian Government Design System RFCs

> A place to submit, discuss and host Request for Comments (RFCs)

## What are RFCs?

An RFC (Request for Comments) is a document, in our case a markdown file, that seeks to suggest a change to a software, in our case the [Australian Government Design System](https://github.com/designsystemau/design-system-components), by outlining:

- The problem it seeks to fix
- An overview of the proposed change
- Technical description

## How do I submit an RFC?

If you have identified a change you'd like to see in the [Australian Government Design System](https://github.com/designsystemau/design-system-components) then please submit an RFC to [this repository](https://github.com/designsystemau/RFCs).

1. Duplicate `RFCs/RFC-by-stage/1-approved/_RFC-template.md` to `RFCs/RFC-by-stage/1-approved/[YOUR RFC NAME].md`
2. Fill out all the sections
   - Do not change the status at the top of the file
   - Do not remove the `_RFC-template.md` file
3. Submit your PR

Open a [new PR](https://github.com/designsystemau/RFCs/compare) to this repository and use [the template](RFCs/1-approved/_RFC-template.md) as a starting point and fill it with the information you have.

(💡 The template comes with hints and sections to help you navigate it.)

## What are the stages of an RFC?

An RFC can be merged when it receives an absolute majority of approvals from [Maintainers](https://github.com/orgs/designsystemau/teams/maintainers).

1. The first stage a new RFC will be in is `draft` while it is being discussed in the PR stage.
2. The second stage is `approved` after it is merged into the `RFCs/1-approved/` folder.
3. The third stage is `ready-for-implementation` which means the RFC is looking for people to implement it. Come here if you're looking to contribute.
4. The forth stage is `being-implemented` and this is where all RFCs land when they have not been finished but have dedicated people working on it already. The people implementing will be noted at the top of the RFC.
5. The fifth stage is `implemented` and that's where all RFCs land when they have been finished and are live.

## How will my RFC be approved?

[Maintainers](https://github.com/designsystemau/maintainers) will look at your RFC and discuss it in your PR.

You can also ask for help with the RFC process on Slack at [#ref-help](https://govau-guides.slack.com/archives/C02B0046A5T).

An RFC can be merged once it has an absolute majority of PR approvals of all maintainers.

Make sure you check the [list of maintainers](https://github.com/orgs/designsystemau/teams/maintainers), since the number of maintainers may vary.

## Who will implement my RFC?

Anyone may pick up an RFC and ask to implement it.

To raise your hands to implement an RFC submit a PR to the RFC document and add your name to the `Implementer: ` section at the top.
