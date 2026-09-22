<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Refining space alone at fixed positive time step does not generally converge.** The diffusion [Courant number](../../../../../../courant-number.md) is $\widehat\sigma^2k/h^2$, which grows by four at each halving of $h$. For positive volatility it eventually violates the explicit diffusion [stability](../../../../../../stability-of-a-numerical-method.md) restriction. The [explicit log-price scheme for local-volatility pricing](../../../../../../explicit-log-price-scheme-for-local-volatility-pricing.md) then amplifies grid-scale errors, rather than approaching the pricing solution.

The strike kink makes the failure concrete. At the terminal node $x_i=\log K$, $u_i^m=0$, while $D_{xx}u_i^m=K/h+O(1)$. Even a single step of fixed size $k$ gives $u_i^{m-1}=ka_i^mK/h+O(1)$, unbounded as $h\downarrow0$ if $a_i^m>0$. Thus the problem is not cured by monitoring exactly at the money. A stable joint space-time refinement is required; the zero-diffusion case does not support the same diffusion argument and centered explicit advection has its own [stability](../../../../../../stability-of-a-numerical-method.md) problem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
