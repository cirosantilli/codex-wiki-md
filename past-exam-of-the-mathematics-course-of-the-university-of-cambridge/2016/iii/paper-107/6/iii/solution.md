<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $p_j=2\kappa^j$, where $\kappa=n/(n-2)>1$. Since $p_j^2/(p_j-1)\leq2p_j$, part (ii), followed by a $p_j$-th root, gives the [Moser iteration](../../../../../../moser-iteration.md) step

$$
\|u\|_{L^{p_{j+1}}(\Omega)}\leq\bigl(C(n)\lambda p_j\bigr)^{1/p_j}\|u\|_{L^{p_j}(\Omega)}.
$$

After $N$ steps,

$$
\|u\|_{L^{p_N}}\leq(C(n)\lambda)^{S_N}
\exp\left(\sum_{j=0}^{N-1}\frac{\log p_j}{p_j}\right)\|u\|_{L^2},
\qquad S_N=\sum_{j=0}^{N-1}\frac1{p_j}.
$$

The [geometric series](../../../../../../geometric-series.md) and its differentiated form give

$$
\sum_{j=0}^\infty\frac1{p_j}=\frac{\kappa}{2(\kappa-1)}=\frac n4,
\qquad
\sum_{j=0}^\infty\frac j{\kappa^j}=\frac{\kappa}{(\kappa-1)^2}.
$$

In particular the exact convergent product is

$$
\prod_{j=0}^\infty(2\kappa^j)^{1/(2\kappa^j)}
=2^{\kappa/(2(\kappa-1))}\kappa^{\kappa/(2(\kappa-1)^2)}<\infty.
$$

The printed hint's equality to a single power of $2\kappa$ is not correct in general; its claimed finiteness is correct and the displayed expression supplies the correction.

On a finite-measure domain, [Lp norms converge to the supremum norm](../../../../../../lp-norms-converge-to-the-supremum-norm.md) for a bounded continuous function. Indeed, the upper bound is $\|u\|_p\leq|\Omega|^{1/p}\|u\|_\infty$; for every $a<\|u\|_\infty$, the set $\{|u|>a\}$ has positive measure, giving $\|u\|_p\geq a|\{|u|>a\}|^{1/p}$. Let $N\to\infty$ in the iteration and use part (i), which gives $\lambda>0$. The [Dirichlet eigenfunction supremum estimate](../../../../../../dirichlet-eigenfunction-supremum-estimate.md) is

$$
\boxed{\sup_\Omega|u|\leq C(n)\lambda^{n/4}\|u\|_{L^2(\Omega)}.}
$$

**The eigenvalue exponent is exactly $n/4$.** The constant depends only on $n$: the supplied zero-boundary [Sobolev inequality](../../../../../../sobolev-inequality.md) has a dimension-only constant, and every product factor above depends only on $\kappa$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
