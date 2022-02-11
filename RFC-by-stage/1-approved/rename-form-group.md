---
Status: `Proposal` # Please do not change this.
Implementer: # It will be changed upon merging and as it moves through the RFC stages
---

# Rename form group

## The issue to be solved

Currenty GOLD uses the name `form group` to refer to the elements which make up a single form field (label, hint, error message etc). I believe the naming could be improved as it can be easily mistaken for a collection of form fields and not a single form field.

## A short description of the desired outcome or solution

- (The documentation)[https://gold.designsystemau.org/components/form/#form-groups] is updated to reflect the new name
- `au-form-group` is renamed to `au-field`. 

## Technical details

- Rename CSS class
- No JS changes are necessary 
- Update documentation