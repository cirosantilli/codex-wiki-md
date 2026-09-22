<h1 id="b/8/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First state the normalization needed for the displayed logarithmic factorization: choose a continuous [holomorphic function](../../../../../../holomorphic-function-split.md) branch $L=\log F$ in the strip that tends to zero at both horizontal ends and has sufficient decay for its [Cauchy integrals](../../../../../../cauchy-transform.md). In particular the index of the kernel along a horizontal line must be zero.

Choose $\alpha<c_+<c_-<\beta$ and let $\Gamma_\pm=\{\xi+ic_\pm:\xi\in\mathbb R\}$, both oriented from left to right. Put

$$
C_\pm L(z)=\frac1{2\pi i}\int_{\Gamma_\pm}
\frac{L(\zeta)}{\zeta-z}\,d\zeta.
$$

The first is analytic above the lower line and the second below the upper line. On the region between the lines, closing a rectangle gives $C_+L-C_-L=L$: the lower horizontal side is traversed forward and the upper side backward. Hence

$$
F_\pm=e^{C_\pm L},\qquad \frac{F_+}{F_-}=F.
$$

The equation $Fw_+=w_-$ becomes $F_+w_+=F_-w_-$ on the [overlap region](../../../../../../overlap-region.md). With the canonical bounded factors normalized at infinity, these two products glue to a bounded [entire function](../../../../../../entire-function.md). Part (a) gives

$$
\boxed{F_+w_+=F_-w_-=C.}
$$

This is [Wiener-Hopf factorization](../../../../../../wiener-hopf-factorization.md) with the quotient convention used in this question.

The source hypotheses require a qualification: nonvanishing in the strip and $F\to1$ do not by themselves force index zero or a [logarithm](../../../../../../logarithm.md) tending to zero at both ends. For example

$$
F(z)=\frac{z-i}{z+i}
$$

is analytic and nonzero for $|\operatorname{Im}z|<1/2$, tends to one at both ends, but winds once around zero along the real line. A [logarithm](../../../../../../logarithm.md) continued along that line changes by $2\pi i$, so it cannot have the stated normalization at both ends. One must first separate the index factor, or allow appropriately subtracted factors and a correspondingly different common-function growth class. The displayed constant conclusion follows under the canonical zero-index assumptions above; it is not an unconditional consequence of the two printed properties of $F$. This is the issue measured by the [Index of a Wiener-Hopf kernel](../../../../../../index-of-a-wiener-hopf-kernel.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [I](../../i.md)
3. [8](../../../8.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../../split.md)
7. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
