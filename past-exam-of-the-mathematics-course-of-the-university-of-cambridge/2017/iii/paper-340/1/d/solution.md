<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the smoothness hypotheses in the [smooth-mask vanishing-moment criterion](../../../../../../smooth-mask-vanishing-moment-criterion.md), write any nonzero [integer](../../../../../../integer.md) $j$ as $j=2^r\ell$, where $r\ge0$ and $\ell$ is odd, possibly negative. Iterating the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) exactly $r+1$ times gives

$$
\widehat\varphi(2\pi j+t)=\left[\prod_{n=1}^{r+1}m\left(\frac{2\pi j+t}{2^n}\right)\right]\widehat\varphi\left(\frac{2\pi j+t}{2^{r+1}}\right).
$$

The last [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) factor is $m(\pi\ell+t/2^{r+1})$. Its [derivatives](../../../../../../derivative.md) of all orders less than $p$ vanish at $t=0$, because $\ell$ is odd and the [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) is $2\pi$-periodic. If the remaining factors are $C^{p-1}$ at the displayed arguments, the [product rule](../../../../../../product-rule.md) forces every [derivative](../../../../../../derivative.md) of order less than $p$ of the product to vanish. In particular [compact support](../../../../../../compact-support.md) and a finite [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) supply all these hypotheses. Therefore the [integer-frequency zeros of a scaling function](../../../../../../integer-frequency-zeros-of-a-scaling-function.md) are

$$
\boxed{\widehat\varphi^{(k)}(2\pi j)=0\quad(j\ne0,\ 0\le k<p),\quad\text{with the stated regularity}.}
$$

Under only the printed assumptions, the exact same finite refinement argument gives the [Peano zero](../../../../../../peano-zero.md) $\widehat\varphi(2\pi j+t)=o(|t|^{p-1})$. Indeed, the last [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) factor has that estimate, the other [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) factors are bounded by one almost everywhere by the [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) identity, and the last [Fourier transform](../../../../../../fourier-transform.md) factor is bounded because $\varphi\in L^1$. The estimate initially holds almost everywhere and extends to every $t$ by [continuity](../../../../../../continuous-function.md) of $\widehat\varphi$. It does not imply arbitrary ordinary higher [derivatives](../../../../../../derivative.md). In the [lacunary scaling-phase regularity counterexample](../../../../../../lacunary-scaling-phase-regularity-counterexample.md), $\widehat\varphi=a\widehat\varphi_0$ is nondifferentiable at [dense](../../../../../../dense-set.md) dyadic points next to the isolated integer-frequency zeros of the [smooth](../../../../../../smooth-function.md) base transform. Thus the same regularity qualification is necessary here.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
