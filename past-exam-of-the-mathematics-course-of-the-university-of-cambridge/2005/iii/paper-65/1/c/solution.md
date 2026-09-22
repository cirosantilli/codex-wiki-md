<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [translation-covariant phase expansion](../../../../../../translation-covariant-phase-expansion.md) with $\xi=x+\phi(Y,T)$, $Y=\varepsilon y$ and $T=\varepsilon^4t$. Write all fast profiles at $\xi$, including the corrections. Let

$$
B=1+\partial_\xi^2,\quad
\mathcal D_Y=\partial_Y+\phi_Y\partial_\xi,\quad
L=r-B^2-3w_0^2.
$$

The [Swift–Hohenberg equation](../../../../../../swift-hohenberg-equation.md) has steady equation $rw_0-B^2w_0-w_0^3=0$, and differentiation gives $Lw_0'=0$. On a fast periodic cell $L$ is a [self-adjoint operator](../../../../../../self-adjoint-operator.md). We assume the translation mode is its only zero mode; otherwise one must impose the corresponding additional [Fredholm solvability conditions](../../../../../../fredholm-solvability-condition.md) and retain additional amplitudes.

Since $\nabla^2=\partial_\xi^2+\varepsilon^2\mathcal D_Y^2$, its squared operator is $B^2+2\varepsilon^2B\mathcal D_Y^2+\varepsilon^4\mathcal D_Y^4$. The time derivative first contributes at order $\varepsilon^4$. At order $\varepsilon^2$,

$$
Lw_2=2B\mathcal D_Y^2w_0
=2\left[(w_0''''+w_0'')\phi_Y^2+(w_0'''+w_0')\phi_{YY}\right].
$$

The [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) is orthogonality of this forcing to $w_0'$. Periodic [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\langle w_0'(w_0''''+w_0'')\rangle=0,\qquad
J:=\langle w_0'(w_0'''+w_0')\rangle
=\langle (w_0')^2-(w_0'')^2\rangle.
$$

Thus the condition is $2J\phi_{YY}=0$. General slowly curved rolls require $J=0$ at leading order. If $J=O(\varepsilon^2)$, this order-$\varepsilon^2$ residual first enters the order-$\varepsilon^4$ equation, so the leading order-$\varepsilon^2$ problem is solvable. In particular,

$$
\boxed{\langle(w_0')^2+w_0'w_0'''\rangle=O(\varepsilon^2)}
$$

is precisely the near-threshold condition. Defining $N=\langle(w_0')^2\rangle>0$ and $J=-\varepsilon^2\lambda N/2$ keeps the residual as the phase-diffusion term at the next order.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
