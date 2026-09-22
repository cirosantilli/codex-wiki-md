<h1 id="j/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In vacuum the source-free equations are

$$
\nabla\cdot\mathbf E=\nabla\cdot\mathbf B=0,\qquad\nabla\times\mathbf E=-\mathbf B_t,\qquad\nabla\times\mathbf B=c^{-2}\mathbf E_t.
$$

Adding the divergence equations with weights $1,ic$ gives the complex divergence equation. Adding the curl equations in the same way gives $\nabla\times\mathbf W=(i/c)\mathbf W_t$. Conversely real and imaginary parts of these two complex equations recover all four real equations.

For the cosine ansatz, differentiation yields divergence $(\boldsymbol\Omega\cdot\mathbf K)\sin(\omega t-\mathbf K\cdot\mathbf x)$ and curl $-(\boldsymbol\Omega\times\mathbf K)\sin(\omega t-\mathbf K\cdot\mathbf x)$. The time [derivative](../../../../derivative.md) is $-\omega\boldsymbol\Omega\sin(\omega t-\mathbf K\cdot\mathbf x)$. Since that sine is not identically zero, the required conditions are precisely

$$
\boxed{\boldsymbol\Omega\cdot\mathbf K=0,\qquad\boldsymbol\Omega\times\mathbf K=(i\omega/c)\boldsymbol\Omega.}
$$

Dotting the second equation with $\boldsymbol\Omega$ gives $\boldsymbol\Omega\cdot\boldsymbol\Omega=0$ because $\omega\ne0$. This dot product is complex bilinear, not Hermitian. Taking the [cross product](../../../../cross-product.md) again with $\mathbf K$ and using transversality gives $-|\mathbf K|^2\boldsymbol\Omega=-\omega^2\boldsymbol\Omega/c^2$. Nonzero amplitude therefore requires $\boxed{|\mathbf K|^2=\omega^2/c^2}$.

Taking real and imaginary parts yields the full conditions

$$
\boxed{\mathbf e\cdot\mathbf K=\mathbf b\cdot\mathbf K=0,\quad\mathbf K\times\mathbf e=\omega\mathbf b,\quad\mathbf b\times\mathbf K=(\omega/c^2)\mathbf e.}
$$

They imply $\mathbf e\cdot\mathbf b=0$ and $|\mathbf e|=c|\mathbf b|$, together with the dispersion relation. Conversely a nonzero transverse $\mathbf e$, this dispersion relation and $\mathbf b=\mathbf K\times\mathbf e/\omega$ satisfy all the conditions.

The physical [fields](../../../../field.md) are $\mathbf E=\mathbf e\cos(\omega t-\mathbf K\cdot\mathbf x)$ and $\mathbf B=\mathbf b\cos(\omega t-\mathbf K\cdot\mathbf x)$. Each oscillates along one fixed real direction, so **both [fields](../../../../field.md) are linearly polarized**. Complex encoding of the two [fields](../../../../field.md) here does not mean either real [field](../../../../field.md) is circularly polarized.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [J](../../j.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
