<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) pair $\widehat q(k)=\int q(x)e^{ikx}dx$, $q(x)=(2\pi)^{-1}\int\widehat q(k)e^{-ikx}dk$. The point [force](../../../../../../force.md) transforms to $F$. With the [dispersion relation](../../../../../../dispersion-relation.md) $D$ defined above, the sheet equation becomes

$$
D(k,\omega)\widehat\eta(k)=F,\qquad
\widehat p_+(k,y)=-\frac{F\rho_0\omega^2e^{-\gamma y}}{\gamma(Tk^2-m\omega^2)-2\rho_0\omega^2}.
$$

The [point-force radiation from a fluid-loaded sheet](../../../../../../point-force-radiation-from-a-fluid-loaded-sheet.md) is therefore represented exactly by

$$
\rho'(x,y,t)=-\frac{F\rho_0\omega^2}{2\pi c_0^2}e^{i\omega t}
\int_C\frac{e^{-ikx-\gamma y}}{\gamma(Tk^2-m\omega^2)-2\rho_0\omega^2}\,dk.
$$

The causal contour and [outgoing acoustic square-root branch](../../../../../../outgoing-acoustic-square-root-branch.md) are fixed first with $\operatorname{Im}\omega<0$, then continued to the desired real frequency. This prescription fixes how poles and the branch points are passed.

For the [acoustic far field](../../../../../../acoustic-far-field.md) $x=r\cos\theta$, $y=r\sin\theta$, take $0<\theta<\pi$ bounded away from grazing and $k_0r\gg1$. The [method of steepest descent](../../../../../../method-of-steepest-descent.md) [saddle point](../../../../../../saddle-point.md) is $k_s=k_0\cos\theta$, with $\gamma_s=ik_0\sin\theta$. The supplied [saddle point](../../../../../../saddle-point.md) rule, including its $\sin\theta$ factor, gives, provided the [contour deformation](../../../../../../contour-deformation.md) crosses no poles,

$$
\rho'\sim-\sqrt{\frac{k_0}{2\pi r}}\,
\frac{F\rho_0\omega^2\sin\theta\,e^{i\omega(t-r/c_0)+i\pi/4}}
{c_0^2\left[ik_0\sin\theta\,(Tk_0^2\cos^2\theta-m\omega^2)-2\rho_0\omega^2\right]}.
$$

A convenient simplification, free of division by $T$, is

$$
\boxed{\rho'\sim-\sqrt{\frac{\omega}{2\pi c_0r}}\,
\frac{F\rho_0\sin\theta\,e^{i\omega(t-r/c_0)+i\pi/4}}
{c_0^2\left[ik_0\sin\theta\,(T\cos^2\theta/c_0^2-m)-2\rho_0\right]}.}
$$

Equivalently, when $T\ne0$,

$$
\rho'\sim-\sqrt{\frac{\omega}{2\pi r}}\,
\frac{F\rho_0c_0^{-3/2}\sin\theta\,e^{i\omega(t-r/c_0)+i\pi/4}}
{(\cos^2\theta-mc_0^2/T)i\omega(T/c_0^2)\sin\theta-2\rho_0c_0}.
$$

**The expression printed in the PDF is missing sound-speed factors for general dimensional $c_0$.** It agrees with this result if $c_0=1$ in fully normalized units; when $c_0$ is retained as an arbitrary [sound speed](../../../../../../speed-of-sound.md), the numerator needs $c_0^{-3/2}$ and the structural term needs $T/c_0^2$ in the last form. These factors arise respectively from cylindrical spreading, the pressure-density relation, and $k_s=\omega\cos\theta/c_0$.

A direct countercheck is the transparent-sheet limit $m=T=0$. The sheet jump condition then gives $\widehat p_+(k,0)=F/2$, so the [saddle point](../../../../../../saddle-point.md) rule requires

$$
\boxed{\rho'\sim\frac{F}{2c_0^2}\sqrt{\frac{\omega}{2\pi c_0r}}\sin\theta\,
 e^{i\omega(t-r/c_0)+i\pi/4}.}
$$

The printed expression, interpreted continuously after multiplying out its structural factor, instead gives $F(2c_0)^{-1}\sqrt{\omega/(2\pi r)}\sin\theta$ times the same phase. It differs by a factor $c_0^{3/2}$; for example it is eight times too large when $c_0=4$. This limit also verifies the normalization of the corrected density field independently of the sheet's [elastic-sheet tension](../../../../../../elastic-sheet-tension.md).

To decide about poles, track the roots of $\Delta(k,\omega)$ on the chosen square-root sheet and deform the original causal contour to the [steepest descent contour](../../../../../../steepest-descent-contour.md). A root contributes a residue exactly when it lies in the region swept out by that deformation; its sign is fixed by the contour orientation. Branch cuts must be retained throughout this comparison. Which roots are crossed can depend on observation angle, producing a change of the modal contribution when a pole meets the deformation boundary. A [saddle point](../../../../../../saddle-point.md) approaching a pole or a grazing endpoint requires an approximation uniform in that limit, rather than the isolated [saddle point](../../../../../../saddle-point.md) formula above.

The crossed poles are the free fluid-sheet modes of the preceding solution. Real subsonic roots represent [evanescent acoustic surface waves](../../../../../../evanescent-acoustic-surface-wave.md) carrying energy along the sheet, with normal decay; complex continuations represent leaky or radiating modes. Their residues must be added to the [saddle point](../../../../../../saddle-point.md) sound when the causal contour selects them. The specification “no poles contribute” is therefore a substantive condition on the contour, not permission to ignore zeros of the [dispersion relation](../../../../../../dispersion-relation.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
