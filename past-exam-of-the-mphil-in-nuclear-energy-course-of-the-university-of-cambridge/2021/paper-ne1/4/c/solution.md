<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [neutron fluence](../../../../../neutron-fluence.md) $\Phi$ as the independent variable and abbreviate $a=\sigma_{a\rm Th}$, $b=\sigma_{a\rm U}$ and $c=\sigma_{c\rm Th}$. Substituting the parent solution into the second [linear differential equation](../../../../../linear-differential-equation.md) gives

$$
\frac{dN_{\rm U}}{d\Phi}+bN_{\rm U}=cN_{\rm Th0}e^{-a\Phi}.
$$

The [integrating factor](../../../../../integrating-factor.md) is $e^{b\Phi}$. Integrating from the initial state yields

$$
\boxed{N_{\rm U}(\Phi)=N_{\rm U0}e^{-b\Phi}+\frac{cN_{\rm Th0}}{b-a}\left(e^{-a\Phi}-e^{-b\Phi}\right),\qquad b\ne a.}
$$

The first term is survival of the initial population; the second accumulates production at earlier exposures, weighted by subsequent survival. For $b=a$, the continuous [limit](../../../../../limit-of-a-function.md) is $(N_{\rm U0}+cN_{\rm Th0}\Phi)e^{-a\Phi}$. The same formula applies to a time-varying prescribed flux through $\Phi(t)$; intervals of zero flux leave both populations unchanged.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [4](../../4.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
