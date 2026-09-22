<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Use seven [variables](../../../../../variable-mathematics.md) $X_A,\ldots,X_G$, with $D_A=\{1\}$ and every other [constraint domain](../../../../../constraint-domain.md) $\{1,2,3,4\}$. Each conflict is a [binary constraint](../../../../../binary-constraint.md) $X_U\ne X_V$.**

The audience assumptions are part of the [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md). Talks occupy whole common-length slots, room capacity and travel times impose no additional restrictions, and different CS year cohorts do not overlap. Physics attendees are treated as separate from those cohorts and the Head of Department. To protect possible society overlaps, assume society members occur in each relevant student cohort and that the Head of Department may also need to attend $E$. No additional overlap between otherwise distinct audience groups is assumed. These are declared modelling choices, rather than claims about the actual membership of any group.

The shared-audience restrictions give the [edge](../../../../../edge-of-a-graph.md) pairs

$$
\{CD,FG,BD,AB,AG,BG,DF\}.
$$

For example, the Head of Department's three introductions produce all three pairwise inequalities on $A,B,G$; the Physics audience gives $D\ne F$. The possible society overlaps add

$$
\{EA,EB,EC,ED,EF,EG\}.
$$

Together these thirteen inequalities and $X_A=1$ give a binary formulation. There is no need for an [all-different constraint](../../../../../all-different-constraint.md) on all seven [variables](../../../../../variable-mathematics.md): compatible talks may run in parallel. At least two rooms suffice for the solution below.

If the Head of Department is stipulated not to attend $E$, remove just $EA$; the exhibited schedule remains valid. If actual society membership excludes a specified cohort, remove its corresponding additional conflicts too. This separation makes clear which restrictions are direct requirements and which protect assumed overlapping attendance.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
