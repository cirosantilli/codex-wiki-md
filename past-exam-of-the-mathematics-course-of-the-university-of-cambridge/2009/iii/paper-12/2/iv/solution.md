<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Take $\Omega=(0,\pi)$, $a_{11}=1$, $q=1$, $\psi=0$ and $f(x)=\sin x$. The coefficients are bounded and the operator is [uniformly elliptic](../../../../../../uniformly-elliptic-operator.md). If a [weak solution](../../../../../../weak-solution.md) $u\in H_0^1(0,\pi)$ existed, testing its [weak formulation](../../../../../../weak-formulation.md) with $\varphi=\sin x\in H_0^1(0,\pi)$ would give

$$
\int_0^\pi u'\cos x-\int_0^\pi u\sin x=-\int_0^\pi\sin^2x.
$$

By [integration by parts](../../../../../../integration-by-parts.md) for $H_0^1$ functions, the first integral on the left is $\int_0^\pi u\sin x$, so the left side is zero. The right side equals $-\pi/2$, a contradiction. Thus

$$
\boxed{u''+u=\sin x,\quad u(0)=u(\pi)=0\text{ has no }H^1\text{ weak solution}.}
$$

The forcing is not orthogonal to the homogeneous zero-boundary [eigenfunction](../../../../../../eigenfunction.md) $\sin x$. This is the obstruction described by the [Fredholm alternative for an elliptic Dirichlet problem](../../../../../../fredholm-alternative-for-an-elliptic-dirichlet-problem.md), proved here directly without assuming that theorem.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
