<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A uniform [spatial translation](../../../../../../spatial-translation.md) of the rolls changes $\phi$ by a constant, so a local [phase modulation](../../../../../../phase-modulation.md) equation cannot depend on $\phi$ itself. Reflection across the transverse axis acts as $Y\mapsto-Y$; reflection across the roll coordinate acts as $\phi\mapsto-\phi$, after choosing a reflection-symmetric roll profile. The right-hand side must therefore be odd in $\phi$ and even under $Y$ reflection.

At the lowest orders, $\phi_{YY}$ and $\phi_{YYYY}$ have these symmetries. The terms $\phi_Y^2$, $\phi_Y\phi_{YYY}$ and $\phi_{YY}^2$ are even in $\phi$ and are forbidden; $\phi_Y^3$ is odd under $Y$ reflection and is forbidden. The first nonlinear derivative term at this order is $\phi_Y^2\phi_{YY}$. Near the transverse threshold use the [quartic-time transverse phase scaling](../../../../../../quartic-time-transverse-phase-scaling.md): the small coefficient of $\phi_{YY}$, the fourth derivative and this cubic term have the same asymptotic order. This gives

$$
\boxed{\phi_T=\lambda\phi_{YY}-\gamma\phi_{YYYY}-\alpha\phi_Y^2\phi_{YY}.}
$$

The symmetry arguments determine the allowed terms, not their coefficients. A well-posed short-wave regularization requires $\gamma>0$. The [zigzag instability](../../../../../../zigzag-instability.md) occurs for $\lambda<0$, since a [Fourier mode](../../../../../../fourier-mode.md) grows at $-\lambda k^2-\gamma k^4$. With $p=\phi_Y$, differentiating gives

$$
p_T=\partial_Y^2\left(\lambda p-\gamma p_{YY}-\frac\alpha3p^3\right).
$$

For $\lambda,\alpha<0$ the preferred uniform slopes satisfy $p^2=3\lambda/\alpha$; their slope diffusion coefficient is $\lambda-\alpha p^2=-2\lambda>0$. This identifies how the leading nonlinear term can saturate the [zigzag instability](../../../../../../zigzag-instability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
