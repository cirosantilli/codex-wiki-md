<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u_j\in C_c^\infty(\mathbb R^n)$ tend to $u$ in the [Sobolev space](../../../../../../sobolev-space-split.md) $W^{1,p}$, using [density of smooth functions in a Sobolev space](../../../../../../density-of-smooth-functions-in-a-sobolev-space.md). Write $\alpha=1-n/p>0$. Applying the [Morrey inequality on a cube](../../../../../../morrey-inequality-on-a-cube.md) to a unit cube centered at $x$, and bounding its average by the [Holder inequality](../../../../../../holder-inequality.md), gives

$$
|v(x)|\leq\|v\|_{L^p(\mathbb R^n)}+C\|Dv\|_{L^p(\mathbb R^n)}
$$

for every smooth $v$. Hence $u_j$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the supremum norm and has a bounded continuous limit $u^*$ by [uniform convergence](../../../../../../uniform-convergence.md). On every finite-measure cube, this limit is also the $L^p$ limit, so $u=u^*$ [almost everywhere](../../../../../../almost-everywhere.md).

For $x\ne y$, choose $r=4|x-y|$, so that $y\in Q_r(x)$. The second estimate from part (a), followed by passage to the limit, gives

$$
|u^*(y)-u^*(x)|\leq C|y-x|^\alpha\|Du\|_{L^p(\mathbb R^n)}.
$$

Thus $u^*$ is a [Hölder continuous function](../../../../../../holder-condition.md) and

$$
\boxed{u^*\in C^{0,1-n/p}(\mathbb R^n),\qquad
\|u^*\|_\infty+[u^*]_{C^{0,1-n/p}}\leq C\|u\|_{W^{1,p}}.}
$$

It is the unique continuous representative: two continuous functions agreeing [almost everywhere](../../../../../../almost-everywhere.md) agree everywhere.

For $1\leq p<n$, take a [smooth cutoff function](../../../../../../smooth-cutoff-function.md) $\chi$ equal to one near zero and set

$$
\boxed{u(x)=\chi(x)|x|^{-a},\qquad 0<a<\frac np-1.}
$$

Its [weak derivative](../../../../../../weak-derivative.md) has size $O(|x|^{-a-1})$ near zero, whose $p$th power is integrable because $p(a+1)<n$. Thus $u\in W^{1,p}$, but it is essentially unbounded in every neighborhood of zero and has no continuous representative. The value assigned at zero is irrelevant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
