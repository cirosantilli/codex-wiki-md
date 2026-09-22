<h1 id="3/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**With the standard Sobolev norm, the printed constant one is not valid for arbitrary $a$.** The constant function $u=1$ has supremum norm one and $H^1$ norm $\sqrt{2a}$, which is smaller when $a<1/2$.

For the continuous [one-dimensional Sobolev representative](../../../../../../../one-dimensional-sobolev-representative.md), let $\bar u=(2a)^{-1}\int_Iu$. The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) gives $|\bar u|\le(2a)^{-1/2}\|u\|_2$. Using the preceding [Hölder seminorm](../../../../../../../holder-seminorm.md) estimate,

$$
|u(x)-\bar u|\le\frac1{2a}\int_I|u(x)-u(y)|\,dy\le\sqrt{2a}\|u'\|_2.
$$

Consequently the corrected [interval Sobolev supremum estimate](../../../../../../../interval-sobolev-supremum-estimate.md) is

$$
\boxed{\|u\|_\infty\le(2a)^{-1/2}\|u\|_2+\sqrt{2a}\|u'\|_2\le\sqrt{(2a)^{-1}+2a}\,\|u\|_{H^1(I)}.}
$$

One may first prove this for smooth approximations and pass on the full-measure convergence set. Averaging differences also handles complex-valued functions without assuming that a function takes its complex average at some point. At the fixed interval used below the constant is absolute, which suffices for the intended interior estimate.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
