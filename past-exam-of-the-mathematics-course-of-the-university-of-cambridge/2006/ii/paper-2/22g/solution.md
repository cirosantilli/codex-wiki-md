<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

A subset is [nowhere dense](../../../../../nowhere-dense-set.md) when its closure has empty interior. It is of first category, or meagre, when it is a [countable union](../../../../../countable-union.md) of nowhere-dense subsets; otherwise it is of second category.

The [Baire category theorem](../../../../../baire-category-theorem.md) says that in a [complete metric space](../../../../../complete-metric-space.md) every [countable intersection](../../../../../countable-intersection.md) of open [dense subsets](../../../../../dense-set.md) is dense. To prove it, start inside an arbitrary nonempty [open set](../../../../../open-set.md) and choose a [closed ball](../../../../../closed-ball.md) of positive radius there and in the first dense [open set](../../../../../open-set.md). Inductively choose a [closed ball](../../../../../closed-ball.md) inside the interior of the preceding ball and the next dense [open set](../../../../../open-set.md), with radius less than $2^{-n}$. The centres are Cauchy. Completeness gives a limit lying in all the nested [closed balls](../../../../../closed-ball.md), hence in all the dense [open sets](../../../../../open-set.md) and the original [open set](../../../../../open-set.md). Thus a nonempty [complete metric space](../../../../../complete-metric-space.md) is not meagre in itself.

For $p<r\le\infty$, put $E_m=\{x\in\ell^p:\|x\|_p\le m\}$, viewed inside $\ell^r$. Necessarily $p<\infty$. Each $E_m$ is closed: convergence in the $\ell^r$ [norm](../../../../../norm.md) gives coordinatewise convergence, and every finite [partial sum](../../../../../partial-sum.md) of $\sum|x_i|^p$ is bounded by $m^p$ in the limit. Taking the supremum of [partial sums](../../../../../partial-sum.md) proves the assertion.

It has empty interior. Given a point in it and any small $\ell^r$ radius, perturb a block of $N$ coordinates by entries of modulus $\delta N^{-1/r}$, choosing signs to avoid cancelling the existing coordinates. The $\ell^r$ distance is $\delta$, while the resulting $\ell^p$ [norm](../../../../../norm.md) is at least $\delta N^{1/p-1/r}$, exceeding $m$ for large $N$. For $r=\infty$, use entries of modulus $\delta$ on that block. Hence each $E_m$ is [nowhere dense](../../../../../nowhere-dense-set.md), and

$$
\boxed{\ell^p=\bigcup_{m=1}^\infty E_m\text{ is first category in }\ell^r\ (p<r).}
$$

For $r=p$, including $p=\infty$, the space is Banach and so **second category in itself** by Baire. There is no case $r>p$ when $p=\infty$.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
