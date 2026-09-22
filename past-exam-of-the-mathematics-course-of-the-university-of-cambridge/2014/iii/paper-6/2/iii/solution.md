<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $q:X^*\to X^*/Y$ be the quotient map. Since $Y$ is [norm](../../../../../../norm.md) closed and has finite codimension, the quotient is a finite-dimensional normed space. Choose a basis of its continuous dual and compose its coordinate [linear functionals](../../../../../../linear-functional.md) with $q$. This gives $\phi_1,\ldots,\phi_n\in X^{**}$ such that

$$
Y=\bigcap_{k=1}^n\ker\phi_k,\qquad F=\operatorname{span}\{\phi_1,\ldots,\phi_n\}.
$$

If $Jx\in F$, it vanishes on $Y$. Evaluation at $x$ is weak-star continuous, and $Y$ is weak-star dense, so it vanishes on all of $X^*$. The dual [norm](../../../../../../norm.md) formula gives $x=0$. Hence **$F\cap JX=\{0\}$**.

Assume $X\neq\{0\}$; the zero space is trivially normed by any positive constant. We claim that

$$
\boxed{d=\operatorname{dist}(S_X,F)>0.}
$$

If not, there would be $x_j\in S_X$ and $\psi_j\in F$ with $\|Jx_j-\psi_j\|\to0$. The sequence $\psi_j$ is bounded. Finite-dimensionality of $F$ gives a norm-convergent subsequence with limit $\psi\in F$. Then $Jx_j\to\psi$, and $JX$ is [norm](../../../../../../norm.md) closed because $X$ is Banach. Thus $\psi\in F\cap JX$ and $\|\psi\|=1$, a contradiction. This is [positive distance between a unit sphere and a disjoint finite-dimensional subspace](../../../../../../positive-distance-between-a-unit-sphere-and-a-disjoint-finite-dimensional-subspace.md).

Fix $x\in S_X$, identifying it with $Jx$, and put $\delta=\operatorname{dist}(x,F)\geq d$. On $F+\mathbb Rx$, define $h(\phi+tx)=t\delta$. The distance definition gives

$$
|h(\phi+tx)|=|t|\delta\leq\|\phi+tx\|.
$$

The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) extends it to $\Psi\in X^{***}$ with $\|\Psi\|\leq1$, $\Psi|_F=0$ and $\Psi(x)=\delta$.

Apply part (ii) with the [Banach space](../../../../../../banach-space-split.md) **$X^*$**, its finite-dimensional dual [vector subspace](../../../../../../vector-subspace.md) $E=F+\mathbb Rx\subseteq X^{**}$, and the [bidual space](../../../../../../bidual-of-a-normed-space.md) element $\Psi\in X^{***}$. For every $\eta>0$ it supplies $y_\eta\in X^*$ satisfying

$$
\|y_\eta\|<1+\eta,\qquad\phi(y_\eta)=0\ (\phi\in F),\qquad y_\eta(x)=\delta.
$$

Thus $y_\eta\in Y$. Normalize by $1+\eta$ and let $\eta\downarrow0$ to obtain

$$
\sup_{y\in Y,\ \|y\|\leq1}y(x)\geq\delta\geq d.
$$

Homogeneity gives, for all $x\in X$,

$$
\boxed{d\|x\|\leq\sup_{y\in Y,\ \|y\|\leq1}y(x).}
$$

Consequently a [finite-codimensional weak-star dense dual subspace is norming](../../../../../../finite-codimensional-weak-star-dense-dual-subspace-is-norming.md), with **$c=d$**. Since $Y$ is a real linear [vector subspace](../../../../../../vector-subspace.md) and its ball is symmetric, the same supremum is obtained if an absolute value is inserted. The argument uses near-unit interpolation and a limiting supremum, not an assertion that the supremum is attained.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
