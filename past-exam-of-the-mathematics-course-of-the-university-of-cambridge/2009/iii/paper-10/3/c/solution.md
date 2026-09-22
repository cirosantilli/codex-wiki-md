<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We construct the [Jordan decomposition of a bounded functional on C(K)](../../../../../../jordan-decomposition-of-a-bounded-functional-on-c-k.md) directly, without assuming a measure representation. For $f\geq0$, define

$$
P(f)=\sup\{\phi(g):g\in C(K),\ 0\leq g\leq f\}.
$$

This is finite, nonnegative, and positively homogeneous, since $0$ is allowed and $|\phi(g)|\leq\|\phi\|\|f\|_\infty$. If $f,h\geq0$, separately chosen approximate maximizers add to an admissible function for $P(f+h)$, giving $P(f+h)\geq P(f)+P(h)$. For the converse, any $0\leq g\leq f+h$ splits into the [continuous functions](../../../../../../continuous-function.md)

$$
g_1=\min(g,f),\qquad g_2=g-g_1=\max(g-f,0),
$$

with $0\leq g_1\leq f$ and $0\leq g_2\leq h$. Hence $\phi(g)\leq P(f)+P(h)$ and $P$ is additive on the positive cone.

Extend it to a [linear functional](../../../../../../linear-functional.md) by $\phi^+(u-v)=P(u)-P(v)$ for $u,v\geq0$. This is well defined: two decompositions satisfy $u+v'=u'+v$, and additivity gives the same difference. Every continuous real function has such a decomposition, for example into its pointwise positive and negative parts. The extension is positive. Define $\phi^-=\phi^+-\phi$; for $f\geq0$, the choice $g=f$ shows $P(f)\geq\phi(f)$, so $\phi^-$ is also positive. Part (a) makes both [positive linear functionals](../../../../../../positive-linear-functional.md) continuous.

Their [operator norms](../../../../../../operator-norm.md) satisfy

$$
\|\phi^+\|+\|\phi^-\|=2P(1)-\phi(1)
=\sup_{0\leq g\leq1}\phi(2g-1)
=\sup_{\|h\|_\infty\leq1}\phi(h)=\|\phi\|.
$$

The last equality uses symmetry of the real unit ball. Therefore

$$
\boxed{\phi=\phi^+-\phi^-,\qquad\|\phi\|=\|\phi^+\|+\|\phi^-\|.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
