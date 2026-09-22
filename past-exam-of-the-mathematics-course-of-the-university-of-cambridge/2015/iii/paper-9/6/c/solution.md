<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose nested interior open sets $U\subset\subset V\subset\subset W\subset\subset\Omega$. For small $\sigma$, part (b) gives a smooth equation on $V$ of the form

$$
\Delta u_\sigma=\operatorname{div}F_\sigma+G_\sigma,\qquad F_\sigma=(bu)_\sigma,\quad G_\sigma=(cu)_\sigma+f_\sigma.
$$

The [divergence-forcing interior H1 estimate](../../../../../../divergence-forcing-interior-h1-estimate.md) is

$$
\|u_\sigma\|_{H^1(U)}\leq C\left(\|u_\sigma\|_{L^2(V)}+\|F_\sigma\|_{L^2(V)}+\|G_\sigma\|_{L^2(V)}\right).
$$

One can obtain this estimate directly by testing the smooth equation against $\eta^2u_\sigma$ and applying [Young inequality](../../../../../../young-s-inequality-for-products.md), with a [cutoff function](../../../../../../cutoff-function.md) equal to one on $U$ and supported in $V$. The [approximate identity](../../../../../../approximate-identity.md) and the $L^2$ [convolution](../../../../../../convolution.md) bound give, uniformly in $\sigma$,

$$
\|u_\sigma\|_{L^2(V)}\leq\|u\|_{L^2(W)},\quad\|(bu)_\sigma\|_{L^2(V)}\leq\|b\|_{L^\infty(W)}\|u\|_{L^2(W)},
$$

with analogous bounds for $(cu)_\sigma$ and $f_\sigma$. The coefficients need only be bounded on $W$. Therefore $u_\sigma$ is bounded in $H^1(U)$. It converges to $u$ in $L^2(U)$, and [weak sequential compactness in a Hilbert space](../../../../../../weak-sequential-compactness-in-a-hilbert-space.md) in this [Sobolev space](../../../../../../sobolev-space-split.md) gives $u\in H^1(U)$. Since $U$ was arbitrary, $u\in H^1_{\mathrm{loc}}(\Omega)$.

Now expand the [distributional derivative](../../../../../../distributional-derivative.md):

$$
\Delta u=b\cdot\nabla u+(\operatorname{div}b+c)u+f.
$$

Its right side belongs to $L^2_{\mathrm{loc}}$, so the interior $H^2$ [elliptic regularity](../../../../../../elliptic-regularity.md) estimate gives $u\in H^2_{\mathrm{loc}}$. More generally, if $u\in H^m_{\mathrm{loc}}$ for an integer $m\geq1$, multiplication by the smooth coefficients puts the right side in $H^{m-1}_{\mathrm{loc}}$. Interior [elliptic regularity](../../../../../../elliptic-regularity.md) then gives $u\in H^{m+1}_{\mathrm{loc}}$. This [elliptic regularity bootstrap](../../../../../../elliptic-regularity-bootstrap-with-smooth-lower-order-coefficients.md) proves $u\in H^k_{\mathrm{loc}}$ for every integer $k$.

For any nonnegative integer $\ell$, choose $k>\ell+n/2$. The [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) on compact interior subsets gives $u\in C^\ell_{\mathrm{loc}}$. Taking all $\ell$ proves **$u\in C^\infty(\Omega)$**, for its smooth representative. The first gain from $L^2$ to $H^1$ is the step supplied by the mollified equation; assuming $H^1$ in the initial definition would miss that step.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
