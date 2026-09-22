<h1 id="22f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The defining integral is well-defined and bounded for every dimension: $|\mathcal Ff|\leq\|f\|_1$ and the multiplier is supported on a finite-[volume](../../../../../../volume.md) ball. However **the asserted general-dimensional $L^1$ conclusion is false for the Euclidean radial cutoff printed in the original PDF**. The [nonintegrability of a radial triangular Fourier cutoff in three dimensions](../../../../../../nonintegrability-of-a-radial-triangular-fourier-cutoff-in-three-dimensions.md) is a source issue, not an omitted conjugate or OCR substitution.

For a direct counterexample in $n=3$, take the [Schwartz function](../../../../../../schwartz-function.md) $f(x)=e^{-\pi|x|^2}$, whose [Fourier transform](../../../../../../fourier-transform.md) is the same Gaussian. With $r=|x|$ and $a=2\pi r$, radial integration gives

$$
F_R(r)=\frac{4\pi}{a}\int_0^R \rho(1-\rho/R)e^{-\pi\rho^2}\sin(a\rho)\,d\rho.
$$

The amplitude $b(\rho)=\rho(1-\rho/R)e^{-\pi\rho^2}$ vanishes at both endpoints, and $b'(R)=-e^{-\pi R^2}$. Two integrations by parts, with a further one to bound the remainder, give

$$
F_R(r)=-\frac{4\pi e^{-\pi R^2}}{(2\pi r)^3}\sin(2\pi Rr)+O(r^{-4}).
$$

The integral $\int_1^\infty r^2|F_R(r)|\,dr$ diverges logarithmically for every fixed $R>0$. For example, restrict to the periodic subintervals on which $|\sin(2\pi Rr)|\geq1/2$; the error is smaller than half the leading term at sufficiently large $r$. Thus $F_R\notin L^1(\mathbb R^3)$, even for this smooth integrable $f$.

The familiar intended argument is valid in one dimension. There the inverse Fourier kernel is

$$
K_R(x)=R\left(\frac{\sin(\pi Rx)}{\pi Rx}\right)^2\geq0,\qquad\int K_R=1,
$$

and $F_R=K_R*f$ by [Fubini's theorem](../../../../../../fubini-s-theorem.md). Its mass outside any fixed neighbourhood of zero tends to zero by scaling, so

$$
\|K_R*f-f\|_1\leq\int K_R(y)\|f(\cdot-y)-f\|_1\,dy\longrightarrow0
$$

by [continuity](../../../../../../continuous-function.md) of translations in $L^1$. For arbitrary dimension, replacing the radial cutoff by the product $\prod_{j=1}^n(1-|\xi_j|/R)_+$ gives a [tensor product](../../../../../../tensor-product.md) of these integrable kernels and the same [approximate identity](../../../../../../approximate-identity.md) proof. These are explicit valid repairs, not claims that the PDF specified a product cutoff.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
