# Sequential SATPlan correctness

↑ **Parent:** [SATPlan](satplan.md)

A sequential [SATPlan](satplan.md) encoding has a complete initial assignment of [planning fluents](planning-fluent.md), final goal constraints, [action precondition axioms](action-precondition-axiom.md), [successor-state axioms](successor-state-axiom.md) and [action exclusion axioms](action-exclusion-axiom.md) allowing at most one action per layer. Zero selected actions is an idle step: the [successor-state axioms](successor-state-axiom.md) preserve all facts. This encodes an upper bound on [plan](plan.md) length rather than forcing exactly $T$ physical actions.

For soundness, read selected [ground actions](ground-action.md) in layer order. The initial assignment is the real initial state. By [mathematical induction](mathematical-induction.md), each selected action has its [preconditions](precondition.md) in the current state and the [successor-state axioms](successor-state-axiom.md) give precisely its add/delete update; an empty layer leaves that state unchanged. The final goal constraint therefore proves that the decoded [plan](plan.md) succeeds. Conversely, take any [plan](plan.md) of length at most $T$, assign its actual state trajectory to the fluent [variables](variable-mathematics.md), select its actions in successive layers and pad with idle layers. All encoding components hold. Complete initial negations and persistence conditions are essential: omitting either can introduce unsupported facts and spurious [plans](plan.md).

## ↑ Ancestors (6)

1. [SATPlan](satplan.md)
2. [Classical planning](classical-planning.md)
3. [Automated planning](automated-planning.md)
4. [Artificial intelligence](artificial-intelligence-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/3/e/solution.md)
