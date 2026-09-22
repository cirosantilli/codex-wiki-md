<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [local wave energy estimate](../../../../../../local-wave-energy-estimate.md) is, for $T\geq0$, $r>0$, and any center $x_0$,

$$
\boxed{\int_{B_r(x_0)}(u_t^2+|\nabla u|^2)(T,x)\,dx
\leq\int_{B_{r+T}(x_0)}(g^2+|\nabla f|^2)(x)\,dx.}
$$

To prove it, let $R=r+T$ and integrate the local [energy estimate](../../../../../../energy-estimate.md) identity $\partial_t e=\operatorname{div}(u_t\nabla u)$, where $e=(u_t^2+|\nabla u|^2)/2$, over the shrinking ball $B_{R-t}(x_0)$. Differentiation of this moving-domain integral yields

$$
\frac{d}{dt}\int_{B_{R-t}}e
=\int_{\partial B_{R-t}}\left(u_t\partial_nu-\frac12u_t^2-\frac12|\nabla u|^2\right)\,dS
=-\frac12\int_{\partial B_{R-t}}\left((u_t-\partial_nu)^2+|\nabla_{\mathrm{tan}}u|^2\right)\,dS\leq0.
$$

Integrating in time proves the [local wave energy estimate](../../../../../../local-wave-energy-estimate.md), without assumptions at spatial infinity.

Let the union of the initial [supports](../../../../../../support.md) be a compact set $K$. If $\operatorname{dist}(x_0,K)>T$, choose $r>0$ with $r+T<\operatorname{dist}(x_0,K)$. The initial energy on $B_{r+T}(x_0)$ vanishes. Applying the shrinking-ball identity up to every intermediate time shows $u_t$ and $\nabla u$ vanish throughout that cone. In particular, along the vertical segment through $x_0$, $u_t=0$; its initial value is also zero, so $u(T,x_0)=0$. This last value check removes the constant ambiguity invisible to gradient energy.

Consequently the [finite propagation speed](../../../../../../finite-propagation-speed.md) conclusion is

$$
\boxed{\operatorname{supp}u(t,\cdot)\subseteq\{x:\operatorname{dist}(x,K)\leq|t|\}.}
$$

This set is compact for each finite $t$. The speed is at most one in these units, or $c$ for $u_{tt}-c^2\Delta u=0$. Time reversal gives the same conclusion for negative time.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
