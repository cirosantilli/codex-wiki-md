<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**True.** In the [norm topology](../../../../../../norm-topology.md) on the unit ball, the set $\{x\in B:\|x\|<1/2\}$ is a neighbourhood of zero. If the relative [weak topology](../../../../../../weak-topology-split.md) agrees with it, there are finitely many [continuous linear functionals](../../../../../../continuous-linear-functional.md) $f_1,\ldots,f_m$ and positive $\epsilon_j$ such that

$$
\{x\in B:|f_j(x)|<\epsilon_j\text{ for }1\leq j\leq m\}
\subseteq\{x\in B:\|x\|<1/2\}.
$$

If $\bigcap_j\ker f_j$ contained a nonzero vector, rescaling it to have norm $3/4$ would put it in the left-hand set but not the right-hand set. Therefore $\bigcap_j\ker f_j=\{0\}$. The [linear map](../../../../../../linear-map.md)

$$
x\longmapsto(f_1(x),\ldots,f_m(x))
$$

is injective into a finite-dimensional scalar space, so

$$
\boxed{\dim E\leq m<\infty.}
$$

This proof works for either the open or closed unit-ball convention and does not require completeness.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
