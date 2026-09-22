<h1 id="b/5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Independently retain each event with [probability](../../../../../../probability.md) $t$, using a fresh Bernoulli mark for every index. Its retained occurrence is the original principal [up-set](../../../../../../up-set.md) together with its mark being one, so the first proof applies in the enlarged independent product space. The new parameters are $\mu_t=t\mu$ and $\Delta_t=t^2\Delta$: distinct retained events have independent marks, and pairs of disjoint original supports remain independent.

If no original event occurs, no retained event occurs. Thus

$$
\mathbb P(X=0)\leq\exp(-t\mu+t^2\Delta/2),\qquad0\leq t\leq1.
$$

When $\Delta\geq\mu>0$, choose $t=\mu/\Delta$ to minimize this quadratic exponent. It gives

$$
\boxed{\mathbb P(X=0)\leq\exp\left(-\frac{\mu^2}{2\Delta}\right)}.
$$

If $\mu=0$, the appropriate trivial bound is one, rather than an undefined zero-over-zero exponent. The argument is the [Janson lower-tail bound by independent thinning](../../../../../../janson-lower-tail-bound-by-independent-thinning.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
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
