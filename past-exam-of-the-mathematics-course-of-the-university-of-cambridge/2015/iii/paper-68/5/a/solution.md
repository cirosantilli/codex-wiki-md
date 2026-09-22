<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [energy stability for variable-coefficient reaction diffusion](../../../../../../energy-stability-for-variable-coefficient-reaction-diffusion.md), let $h_x=1/(M+1)$, let $D_h$ be the [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md), and set $V_h=\operatorname{diag}(a_m)$. Use the mesh-weighted [inner product](../../../../../../inner-product.md) $(v,w)_h=h_x\sum_{m=1}^Mv_mw_m$ with the corresponding discrete [L2 norm](../../../../../../l2-norm.md). For zero boundary values, [summation by parts](../../../../../../abel-s-summation-formula.md) gives

$$
(v,D_hv)_h=-\frac1{h_x}\sum_{m=0}^M(v_{m+1}-v_m)^2\leq0.
$$

For a solution, or a difference of two solutions, the [energy method](../../../../../../energy-method.md) gives

$$
\frac12\frac d{dt}\|v\|_h^2=(v,D_hv)_h+(v,V_hv)_h
\leq a_+\|v\|_h^2.
$$

The [Gronwall inequality](../../../../../../gronwall-inequality.md) therefore proves

$$
\boxed{\|v(t)\|_h\leq e^{a_+t}\|v(0)\|_h.}
$$

The constant is independent of $M$, so this is [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) on every fixed finite time interval. The bound allows physical growth if $a_+>0$; [stability](../../../../../../stability-of-a-numerical-method.md) here does not mean uniform boundedness as $t\to\infty$.

There is also a uniform maximum-[norm](../../../../../../norm.md) bound. At a positive spatial maximum the second difference is nonpositive. Applying this observation to $e^{-a_+t}v$ and to its negative gives $\|v(t)\|_\infty\leq e^{a_+t}\|v(0)\|_\infty$. With a perturbing source $r(t)$, the [Duhamel principle](../../../../../../duhamel-s-principle.md) gives the corresponding initial-data bound plus $\int_0^te^{a_+(t-s)}\|r(s)\|\,ds$ in either [norm](../../../../../../norm.md). Thus the estimate controls accumulated residuals as well as initial perturbations.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
