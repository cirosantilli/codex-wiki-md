# Oscillating-wall forcing of a rectangular tank

↑ **Parent:** [Normal modes of surface gravity waves in a rectangular tank](normal-modes-of-surface-gravity-waves-in-a-rectangular-tank.md)

For a tank $0<x<L$, $-h<z<0$, let the left wall move by $\operatorname{Re}(ce^{-i\omega t})$ with small [amplitude](wave-amplitude.md), while the right wall and bottom remain fixed. A periodic [velocity potential](velocity-potential.md) $\operatorname{Re}(f e^{-i\omega t})$ has $f_x(0,z)=-i\omega c$. Add the [harmonic function](harmonic-function.md)

$$
Q(x,z)=\frac{i\omega c}{2L}[(z+h)^2-(L-x)^2]
$$

to obtain $G=f+Q$ with homogeneous wall and bottom [Neumann boundary conditions](neumann-boundary-condition.md). Thus $G=a_0/2+\sum_{n\geq1}a_n\cos(k_nx)\cosh(k_n(z+h))$, where $k_n=n\pi/L$. The [linearized free-surface boundary conditions](linearized-free-surface-boundary-conditions.md) give $G_z-\lambda G=H$ at $z=0$, with $\lambda=\omega^2/g$ and

$$
H(x)=\frac{i\omega c}{L}\left[h-\frac\lambda2(h^2-(L-x)^2)\right].
$$

Its [Fourier cosine coefficients](fourier-cosine-coefficient.md) $H_n=(2/L)\int_0^L H(x)\cos(k_nx)dx$ give the title expression for $n\geq1$ and $a_0=-H_0/\lambda$. In particular $H_n=2i\omega c\lambda/(Lk_n^2)$ for $n\geq1$. The denominator vanishes at the corresponding [normal modes of surface gravity waves in a rectangular tank](normal-modes-of-surface-gravity-waves-in-a-rectangular-tank.md), giving [resonance](resonance.md). Exact undamped resonance produces secular growth instead of a bounded periodic response. Free transients do not generally decay in this inviscid model.

## ↑ Ancestors (7)

1. [Normal modes of surface gravity waves in a rectangular tank](normal-modes-of-surface-gravity-waves-in-a-rectangular-tank.md)
2. [Surface gravity wave](surface-gravity-wave.md)
3. [Free surface](free-surface.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Normal modes of surface gravity waves in a rectangular tank](normal-modes-of-surface-gravity-waves-in-a-rectangular-tank.md)
- [Solution](past-exam-of-the-waves-and-compressible-flow-course-of-the-university-of-oxford/2023/1/b/ii/solution.md)
