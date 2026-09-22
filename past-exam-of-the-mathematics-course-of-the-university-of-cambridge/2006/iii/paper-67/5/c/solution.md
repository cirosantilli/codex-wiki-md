<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the general [B-spline interpolation operator norm](../../../../../../b-spline-interpolation-operator-norm.md) estimate in part (I) to the inverse [norm](../../../../../../norm.md) from (b):

$$
\boxed{\|P_{\mathbf x}\|_{L^\infty}\leq\|A_n^{-1}\|_{\ell^\infty}<3,}
$$

and hence in particular $\|P_{\mathbf x}\|_{L^\infty}\leq3$, independently of $n$. The strict finite-dimensional estimate uses the actual finite collocation [matrix](../../../../../../matrix.md); it does not require periodic closure, natural boundary conditions or endpoint knot repetitions.

There is also a direct shorter verification of the uniform bound. For an index $i$ maximizing $|z_i|$, the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\|A_nz\|_{\ell^\infty}\geq|(A_nz)_i|\geq\left(\frac23-\frac16-\frac16\right)\|z\|_{\ell^\infty}=\frac13\|z\|_{\ell^\infty},
$$

with an even larger margin when a neighbor is missing. This is the [inverse infinity-norm bound from diagonal dominance](../../../../../../inverse-infinity-norm-bound-from-diagonal-dominance.md), and again gives $\|A_n^{-1}\|_{\ell^\infty}\leq3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
