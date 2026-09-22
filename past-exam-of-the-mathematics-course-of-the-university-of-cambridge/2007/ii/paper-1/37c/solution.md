<h1 id="37c/solution">Solution</h1>

↑ **Parent:** [37C](../37c.md)

Take [shear-horizontal waves](../../../../../shear-horizontal-wave.md) with displacement $\boldsymbol u=(0,0,w(x,y,t))$. This is divergence-free, so the elastic equation reduces to $\rho w_{tt}=\mu(w_{xx}+w_{yy})$. Rigid boundaries require $w=0$ at $y=0,h$, giving modes $w=A\sin(n\pi y/h)\cos(kx-\omega t)$, $n\ge1$. With shear speed $c_s=\sqrt{\mu/\rho}$, the [dispersion relation](../../../../../dispersion-relation.md) is

$$
\boxed{\omega^2=c_s^2\left(k^2+\frac{n^2\pi^2}{h^2}\right),\qquad \omega_{c,n}=\frac{n\pi c_s}{h}.}
$$

For $k>0$, the [phase velocity](../../../../../phase-velocity.md) is $v_p=\omega/k>c_s$ and the [group velocity](../../../../../group-velocity.md) is $v_g=d\omega/dk=c_s^2k/\omega<c_s$, with $v_pv_g=c_s^2$.

The [kinetic energy density](../../../../../kinetic-energy-density.md) is $T=\rho w_t^2/2$. The only strains are $e_{xz}=w_x/2$ and $e_{yz}=w_y/2$, together with their symmetric counterparts; thus the [isotropic linear-elastic energy density](../../../../../isotropic-linear-elastic-energy-density.md) is $W=\mu(w_x^2+w_y^2)/2$. Average over one temporal period and integrate across the layer. The sine- and cosine-squared transverse integrals are both $h/2$, giving

$$
\boxed{\left\langle\int_0^hT\,dy\right\rangle=\frac{\rho A^2\omega^2h}{8}
=\frac{\mu A^2h}{8}\left(k^2+\frac{n^2\pi^2}{h^2}\right)
=\left\langle\int_0^hW\,dy\right\rangle.}
$$

The [guided shear-horizontal mode](../../../../../guided-shear-horizontal-mode.md) has average equipartition after both operations; a time average at a fixed transverse point alone need not give equality.

## ↑ Ancestors (10)

1. [37C](../37c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
