# Per-action conditions in the rule editor

The rule editor has one condition builder per rule. It does not give a tag action, or any other action, a condition builder of its own. The API still stores and evaluates a condition for each action.

## Why

- One rule for each status covers the case, and the automations documentation describes it: make one rule per tag condition.
- A condition builder on each action makes the rule editor heavier for every user, and few users gain from it.

When the editor opens a rule whose actions have different conditions (a rule made through the API or imported), it shows a warning that a save applies one condition to every action.

## Prior requests

- #2771
