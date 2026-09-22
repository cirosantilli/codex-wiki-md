<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $d=\psi_1-\psi_2$ and $C=f_0^2/g'=H_1F_1=H_2F_2$. Multiply each [two-layer quasi-geostrophic potential vorticity](../../../../../../two-layer-quasi-geostrophic-potential-vorticity.md) equation by $H_i\psi_i$ and sum. The time-derivative terms are

$$
\sum_iH_i\psi_iq_{it}
=\nabla_h\cdot\sum_iH_i\psi_i\nabla_h\psi_{it}
-\partial_t\left[\frac12\sum_iH_i|\nabla_h\psi_i|^2+\frac C2d^2\right].
$$

The interface terms combine to $-Cd\,d_t$, since the two layers share the same depth-weighted coupling $H_iF_i$. The planetary term $\beta y$ has no time derivative. For the nonlinear terms, $\nabla_h\cdot\mathbf u_i=0$ and $\mathbf u_i\cdot\nabla_h\psi_i=0$ imply

$$
H_i\psi_iJ(\psi_i,q_i)=\nabla_h\cdot(H_i\psi_iq_i\mathbf u_i).
$$

Consequently the local [two-layer quasi-geostrophic energy conservation](../../../../../../two-layer-quasi-geostrophic-energy-conservation.md) law is

$$
\boxed{\partial_tE+\nabla_h\cdot\mathbf F_E=0,\qquad
E=\frac12\left[H_1|\nabla_h\psi_1|^2+H_2|\nabla_h\psi_2|^2+C(\psi_1-\psi_2)^2\right],}
$$



$$
\boxed{\mathbf F_E=-\sum_{i=1}^2H_i\left(\psi_i\nabla_h\psi_{it}+\psi_iq_i\mathbf u_i\right).}
$$

The flux expression is one convenient form obtained directly from the requested multiplication; divergence-free modifications would represent the same local balance. $E$ is physical energy per horizontal area divided by the common reference density. Multiplying both $E$ and $\mathbf F_E$ by that density restores the dimensional physical-energy convention.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
