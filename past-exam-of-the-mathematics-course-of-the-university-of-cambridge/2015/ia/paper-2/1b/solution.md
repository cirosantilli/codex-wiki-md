<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

The [integrating factor](../../../../../integrating-factor.md) is $e^{-2x}$, so $(e^{-2x}y)'=e^{(\lambda-2)x}$. Integrating gives **the general solution**

$$
\boxed{y=Ce^{2x}+\frac{e^{\lambda x}}{\lambda-2}\quad(\lambda\ne2).}
$$

The [particular solution](../../../../../particular-solution.md) is only defined up to a [homogeneous solution](../../../../../homogeneous-solution.md). Subtract $e^{2x}/(\lambda-2)$ from it, absorbing that multiple into the arbitrary constant. The same family can then be written

$$
y=\widetilde C e^{2x}+\frac{e^{\lambda x}-e^{2x}}{\lambda-2}.
$$

Holding $\widetilde C$ fixed, the quotient tends to $xe^{2x}$, the derivative of $e^{\lambda x}$ with respect to $\lambda$ at $2$. Thus **the resonant family is $y=e^{2x}(\widetilde C+x)$**. Direct differentiation gives $y'-2y=e^{2x}$, so it is the full general solution at resonance. This [resonant exponential forcing in a first-order equation](../../../../../resonant-exponential-forcing-in-a-first-order-equation.md) limit concerns a reparametrized family, not a fixed value of the original divergent constant $C$. The [initial condition](../../../../../initial-condition.md) gives $\widetilde C=2e^{-2}-1$, hence

$$
\boxed{y(x)=e^{2x}\left(x-1+2e^{-2}\right).}
$$

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
