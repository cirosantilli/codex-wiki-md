<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $\kappa=(a^2/3-b)^{1/2}>0$, $\sigma=-c+ab/3-2a^3/27$, and use the [gauge reduction of a third-order half-line equation](../../../../../../gauge-reduction-of-a-third-order-half-line-equation.md)

$$
x=\kappa X,\qquad t=\kappa^3T,\qquad Q(X,T)=e^{-aX/3+\sigma T}q(x,t).
$$

The spatial differential operator acting on $q$ is obtained by replacing $\partial_X$ with $\kappa\partial_x-a/3$. Its second-derivative coefficient vanishes. The first-derivative coefficient is $\kappa(b-a^2/3)=-\kappa^3$, and the constant coefficient is $c-ab/3+2a^3/27=-\sigma$. The time derivative supplies $\sigma q+\kappa^3q_t$, so all constant terms cancel and the remaining equation is $\kappa^3(q_t+q_{xxx}-q_x)=0$.

The transformed [initial condition](../../../../../../initial-condition.md) and [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) are therefore

$$
\boxed{q_0(x)=e^{ax/(3\kappa)}Q_0(x/\kappa),\qquad g_0(t)=e^{-\sigma t/\kappa^3}G_0(t/\kappa^3).}
$$

Compatibility at the corner is preserved. Since $a<0$, this exponential gauge improves the spatial decay of the initial data, which supports convergence of its [Half-range Fourier transform](../../../../../../half-range-fourier-transform.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
