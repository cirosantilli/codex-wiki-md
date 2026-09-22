<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

Let $u=\phi_1-\phi_2$. It is a [harmonic function](../../../../../harmonic-function.md) in the bounded region and vanishes on its entire boundary. For smooth solutions and boundary, the [divergence theorem](../../../../../divergence-theorem.md) applied to $u\nabla u$ gives the energy identity

$$
\int_R|\nabla u|^2dV
=\int_Su\,\partial_nu\,dS-\int_Ru\nabla^2u\,dV=0.
$$

The integrand is nonnegative, so $\nabla u=0$ in $R$. Thus $u$ is constant on each connected component, and its zero [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) makes every constant zero. Hence

$$
\boxed{\phi_1=\phi_2}.
$$

This proves the [Uniqueness of the Dirichlet problem](../../../../../uniqueness-of-the-dirichlet-problem.md) rather than assuming it.

For the separated expression, write $\phi=F(x)G(y)$. The hyperbolic factor obeys $F''=\lambda^2F$ and the trigonometric factor obeys $G''=-\lambda^2G$, so

$$
\phi_{xx}+\phi_{yy}=F''G+FG''=0
$$

for all the constants, including $\lambda=0$. In the half-strip take $a>0$ so the region has positive width. For every nonzero integer $n$, the decaying [harmonic sine mode in a half-strip](../../../../../harmonic-sine-mode-in-a-half-strip.md) is

$$
\boxed{\phi(x,y)=e^{-|n|\pi x/a}\sin\left(\frac{n\pi y}{a}\right)}.
$$

Its second derivatives cancel, it vanishes at $y=0,a$, and it has the prescribed sine trace at $x=0$. The absolute value in the exponential ensures decay for negative as well as positive $n$. For $n=0$, the zero function is the solution. Thus all integer cases are covered, and the decay is uniform across the strip.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
