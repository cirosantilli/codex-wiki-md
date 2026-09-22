# Last-achiever algorithm for precondition-free planning

↑ **Parent:** [Precondition-free STRIPS planning](precondition-free-strips-planning.md)

Start with required facts $R=G$. If $R\subseteq I$, the empty prefix suffices. Otherwise choose an action adding a member of $R$ and deleting none of $R$, record it as a final action, and remove its add effects from $R$. Repeat and reverse the recorded actions when the residual requirements hold initially. Reject if no permitted action exists.

Soundness follows because each recorded last action supplies its removed requirements without deleting the remaining ones. If a [plan](plan.md) satisfies a residual $R$ not contained in $I$, its last action affecting $R$ cannot delete an $R$-fact and must add one; therefore a candidate exists. Any selected candidate leaves a smaller required set, which is no harder to achieve than $R$. This proves completeness by [mathematical induction](mathematical-induction.md). Every selection removes a required fact, so there are at most $|G|$ selections and a scan of all effect lists at each step gives [polynomial time](polynomial-time.md).

## ↑ Ancestors (5)

1. [Precondition-free STRIPS planning](precondition-free-strips-planning.md)
2. [STRIPS](strips.md)
3. [Artificial intelligence](artificial-intelligence-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/3/f/solution.md)
- [Precondition-free STRIPS planning](precondition-free-strips-planning.md)
