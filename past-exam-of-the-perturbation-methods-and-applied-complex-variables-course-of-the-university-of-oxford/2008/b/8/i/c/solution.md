<h1 id="b/8/i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same normalized factors and [contours](../../../../../../complex-integration-contour.md) as in part (b), and put $H=GF_-$. Multiplying the inhomogeneous equation by $F_-$ gives

$$
F_+w_+-F_-w_-=H.
$$

The additive Cauchy decomposition has $C_+H-C_-H=H$ on the [overlap region](../../../../../../overlap-region.md). Subtract it from this equation:

$$
F_+w_+-C_+H=F_-w_--C_-H.
$$

Under the same convergence and boundedness assumptions, these expressions are analytic on complementary half-planes, agree on their [overlap region](../../../../../../overlap-region.md), and glue to a bounded [entire function](../../../../../../entire-function.md). Thus

$$
\boxed{
F_+w_+-\frac1{2\pi i}\int_{\Gamma_+}
\frac{G(\zeta)F_-(\zeta)}{\zeta-z}\,d\zeta
=F_-w_--\frac1{2\pi i}\int_{\Gamma_-}
\frac{G(\zeta)F_-(\zeta)}{\zeta-z}\,d\zeta
=C.}
$$

If the decay is too weak for an unsubtracted [Cauchy integral](../../../../../../cauchy-transform.md), the subtraction and resulting common-function growth condition must be specified. Merely asserting pointwise $G\to0$ is not a substitute for the needed [integral transform](../../../../../../integral-transform-split.md) convergence.

## ↑ Ancestors (14)

1. [C](../c.md)
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
