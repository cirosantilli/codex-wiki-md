<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\Delta=\{(x,y):x=y\}$. For any [transport plan](../../../../../../transport-plan.md) $\pi$ and any [Borel set](../../../../../../borel-set.md) $A$,

$$
\mu(A)-\nu(A)=\pi(A\times A^c)-\pi(A^c\times A).
$$

Both rectangles are contained in $\Delta^c$, so

$$
|\mu(A)-\nu(A)|\leq\pi(\Delta^c)=\mathbb K(\pi).
$$

Thus $\inf\mathbb K\geq\sup_A|\mu(A)-\nu(A)|$.

To attain this bound, use the [dominating measure](../../../../../../dominating-measure.md) $\rho=\mu+\nu$ and [Radon-Nikodym derivatives](../../../../../../radon-nikodym-derivative.md) $f=d\mu/d\rho$, $g=d\nu/d\rho$. Define the common measure and residual mass by

$$
d\alpha=\min(f,g)\,d\rho,\qquad r=1-\alpha(\mathbb R^d).
$$

Since $\int(f-g)\,d\rho=0$, the positive and negative parts have equal mass. Taking $A=\{f>g\}$ gives

$$
r=\int(f-g)_+\,d\rho=\frac12\int|f-g|\,d\rho
=\sup_A|\mu(A)-\nu(A)|.
$$

If $r=0$, then $\mu=\nu$ and the diagonal [transport plan](../../../../../../transport-plan.md) has zero cost. If $r>0$, put $\beta=\mu-\alpha$, $\gamma=\nu-\alpha$ and define

$$
\pi^\dagger=(\operatorname{Id},\operatorname{Id})_\#\alpha+\frac1r\,\beta\otimes\gamma.
$$

The residual measures each have mass $r$, so the [marginal distributions](../../../../../../marginal-distribution.md) of $\pi^\dagger$ are $\alpha+\beta=\mu$ and $\alpha+\gamma=\nu$, and its total mass is $1-r+r=1$. They are [mutually singular measures](../../../../../../mutually-singular-measures.md), concentrated respectively on $\{f>g\}$ and $\{g>f\}$. Their [product measure](../../../../../../product-measure.md) therefore gives no mass to $\Delta$, and $\mathbb K(\pi^\dagger)=r$. This is a [maximal coupling](../../../../../../maximal-coupling.md).

In the paper's convention for the zero-mass signed measure $\mu-\nu$, the answer is

$$
\boxed{\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi)
=\sup_A|\mu(A)-\nu(A)|=\frac12\|\mu-\nu\|_{\mathrm{TV}}.}
$$

The repository's [total variation distance](../../../../../../total-variation-distance.md) uses the supremum itself. The paper's formula $2\sup_A|\sigma(A)|$ agrees with the usual total variation norm when $\sigma$ has total mass zero, as here; it is not the usual norm for an arbitrary positive measure. All suprema above are over [Borel sets](../../../../../../borel-set.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
