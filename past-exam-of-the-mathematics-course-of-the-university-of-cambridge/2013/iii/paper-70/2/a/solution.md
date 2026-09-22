<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the prescribed harmonic convention $e^{i\omega t}$. For a propagating [acoustic plane wave](../../../../../../acoustic-plane-wave.md), let $k=(\omega/c_0)\cos\theta$ and $\ell=(\omega/c_0)\sin\theta>0$. The incident and reflected [pressure](../../../../../../pressure.md) amplitudes in the upper half-space have vertical factors $e^{i\ell y}$ and $e^{-i\ell y}$ respectively:

$$
p'=e^{i\omega t-ikx}\left(Ae^{i\ell y}+Re^{-i\ell y}\right).
$$

The [linear homentropic acoustic equations](../../../../../../linear-homentropic-acoustic-equations.md) imply $i\omega\rho_0v_y=-\partial_y p'$. At the surface, the [normal velocity](../../../../../../normal-velocity.md) is therefore $\ell(R-A)/(\rho_0\omega)=-V$, while the [pressure](../../../../../../pressure.md) amplitude is $P=A+R$. The [surface acoustic impedance](../../../../../../surface-acoustic-impedance.md) condition $P=ZV$ gives

$$
\boxed{\frac{A+R}{A-R}=\frac{Z\sin\theta}{\rho_0c_0},\qquad
\frac RA=\frac{Z-Z_f}{Z+Z_f},\quad Z_f=\frac{\rho_0c_0}{\sin\theta}.}
$$

Here $Z_f$ is the [normal acoustic impedance](../../../../../../normal-acoustic-impedance.md); the angle in this question is measured from the horizontal, not the normal. For a [passive acoustic impedance](../../../../../../passive-acoustic-impedance.md), the mean power absorbed per unit area is $\tfrac12\operatorname{Re}(PV^*)=\tfrac12\operatorname{Re}Z\,|V|^2\geq0$. The four limiting cases have distinct meanings:

- If $Z\to0$, $R=-A$. This is a [pressure-release boundary](../../../../../../pressure-release-boundary.md): the [pressure](../../../../../../pressure.md) perturbation vanishes, while the [normal velocity](../../../../../../normal-velocity.md) is generally nonzero. The reflected [pressure](../../../../../../pressure.md) has equal amplitude and a phase reversal.
- If $Z\to\infty$, $R=A$. The boundary is [acoustically rigid](../../../../../../acoustically-rigid-boundary.md), with zero [normal velocity](../../../../../../normal-velocity.md) and doubled total surface [pressure](../../../../../../pressure.md). There is no [pressure](../../../../../../pressure.md) phase reversal.
- If $R/A\to0$, $Z\to Z_f$. This is a matched boundary, taking up the incoming wave without reflection. Its [pressure](../../../../../../pressure.md) and [normal velocity](../../../../../../normal-velocity.md) are those of the incident wave.
- Formally, $R/A\to\infty$ means $Z\to-Z_f$. A nonzero outgoing field can then exist with vanishing incoming amplitude. For a passive boundary at a real propagating incidence angle, a negative-real-part [surface acoustic impedance](../../../../../../surface-acoustic-impedance.md) cannot describe ordinary absorption: such a scattering pole must be interpreted through an active source or an continued by [analytic continuation](../../../../../../analytic-continuation.md) free-mode resonance. The sheet calculation below identifies the relevant free modes.

## ↑ Ancestors (11)

1. [A](../a.md)
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
