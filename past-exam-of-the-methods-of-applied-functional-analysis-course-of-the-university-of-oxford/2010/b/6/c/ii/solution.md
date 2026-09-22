<h1 id="b/6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In dimension one, the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) gives $H^1(\Omega)\hookrightarrow L^\infty(\Omega)$. Therefore

$$
|\langle A(w,u),v\rangle|\leq\|w\|_\infty^2\|\nabla u\|_2\|\nabla v\|_2,
$$

and, for fixed $w$,

$$
\langle A(w,u)-A(w,z),u-z\rangle=\int_\Omega w^2|\nabla(u-z)|^2\geq0.
$$

Hence **the operator is well-defined and monotone in one dimension**.

In every dimension $n\geq2$ it is **not well-defined on all of $H^1\times H^1$**. We exhibit $w=u=v\in H^1$ for which the purported pairing $\int w^2|\nabla w|^2$ is infinite. Choose a ball compactly contained in $\Omega$, put $r=|x-x_0|$, and multiply each following radial expression by a smooth [cutoff function](../../../../../../cutoff-function.md) that equals one near $r=0$.

For $n\geq3$, set $w=r^{-\alpha}$ with $\alpha=(n-2)/3$. The local [Sobolev norm](../../../../../../sobolev-norm.md) is finite because

$$
\int_0^\delta r^{n-1-2\alpha}\,dr<\infty,\qquad\int_0^\delta r^{n-3-2\alpha}\,dr<\infty,
$$

whereas

$$
\int_{B_\delta}w^2|\nabla w|^2\,dx\asymp\int_0^\delta r^{n-3-4\alpha}\,dr=\infty,
$$

since $n-3-4\alpha=(-n-1)/3<-1$.

For $n=2$, take $w=(\log(1/r))^{1/3}$ on a sufficiently small ball. With $s=\log(1/r)$, the gradient integral is proportional to $\int^\infty s^{-4/3}\,ds<\infty$, while the weighted integral is proportional to $\int^\infty s^{-2/3}\,ds=\infty$. Its $L^2$ integral is finite because the area factor contributes exponential decay in $s$. These singular functions have the indicated [weak derivatives](../../../../../../weak-derivative.md); deleting a small central ball and passing to the limit in [integration by parts](../../../../../../integration-by-parts.md) leaves no boundary term.

Thus $w^2\nabla u\cdot\nabla v$ need not be integrable in dimensions at least two. This is the [squared Sobolev gradient counterexample](../../../../../../squared-sobolev-gradient-counterexample.md). With the additional restriction $w\in L^\infty$, the form is well-defined and monotone in any dimension.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
