<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [turbulent Schmidt number](../../../../../../turbulent-schmidt-number.md) compares turbulent momentum and concentration diffusivities:

$$
\boxed{\mathrm{Sc}_T=\frac{\nu_T}{\kappa_T}=2.}
$$

The mean fluid has no vertical [velocity](../../../../../../velocity.md). Taking $z$ positive upward and $W_s>0$, the settling flux is $-W_s\phi$, while the given turbulent particle flux is $-\kappa_T\phi_z$. Local particle-volume conservation therefore gives

$$
\phi_t+\partial_zJ=0,\qquad J=-W_s\phi-\kappa_T\phi_z.
$$

Consequently the evolution equation is

$$
\boxed{\phi_t=\partial_z\left(W_s\phi+\kappa_T\phi_z\right).}
$$

For constant settling speed this is $\phi_t=W_s\phi_z+\partial_z(\kappa_T\phi_z)$. In the logarithmic region, $\kappa_T=Cz/2$ from the preceding part. The sign is consistent with downward settling: without diffusion, a profile evolves as $\phi(z,t)=\phi(z+W_st,0)$. The dilute suspension approximation neglects feedback on the mean flow and particle interactions; deposition or erosion must be imposed through the bed boundary flux.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
