<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0<\Omega<1$, choose the [Big Bang](../../../../../../big-bang.md) to occur at $\tau=t=0$ and retain the expanding solution. The first integral found above is

$$
a'^2=H_0^2(\Omega a+ba^2).
$$

Use $a=(\Omega/b)\sinh^2u$. Substitution gives $u'=H_0\sqrt b/2=\alpha/2$, so $u=\alpha\tau/2$. This gives the [flat matter-coasting-fluid Friedmann solution](../../../../../../flat-matter-coasting-fluid-friedmann-solution.md):

$$
\boxed{a(\tau)=\frac{\Omega}{b}\sinh^2\frac{\alpha\tau}{2}=\frac{\Omega}{2b}\,[\cosh(\alpha\tau)-1].}
$$

Integrate $dt/d\tau=a$, with the same zero of time:

$$
\boxed{t(\tau)=\frac{\Omega}{2b\alpha}[\sinh(\alpha\tau)-\alpha\tau]=\frac{H_0^{-1}\Omega}{2b^{3/2}}[\sinh(\alpha\tau)-\alpha\tau].}
$$

As a check, $a'=(\Omega\alpha/2b)\sinh(\alpha\tau)$, and the identity $\sinh^2v=(\cosh v-1)(\cosh v+1)$ verifies $a'^2=H_0^2(\Omega a+ba^2)$. Also $t'=a$ exactly. At early times $a\simeq\Omega H_0^2\tau^2/4$ and $t\simeq\Omega H_0^2\tau^3/12$, reproducing the matter-dominated relation $a\propto t^{2/3}$.

The endpoint $\Omega=1$ is obtained by taking the smooth limit: $a=H_0^2\tau^2/4$ and $t=H_0^2\tau^3/12$. At $\Omega=0$ the [coasting cosmic-string universe](../../../../../../coasting-cosmic-string-universe.md) instead has $a=H_0t$ and $\mathcal H=H_0$. Its [Big Bang](../../../../../../big-bang.md) is at $\tau=-\infty$, so a finite conformal-time origin at the bang is no longer available; choosing $a=1$ at $\tau=0$ gives $a=e^{H_0\tau}$ and $t=H_0^{-1}e^{H_0\tau}$. The physical-age limit remains regular.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
