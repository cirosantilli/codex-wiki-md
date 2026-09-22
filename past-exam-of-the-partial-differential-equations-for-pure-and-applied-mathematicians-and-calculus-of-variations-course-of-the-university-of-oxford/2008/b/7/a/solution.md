<h1 id="b/7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With coefficients evaluated along $(x,\bar u,\bar u')$, put $p=f_{vv}$, $r=f_{uv}$ and $s=f_{uu}$. The [second variation](../../../../../second-variation.md) is

$$
q(\phi)=\delta^2I(\bar u)[\phi,\phi]=\int_a^b(p\phi'^2+2r\phi\phi'+s\phi^2)dx.
$$

The [Jacobi equation](../../../../../jacobi-equation.md) in divergence form is $-(pz'+rz)'+rz'+sz=0$; if $r$ is differentiable it is $-(pz')'+(s-r')z=0$. A [conjugate point](../../../../../conjugate-point.md) $c>a$ admits a nonzero Jacobi solution vanishing at $a,c$.

There are two positivity conventions worth distinguishing. Strict pointwise positivity means $q(\phi)>0$ for each nonzero fixed-endpoint variation. Coercive positivity means $q(\phi)\geq c\int\phi'^2$ with one $c>0$ for all such variations; the endpoint Poincaré estimate makes this equivalent to a positive lower bound in the full $H^1$ [norm](../../../../../norm.md). Under the regular Legendre hypothesis $p>0$, the necessary and sufficient Jacobi criterion is **no [conjugate point](../../../../../conjugate-point.md) in $(a,b]$**; in that regular case it gives both strict and coercive positivity. Equivalently the [Jacobi equation](../../../../../jacobi-equation.md) has a solution positive on $[a,b]$, and the square identity

$$
q(\phi)=\int_a^bpz^2[(\phi/z)']^2dx
$$

gives positivity and a uniform derivative lower bound by the positive minimum of $z$ and boundedness of $z,z'$. Conversely a conjugate Jacobi field, extended by zero beyond its second zero, is a nonzero Lipschitz variation with $q=0$, contradicting either positivity convention.

Coercivity itself forces $p>0$: local high-frequency variations make the leading coefficient at least the coercivity constant. Mere strict positivity need not force it, as $q(\phi)=\int\phi^2$ shows. If that weaker convention is intended without regularity, a complete criterion is $p\geq0$, no [conjugate point](../../../../../conjugate-point.md) for every regularized form $q_\eta=q+\eta\int\phi'^2$ with $\eta>0$, and no nonzero zero-endpoint Lipschitz [weak solution](../../../../../weak-solution.md) of the original [Jacobi equation](../../../../../jacobi-equation.md). The regularized criteria imply $q_\eta\geq0$, hence $q\geq0$ by passage to the limit. For a nonnegative quadratic form, $q(\phi)=0$ forces all mixed terms with test variations to vanish, giving exactly the weak Jacobi kernel; excluding it gives strict positivity. Necessity follows in reverse. This specifies the degenerate case without imposing an unstated strict Legendre condition.

For weak local minimality, sufficient conditions are the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) and a coercively positive [second variation](../../../../../second-variation.md) with the stated smoothness. Taylor's remainder is bounded by $\varepsilon\|\phi\|_{H^1}^2$ for small $W^{1,\infty}$ perturbations, so the positive quadratic term dominates it. These are the classical **weak minimum sufficient conditions**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../split.md)
6. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
