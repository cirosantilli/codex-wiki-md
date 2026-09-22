<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Solve the [adjoint transport equation](../../../../../../adjoint-transport-equation.md)

$$
\varphi_t+x\varphi_x+\varphi=\psi
$$

backward with terminal value zero. Along the [characteristic flow map](../../../../../../characteristic-flow-map.md) $Z_{t,s}(x)=e^{s-t}x$, the required solution is

$$
\varphi(t,x)
=-\int_t^\infty e^{s-t}\psi\bigl(s,e^{s-t}x\bigr)\,ds.
$$

Differentiation under the integral verifies the equation. If $\psi$ has [compact support](../../../../../../compact-support.md) in $[0,T]\times[-R,R]$, then $\varphi$ vanishes for $t>T$ and for $|x|>R$, so $\varphi\in C_c^1$ as required.

When the initial datum is zero, inserting this $\varphi$ into the [weak formulation](../../../../../../weak-formulation.md) gives

$$
\int_0^\infty\!\int_{\mathbb R}u\psi\,dx\,dt=0
$$

for every $\psi\in C_c^1$. Thus $u=0$ [almost everywhere](../../../../../../almost-everywhere.md). The difference of two bounded weak solutions has zero initial datum, so this proves uniqueness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
