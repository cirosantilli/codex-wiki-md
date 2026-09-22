<h1 id="34a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Vary the [four-potential](../../../../../../electromagnetic-four-potential.md) with compactly supported variation. Antisymmetry of the [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md) gives $\delta(F_{\mu\nu}F^{\mu\nu})=4F^{\mu\nu}\partial_\mu\delta A_\nu$. Integration by parts therefore gives

$$
\delta S=\frac1{\mu_0c}\int[\partial_\mu F^{\mu\nu}-\lambda^2A^\nu+\mu_0J^\nu]\delta A_\nu\,d^4x.
$$

Thus **the Euler-Lagrange field equation is** $\boxed{\partial_\mu F^{\mu\nu}-\lambda^2A^\nu=-\mu_0J^\nu}$.

A [gauge transformation](../../../../../../gauge-transformation.md) is $A_\mu\mapsto A_\mu+\partial_\mu\chi$. Commuting derivatives leave $F_{\mu\nu}$ unchanged. At $\lambda=0$, the source term changes by $c^{-1}\int\partial_\mu\chi J^\mu$, a boundary term because the current is conserved. With suitable boundary conditions the action is gauge invariant. For $\lambda>0$, the mass term changes by terms involving $2A^\mu\partial_\mu\chi+(\partial\chi)^2$, so **the same arbitrary gauge transformations are not a symmetry**.

Take the divergence of the field equation. Antisymmetry gives $\partial_\nu\partial_\mu F^{\mu\nu}=0$, and conservation gives $\partial_\nu J^\nu=0$. Thus $\lambda^2\partial_\nu A^\nu=0$. For $\lambda>0$ this is the [Lorenz constraint in Proca theory](../../../../../../lorenz-constraint-in-proca-theory.md), and expanding $F$ gives

$$
\boxed{(\Box-\lambda^2)A^\nu=-\mu_0J^\nu.}
$$

For $\lambda=0$ the same reduced equation holds when the [Lorenz gauge](../../../../../../lorenz-gauge-condition.md) $\partial_\mu A^\mu=0$ is imposed. More generally it is enough that the divergence be spacetime constant, but the conventional vanishing boundary conditions set that constant to zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [34A](../../34a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
