<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $g=V_0$ for the effective coupling and keep $N$ for the number obtained by the stated two-dimensional normalization. A repulsive interaction, $g>0$, permits the [Thomas–Fermi approximation for a condensate](../../../../../../thomas-fermi-approximation-for-a-condensate.md): density-gradient [kinetic energy](../../../../../../kinetic-energy.md) is small compared with the trapping and interaction terms over most of the cloud. The stationary [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) then gives

$$
\boxed{\psi(\mathbf x,t)\simeq e^{-i\mu t/\hbar}\sqrt{n_{\rm TF}(r)},\qquad
n_{\rm TF}(r)=\frac{\mu-\tfrac12m\omega^2r^2}{g}\quad(0\le r<R)}
$$

and $n_{\rm TF}=0$ outside the cloud, up to the narrow edge region. Here

$$
R^2=\frac{2\mu}{m\omega^2},\qquad n_c=\frac\mu g.
$$

Normalize the parabolic [number density](../../../../../../number-density.md) directly:

$$
N=\frac{2\pi}{g}\int_0^R\left(\mu-\frac12m\omega^2r^2\right)r\,dr
=\frac{\pi\mu^2}{gm\omega^2}=\frac{\pi n_cR^2}{2}.
$$

Consequently the [two-dimensional Thomas–Fermi condensate](../../../../../../two-dimensional-thomas-fermi-condensate.md) parameters are

$$
\boxed{\mu=\sqrt{\frac{Ngm\omega^2}{\pi}},\qquad
R=\sqrt{\frac{2\mu}{m\omega^2}},\qquad n_c=\frac\mu g}.
$$

With $a_{\rm ho}=\sqrt{\hbar/(m\omega)}$ and central [healing length](../../../../../../healing-length.md) $\xi=\hbar/\sqrt{2m\mu}$, the bulk approximation requires

$$
\boxed{\mu\gg\hbar\omega\quad\Longleftrightarrow\quad
\frac{Ngm}{\pi\hbar^2}\gg1}.
$$

Indeed $R/\xi=2\mu/(\hbar\omega)\gg1$. In the coupling convention printed in the paper, formal substitution of $g=4\pi\hbar^2a/m$ gives

$$
\boxed{\mu=2\hbar\omega\sqrt{Na},\qquad
R=2a_{\rm ho}(Na)^{1/4},\qquad Na\gg1}.
$$

This is the requested relationship in that convention; $\omega$ sets the physical size and [chemical potential](../../../../../../chemical-potential.md), while the interaction-strength ratio to $\hbar\omega$ is independent of $\omega$.

There is a dimensional convention to make explicit. A physical three-dimensional [scattering length](../../../../../../scattering-length-from-a-partial-wave-s-matrix.md) $a$ makes $4\pi\hbar^2a/m$ a three-dimensional contact coupling, whereas a genuinely two-dimensional particle-number normalization requires coupling units of energy times area. For an axial factor $\chi(z)$ normalized to one, the [effective two-dimensional contact coupling](../../../../../../effective-two-dimensional-contact-coupling.md) is $g_{2D}=(4\pi\hbar^2a/m)\int|\chi|^4dz$. For a Gaussian of width $a_z$ this is $4\pi\hbar^2a/(m\sqrt{2\pi}a_z)$, and the physical TF condition becomes $Na/a_z\gg1$ up to numerical constants. Alternatively the printed coupling can be retained if $N$ is a line density. The paper supplies no axial scale, so its $Na$ expressions require that effective-unit or line-density convention; the formulas in terms of $g$ above are unambiguous. The approximation fails inside vortex cores and at the cloud edge, and it is not a repulsive TF ground-state construction for $g\le0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
