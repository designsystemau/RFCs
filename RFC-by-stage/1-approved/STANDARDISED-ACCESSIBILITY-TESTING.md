---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Standardised manual accessibility testing

## The issue to be solved

Web accessibility is too subjective. Reading the WCAG success criteria is challenging and trying to agree on what constitutes a failure is hard, multiple people may have multiple views each slightly different. Normative failings (things which must pass) in WCAG becomes conflated with accessibility best practice and what people *feel* is poor accessibility. Agreeing on what constitutes a failure is the first step towards testing in a consistent way and having consistent results.

Manual accessibility testing is aimed at conveying facts. Tests should strive to avoid personal preferences for identifying accessibility failures.

This article forms the approach
https://www.tpgi.com/heading-off-confusion-when-do-headings-fail-wcag/
> WCAG techniques, such as H42: Using h1-h6 to identify headings and ARIA12: Using role=heading to identify headings, recommend that heading markup indicate the appropriate heading level for the content, but they don’t go so far as to define what’s “appropriate”—an issue that has been the subject of considerable discussion. **So although hierarchical heading structures reflect a best practice, skipping heading levels does not represent a WCAG failure.**

## A short description of the desired outcome or solution

The outcome is a community driven master list of all 50 WCAG 2.1 AA success criteria expanded out into simple easy to understand individual tests. A developer building a component would use the same tests from the same list as a accessibility specialist, accessibility tester, BA or anyone else involved in the accessibility. The tests remove the personal opinions of what people believe is an accessibility failure but isn't and makes it simpler to apply the minimum level of accessibility consistently. 

The master list would invite community input but not every request would be actioned. Requests undergo a rigorous review and require justification that _a). it is a failure_ or _b). the test requires more detail_.

## Technical details

* 103 separate accessibility tests comprising all 50 WCAG 2.1 AA success criteria, as an example https://canaxess.github.io/accessibility-resources/
* filterable by role or component
* excel export functionality

<!--
  Here please go deep into your vision of your solution.
  Provide things like  (if applicable):
    - javascript architecture
    - accessibility concerns
    - designs
    - token usage
    - naming
-->
