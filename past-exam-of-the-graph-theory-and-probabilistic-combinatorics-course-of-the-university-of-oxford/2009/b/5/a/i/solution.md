<h1 id="b/5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $I_i=\mathbf1_{A_i}$ and $X=\sum_iI_i$. Define

$$
\mu=\sum_i\mathbb P(A_i),\qquad
\Delta=\sum_{\substack{i\ne j\\E_i\cap E_j\ne\varnothing}}\mathbb P(A_i\cap A_j).
$$

The dependency sum is over **ordered** pairs, so each unordered overlapping pair is counted twice. Disjoint prescribed edge sets give [independence](../../../../../../independent-random-variables.md).

Order the events. For each $i$, let $B_i$ be the event that all earlier events fail. Split it as $B_i=C_i\cap D_i$, where $C_i$ excludes earlier events with edge sets disjoint from $E_i$, and $D_i$ excludes the overlapping earlier events. These are [down-sets](../../../../../../down-set.md). The event $A_i$ is a principal [up-set](../../../../../../up-set.md), and it is independent of $C_i$ since their determining edge sets are disjoint.

If some $B_i$ has [probability](../../../../../../probability.md) zero the desired zero-event bound is immediate. Otherwise the allowed conditional correlation inequality gives

$$
\mathbb P(C_i\cap D_i\mid A_i)\geq\mathbb P(C_i\mid A_i)\mathbb P(D_i\mid A_i)
=\mathbb P(C_i)\mathbb P(D_i\mid A_i).
$$

Since $\mathbb P(B_i)\leq\mathbb P(C_i)$, it follows that

$$
q_i:=\mathbb P(A_i\mid B_i)
\geq\mathbb P(A_i)\mathbb P(D_i\mid A_i)
\geq\mathbb P(A_i)-\sum_{\substack{j<i\\E_j\cap E_i\ne\varnothing}}\mathbb P(A_i\cap A_j).
$$

The last step is the [union bound](../../../../../../boole-s-inequality.md) under conditioning on $A_i$. Zero-[probability](../../../../../../probability.md) events may simply be omitted, and a certain event makes the target [probability](../../../../../../probability.md) zero. Finally the sequential product and $1-u\leq e^{-u}$ give

$$
\mathbb P(X=0)=\prod_i(1-q_i)
\leq\exp\left(-\sum_iq_i\right)
\leq\boxed{e^{-\mu+\Delta/2}}.
$$

This proves the first [Janson inequality](../../../../../../janson-inequality.md) with the dependency-sum convention explicit.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
