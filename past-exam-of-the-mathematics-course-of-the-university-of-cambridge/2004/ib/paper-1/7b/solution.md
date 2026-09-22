<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

In vacuum SI notation, [Maxwell's equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot E=\rho/\epsilon_0,\quad\nabla\cdot B=0,\quad
\nabla\times E=-\partial_tB,\quad
\nabla\times B=\mu_0J+\mu_0\epsilon_0\partial_tE.
$$

Taking the [divergence](../../../../../divergence.md) of the last equation, using that the [divergence](../../../../../divergence.md) of a [curl](../../../../../curl.md) vanishes and then the first equation, gives

$$
0=\mu_0\nabla\cdot J+\mu_0\partial_t\rho,\qquad
\boxed{\partial_t\rho+\nabla\cdot J=0.}
$$

This is local [conservation of electric charge](../../../../../charge-conservation.md). For spatially uniform [electrical conductivity](../../../../../electrical-conductivity.md), [Ohm's law](../../../../../ohm-s-law.md) $J=\sigma E$ gives $\nabla\cdot J=\sigma\rho/\epsilon_0$, so

$$
\boxed{\rho(x,t)=\rho(x,0)e^{-\sigma t/\epsilon_0},\qquad\text{decay rate }\sigma/\epsilon_0.}
$$

For a homogeneous dielectric conductor with permittivity $\epsilon$, replace $\epsilon_0$ by $\epsilon$. This [charge relaxation](../../../../../charge-relaxation.md) is a statement about bulk charge; charge transported to a boundary is still accounted for by the conservation law.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
