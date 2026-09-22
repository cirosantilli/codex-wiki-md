<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True.** Choose a norm-dense sequence $(x_n)$ in the unit ball of the separable [normed vector space](../../../../../../normed-vector-space.md) $E$. On the dual unit ball $B'$, define

$$
\boxed{d(\phi,\psi)=\sum_{n=1}^{\infty}2^{-n}|\phi(x_n)-\psi(x_n)|.}
$$

Each summand is at most $2^{1-n}$, so the series converges uniformly. Symmetry and the [triangle inequality](../../../../../../triangle-inequality.md) follow term by term. If $d(\phi,\psi)=0$, the two continuous functionals agree on the dense sequence, hence on the unit ball and then on all of $E$. Thus $d$ is a [metric](../../../../../../metric.md).

A relative weak-star neighbourhood controls finitely many evaluations. Conversely, to make $d$ small, first choose a tail whose sum is small and then control the finitely many evaluations at $x_1,\ldots,x_N$. This proves that each [metric](../../../../../../metric.md) ball is weak-star open. For the other direction, let $x\in E$ and $\epsilon>0$. Approximate $x/\|x\|$ by $x_n$ when $x\ne0$. Since $\|\phi-\psi\|\leq2$ on $B'$,

$$
|\phi(x)-\psi(x)|
\leq\|x\|\,|\phi(x_n)-\psi(x_n)|+2\|x\|\,\|x/\|x\|-x_n\|.
$$

The second term can be made smaller than $\epsilon/2$ by choosing $n$; the first is smaller than $\epsilon/2$ whenever $d(\phi,\psi)$ is sufficiently small, because $|\phi(x_n)-\psi(x_n)|\leq2^n d(\phi,\psi)$. Every evaluation is therefore metric-continuous. These two inclusions show that $d$ induces exactly the [weak-star topology](../../../../../../weak-star-topology.md), proving [weak-star metrizability of the dual ball](../../../../../../weak-star-metrizability-of-the-dual-ball.md) without a completeness assumption on $E$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
