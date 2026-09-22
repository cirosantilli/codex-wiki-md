<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Integrating the local [two-layer quasi-geostrophic energy conservation](../../../../../../two-layer-quasi-geostrophic-energy-conservation.md) law over a horizontal domain and using the specified vanishing boundary flux gives

$$
\boxed{\frac{d}{dt}\iint QE\,dx\,dy=0,\qquad
QE=\frac12\left[H_1|\nabla_h\psi_1|^2+H_2|\nabla_h\psi_2|^2+
\frac{f_0^2}{g'}(\psi_1-\psi_2)^2\right].}
$$

Periodic boundaries, or suitable fixed [streamfunction](../../../../../../stream-function.md) boundary data eliminating the displayed energy flux, provide examples. The gradient terms are the two layer kinetic energies; the last term is [available potential energy](../../../../../../available-potential-energy.md), equal to $g'\chi^2/2$ under the interface-displacement relation.

The [baroclinic energy ratio and deformation scale](../../../../../../baroclinic-energy-ratio-and-deformation-scale.md) for unequal layer depths uses a decomposition uses the depth-weighted barotropic [streamfunction](../../../../../../stream-function.md) $\Psi=(H_1\psi_1+H_2\psi_2)/(H_1+H_2)$ and $d=2\tilde\psi$. Define $H_r=H_1H_2/(H_1+H_2)$. Then

$$
K=\frac{H_1+H_2}{2}|\nabla_h\Psi|^2+\frac{H_r}{2}|\nabla_hd|^2,
\qquad K_{\rm bc}=2H_r|\nabla_h\tilde\psi|^2,\qquad
A=2\frac{f_0^2}{g'}\tilde\psi^2.
$$

For variations on horizontal scale $l$, this gives

$$
\boxed{\frac{A}{K_{\rm bc}}\sim\frac{l^2f_0^2}{g'H_r}=\left(\frac l{R_d}\right)^2,\qquad
R_d^2=\frac{g'H_1H_2}{f_0^2(H_1+H_2)}.}
$$

For comparable layer depths $H_r$ is of order either $H_i$, reproducing the requested scale $l^2f_0^2/(g'H_i)$. If one layer is much thinner, its depth controls this ratio; a depth-independent arithmetic barotropic average would leave unwanted cross terms in the energy decomposition.

**Baroclinic [potential energy](../../../../../../potential-energy.md) dominates at scales much larger than the [two-layer internal deformation radius](../../../../../../two-layer-internal-deformation-radius.md); baroclinic [kinetic energy](../../../../../../kinetic-energy.md) dominates at much smaller scales.** They are comparable near $l\sim R_d$. The independent barotropic [kinetic energy](../../../../../../kinetic-energy.md) has no interface-displacement partner, so this scale comparison refers specifically to the baroclinic component.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
