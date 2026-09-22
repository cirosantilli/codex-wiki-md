<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [product rule](../../../../product-rule.md) applied at the [interpolation node](../../../../interpolation-node.md) $x_k$ gives

$$
w'(x_k)=\prod_{j\ne k}(x_k-x_j)\ne0,\qquad
\ell_k(x)=\frac{w(x)}{(x-x_k)w'(x_k)}=w(x)\frac{w_k}{x-x_k}.
$$

Thus [Lagrange interpolation](../../../../lagrange-polynomial.md) gives, away from the [interpolation nodes](../../../../interpolation-node.md),

$$
p_n(x)=w(x)\sum_{k=0}^n\frac{w_k f_k}{x-x_k}.
$$

Apply the same [Lagrange interpolation](../../../../lagrange-polynomial.md) formula to the [constant polynomial](../../../../constant-polynomial.md) one. Since its [interpolant](../../../../interpolant.md) is itself,

$$
1=\sum_{k=0}^n\ell_k(x)=w(x)\sum_{k=0}^n\frac{w_k}{x-x_k}.
$$

Dividing the preceding two identities proves the [barycentric interpolation formula](../../../../barycentric-interpolation-formula.md)

$$
\boxed{p_n(x)=\frac{\displaystyle\sum_{k=0}^n w_k f_k/(x-x_k)}{\displaystyle\sum_{k=0}^n w_k/(x-x_k)}.}
$$

The denominator is exactly $1/w(x)$, so is nonzero away from the [interpolation nodes](../../../../interpolation-node.md). At $x=x_j$, multiply numerator and denominator by $x-x_j$ and take the [limit](../../../../limit-of-a-function.md): their values tend to $w_jf_j$ and $w_j$, respectively. The [removable singularity](../../../../removable-singularity.md) therefore has value $f_j$; in numerical evaluation return the stored value directly at an [interpolation node](../../../../interpolation-node.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
