<h1 id="30a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Convexity and the quadratic growth bound imply $|F_u(v,x)|\le C(1+|v|)$ uniformly in $x$. Indeed bound the derivative between the two secant slopes with increments $\pm(1+|v|)$ and use the upper and lower bounds on $F$. This makes $F_u(u,x)$ square integrable and justifies differentiating the energy in every $H_0^1$ direction by domination. At the minimizer,

$$
\int_\Omega\nabla u\cdot\nabla\varphi\,dx+\int_\Omega F_u(u,x)\varphi\,dx=0\qquad(\varphi\in H_0^1(\Omega)).
$$

Thus the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is the elliptic boundary problem

$$
\boxed{-\Delta u+F_u(u,x)=0\ \text{in }\Omega,\qquad u|_{\partial\Omega}=0,}
$$

initially in the weak sense. The zero [trace](../../../../../../matrix-trace.md) is part of the variational space, not an additional unconstrained endpoint variation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [30A](../../30a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
