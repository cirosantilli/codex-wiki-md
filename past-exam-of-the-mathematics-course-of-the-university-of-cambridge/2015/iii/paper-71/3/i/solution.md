<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [phase function](../../../../../../phase-function.md) is a real $C^\infty$ function on $X\times(\mathbb R^k\setminus\{0\})$, positively homogeneous of degree one in its frequency variable,

$$
\Phi(x,t\theta)=t\Phi(x,\theta)\quad(t>0),
$$

with nonvanishing total differential $d_{x,\theta}\Phi$. Vanishing of its frequency gradient alone is allowed; those critical directions are relevant to singularities.

With $\langle\theta\rangle=(1+|\theta|^2)^{1/2}$, the [symbol class](../../../../../../symbol-class.md) $\operatorname{Sym}(X;\mathbb R^k;N)=S^N_{1,0}$ consists of [smooth functions](../../../../../../smooth-function.md) $a$ such that, for every $K\Subset X$ and every pair of [multi-indices](../../../../../../multi-index-notation.md),

$$
|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|},\qquad x\in K.
$$

There is no requirement that the constant be uniform in the [derivative](../../../../../../derivative.md) indices. We use $D=(1/i)\partial$; the factors of $i$ do not affect these estimates.

For $b=D_x^\alpha D_\theta^\beta a$, any further [derivative](../../../../../../derivative.md) satisfies

$$
|\partial_x^\mu\partial_\theta^\nu b|=|\partial_x^{\mu+\alpha}\partial_\theta^{\nu+\beta}a|\leq C\langle\theta\rangle^{N-|\beta|-|\nu|}.
$$

Thus **frequency [derivatives](../../../../../../derivative.md) lower symbol order and spatial [derivatives](../../../../../../derivative.md) preserve it**:

$$
\boxed{D_x^\alpha D_\theta^\beta a\in\operatorname{Sym}(X;\mathbb R^k;N-|\beta|).}
$$

This is the differentiation rule in [symbol calculus](../../../../../../symbol-calculus.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
