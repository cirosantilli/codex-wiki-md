<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a [smooth cutoff function](../../../../../../smooth-cutoff-function.md) $\eta$ supported in $B_2$, equal to one on $B_1$, with $0\leq\eta\leq1$ and $|D\eta|\leq C$. For $i<n$, put $v_i=D_i u$. The zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) implies that the [tangential boundary derivative](../../../../../../tangential-boundary-derivative.md) $v_i$ vanishes on the flat face. Differentiating the [Poisson equation](../../../../../../poisson-equation.md) gives $\Delta v_i=D_i f$. Test this equation with $\eta^2v_i$. The boundary terms vanish because $v_i=0$ on the flat face and $\eta=0$ near the curved face. [Integration by parts](../../../../../../integration-by-parts.md) in the tangential direction moves $D_i$ off $f$, yielding

$$
\int_{B_2^+}\eta^2|Dv_i|^2
=\int_{B_2^+}fD_i(\eta^2v_i)
-2\int_{B_2^+}\eta v_i Dv_i\cdot D\eta.
$$

This is the essential [Caccioppoli inequality](../../../../../../caccioppoli-inequality.md) step: it involves $f$, rather than $Df$. Expanding $D_i(\eta^2v_i)$ and using the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [Young inequality](../../../../../../young-s-inequality-for-products.md) gives

$$
\int\eta^2|Dv_i|^2
\leq\frac12\int\eta^2|Dv_i|^2
+C\int\bigl(f^2+v_i^2|D\eta|^2\bigr).
$$

The term $f\eta(D_i\eta)v_i$ is bounded by $C f^2+C|D\eta|^2v_i^2$. Absorbing the first term and summing over $i<n$ proves the hinted estimate:

$$
\sum_{i<n}\sum_{j=1}^n\|D_{ij}u\|_{L^2(B_1^+)}^2
\leq C(n)\left(\|Du\|_{L^2(B_2^+)}^2+\|f\|_{L^2(B_2^+)}^2\right).
$$

All mixed second [partial derivatives](../../../../../../partial-derivative.md) are now controlled, since $D_{ni}u=D_{in}u$. The remaining [normal derivative](../../../../../../normal-derivative.md) is recovered from the equation:

$$
D_{nn}u=f-\sum_{i<n}D_{ii}u.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bounds its squared [L2 norm](../../../../../../l2-norm.md) by $n$ times the sum of the squared [L2 norms](../../../../../../l2-norm.md) on the right. Including the already controlled zeroth and first [partial derivatives](../../../../../../partial-derivative.md), and taking square roots, gives the [second-derivative estimate at a flat Dirichlet boundary](../../../../../../second-derivative-estimate-at-a-flat-dirichlet-boundary.md):

$$
\boxed{\|u\|_{W^{2,2}(B_1^+)}\leq C(n)\left(\|u\|_{W^{1,2}(B_2^+)}+\|f\|_{L^2(B_2^+)}\right).}
$$

**The full second-order Sobolev norm is controlled without any norm of $Df$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
