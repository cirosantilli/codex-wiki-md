<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $|z|>\|L\|$, the [Neumann series](../../../../../../neumann-series.md) gives

$$
(L-zI)^{-1}
=-\frac1z\sum_{n=0}^\infty\left(\frac Lz\right)^n.
$$

The series converges in [operator norm](../../../../../../operator-norm.md) because $\|L/z\|<1$. Hence

$$
\boxed{\Sigma(L)\subset\{z:|z|\leq\|L\|\}.}
$$

The same argument applied to small perturbations of an invertible operator shows that the [resolvent set](../../../../../../resolvent-set-of-an-operator.md) is open and the [spectrum](../../../../../../spectrum-functional-analysis.md) is closed.

Suppose $L=L^*$ and $\operatorname{Im}z\ne0$. The quadratic form $\langle Lh,h\rangle$ is real, so the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) implies

$$
|\operatorname{Im}z|\,\|h\|^2
=|\operatorname{Im}\langle(L-zI)h,h\rangle|
\leq\|(L-zI)h\|\,\|h\|.
$$

Thus $L-zI$ is bounded below by $|\operatorname{Im}z|$: it is injective and has closed range. Its [adjoint operator](../../../../../../adjoint-operator.md) $L-\bar zI$ has the same lower bound and trivial kernel. Since

$$
\operatorname{ran}(L-zI)^\perp=\ker(L-\bar zI)=\{0\},
$$

the range is dense as well as closed, and therefore is all of $H$. The inverse has norm at most $|\operatorname{Im}z|^{-1}$. **For a bounded self-adjoint operator, $\Sigma(L)\subset\mathbb R$.** The closed-range and adjoint steps are essential: merely excluding nonreal [eigenvalues](../../../../../../eigenvalue.md) would not exclude all nonreal spectral points.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
