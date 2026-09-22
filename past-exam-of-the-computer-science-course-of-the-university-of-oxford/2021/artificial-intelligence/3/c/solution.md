<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**There are $G=2mn+n(n-1)$ distinct [ground actions](../../../../../ground-action.md), or $tG$ time-indexed action [variables](../../../../../variable-mathematics.md) over $t$ transition steps.** Each of [STRIPS](../../../../../strips.md)'s pick and drop [action schemas](../../../../../action-schema.md) has $mn$ type-correct instantiations. A move chooses an ordered pair of distinct buckets, giving $n(n-1)$. Every physical action is a [ground action](../../../../../ground-action.md) before it receives a time index in [SATPlan](../../../../../satplan.md).

$$
\boxed{G=2mn+n(n-1),\qquad G_t=t\,[2mn+n(n-1)]=O\bigl(t(mn+n^2)\bigr).}
$$

These counts exclude static type checks after [action grounding](../../../../../action-grounding.md) and exclude optional persistence/no-op action symbols. Using [successor-state axioms](../../../../../successor-state-axiom.md) supplies persistence without separate no-op action [variables](../../../../../variable-mathematics.md). If one action occurrence is allowed per layer, it is selected from the same ground-action set; a parallel encoding also begins with these physical [ground actions](../../../../../ground-action.md), but has a different exclusion policy.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
