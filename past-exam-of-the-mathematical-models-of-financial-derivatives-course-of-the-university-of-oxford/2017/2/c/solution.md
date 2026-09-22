<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Black-Scholes reflection symmetry](../../../../black-scholes-reflection-symmetry.md) becomes a weighted reflection after taking a [logarithm](../../../../logarithm.md). Put $x=\log(S/B)$ and $v(x,t)=V(Be^x,t)$. The [multivariable chain rule](../../../../multivariable-chain-rule.md) transforms the equation into

$$
v_t+\tfrac12\sigma^2v_{xx}+bv_x-rv=0,\qquad b=r-\sigma^2/2.
$$

For $w(x,t)=e^{\gamma x}v(-x,t)$, its left-hand side, after removing the factor $e^{\gamma x}$, is

$$
v_t+\tfrac12\sigma^2v_{xx}-(\sigma^2\gamma+b)v_x
+(\tfrac12\sigma^2\gamma^2+b\gamma-r)v,
$$

evaluated at $(-x,t)$. Taking $\gamma=-2b/\sigma^2$ makes the derivative coefficient $b$ and the additional zeroth-order term zero. Thus

$$
\boxed{W(S,t)=(S/B)^{1-2r/\sigma^2}V(B^2/S,t)}
$$

satisfies the same [Black-Scholes equation](../../../../black-scholes-equation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
