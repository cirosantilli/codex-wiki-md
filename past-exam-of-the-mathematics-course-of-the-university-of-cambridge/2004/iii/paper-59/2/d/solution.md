<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each [Fourier mode](../../../../../../fourier-mode.md) the equation is $\Phi_k''+6\mathcal H\Phi_k'+k^2\Phi_k=0$. Set $\Phi_k=a^{-3}u_k$. Direct differentiation removes the first [derivative](../../../../../../derivative.md) and gives

$$
u_k''+\left[k^2-3\mathcal H'-9\mathcal H^2\right]u_k
=u_k''+\left[k^2-\frac3{4\tau^2}\right]u_k=0.
$$

For $|k\tau|\gg1$, the inverse-square term is negligible, and the positive incoming-frequency branch has $u_k\sim A_ke^{-ik\tau}$. Therefore

$$
\boxed{\Phi_k\sim A_ka^{-3}e^{-ik\tau}.}
$$

The momentum constraint then gives

$$
\delta\phi_k=\frac{2(\Phi_k'+\mathcal H\Phi_k)}{\phi_0'}
\sim\frac{2ikA_k}{C}\,a^{-1}e^{-ik\tau},
$$

where $\phi_0'=-C/a^2$. Thus the scalar perturbation has precisely the required $a^{-1}$ behavior. Conversely, the two constraints imply the potential equation in part (c); reconstructing $\delta\phi$ by the momentum constraint therefore satisfies the energy constraint too. This checks compatibility beyond simply comparing powers of $a$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
