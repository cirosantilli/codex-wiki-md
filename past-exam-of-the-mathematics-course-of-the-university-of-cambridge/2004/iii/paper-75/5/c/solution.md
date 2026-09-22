<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $W$ be the complex vertical [velocity](../../../../../../velocity.md) amplitude in $w=\operatorname{Re}\{W(z)e^{ikx}\}$. It satisfies $W''+m^2W=0$, with $W(0)=ikU\eta_0$ and $W(H)=0$. Away from [resonance](../../../../../../resonance.md), solve these two boundary conditions:

$$
\boxed{W(z)=ikU\eta_0\frac{\sin[m(H-z)]}{\sin(mH)}}.
$$

The resulting field is a standing vertical superposition of equal-amplitude upward and downward [internal gravity waves](../../../../../../internal-wave.md). Write $W=A_+e^{imz}+A_-e^{-imz}$. The rigid lid gives $A_-=-A_+e^{2imH}$, and the bed gives

$$
\boxed{A_+=\frac{ikU\eta_0}{1-e^{2imH}}=-\frac{kU\eta_0e^{-imH}}{2\sin(mH)},\qquad A_-=-A_+e^{2imH}}.
$$

The upward vertical-velocity amplitude is $|kU\eta_0|/[2|\sin(mH)|]$. For real positive $\eta_0$, its phase relative to the bed-height coefficient is $-mH+\pi$ if $\sin(mH)>0$ and $-mH$ if $\sin(mH)<0$, modulo $2\pi$. Relative to the imposed bed-velocity coefficient $ikU\eta_0$, the phase is instead $-mH+\pi/2$ in the positive-sine case, with an additional $\pi$ when the sine changes sign. The complex coefficient gives the answer without convention ambiguity. The upward displacement coefficient, if desired, is $A_+/(ikU)$, since $w=U\zeta_x$ for the stationary wave.

A reflecting lid reverses the vertical energy direction while retaining horizontal [wavenumber](../../../../../../wavenumber.md) and laboratory frequency. In the terrain frame the incident and reflected energy rays therefore travel downstream while zigzagging between the boundaries. The [velocity](../../../../../../velocity.md) field has nodes at the lid and a vertically standing pattern; the sketch marks this ray geometry, rather than falsely drawing the reflected ray as a specular optical ray.

The intrinsic [group velocity](../../../../../../group-velocity.md) makes an angle $\theta$ with vertical satisfying $\tan\theta=|c_{gx}^{\rm fluid}|/c_{gz}=m/k$. Consequently the denominator vanishes when

$$
\boxed{mH=kH\tan\theta=n\pi,\qquad n=1,2,\ldots}.
$$

These are the [rigid-lid resonance of stationary topographic internal waves](../../../../../../rigid-lid-resonance-of-stationary-topographic-internal-waves.md). At such a nonzero vertical mode the homogeneous rigid-lid eigenfunction is also zero at the bed, so it cannot satisfy the nonzero prescribed bed [velocity](../../../../../../velocity.md); a bounded stationary inviscid forced solution does not exist. Time-dependent forcing produces secular modal growth until dissipation or nonlinearity intervenes. The formal $n=0$, $m=0$ limit is not this resonance: $\sin[m(H-z)]/\sin(mH)\to(H-z)/H$ is finite. Propagating resonance also requires $k<N/U$; an evanescent field has no real standing-wave resonances of this kind.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
