<h1 id="16c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $T>0$ and a positive prescribed distance $L$; if $L=0$, the zero-speed journey has zero cost. Minimize $E[V]=\int_0^T(aV^2+b\dot V^2)\,dt$ subject to $V(0)=0$ and the [isoperimetric constraint](../../../../../../isoperimetric-constraint.md) $\int_0^TV\,dt=L$. Introduce a constant [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\lambda$ and the integrand $aV^2+b\dot V^2-\lambda V$. For a variation $\eta$ with $\eta(0)=0$, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\delta E_\lambda=\int_0^T(2aV-\lambda-2b\ddot V)\eta\,dt+2b\dot V(T)\eta(T).
$$

The interior [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is

$$
\boxed{b\ddot V-aV=-\frac\lambda2.}
$$

When terminal speed is free, the same calculation also imposes the [natural boundary conditions for a free endpoint](../../../../../../natural-boundary-conditions-for-a-free-endpoint.md):

$$
\boxed{b\dot V(T)=0.}
$$

One cannot drop this boundary term when interpreting an extremal as a genuine minimum. If $b=0<a$, the interior condition makes $V$ constant; with a continuous zero initial speed and $L>0$ it cannot be attained. In that case [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives the infimum $aL^2/T$, approached by speeds nearly constant except in a short initial layer. For $b>0$, the derivative cost controls such layers and the natural terminal condition matters in parts (b) and (c).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16C](../../16c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
