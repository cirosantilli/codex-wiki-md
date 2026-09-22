<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use dimensionless variables throughout this calculation and write $c$ for $\tilde c$. Take $k>0$ without loss of generality, so $\alpha=kh/2>0$; for the opposite Fourier orientation the decay rate is $|k|h/2$. The density profile printed alongside the velocity profile is $\tilde\rho=-1$ above, $0$ in the middle, and $+1$ below. It is absent from the TeX transcription but essential to the interface calculation.

The nondimensional [jump conditions for stratified inviscid shear flow](../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) also follow directly from the stated scales. Divide the dimensional stress bracket by $\Delta U/h$ times the [streamfunction](../../../../../stream-function.md) scale. The density contrast supplies $J\tilde\rho\,\tilde\psi/(\tilde U-c)$. The term from the constant reference density is proportional to $\tilde\psi/(\tilde U-c)$ and drops out of its jump because the first condition makes this ratio continuous. This explains why only the density contrast remains.

For a vertically localized disturbance, take decaying exterior solutions and set $P=\tilde\psi(1)$, $Q=\tilde\psi(-1)$. The velocity is continuous at the interfaces, so the first jump condition gives continuity of $\tilde\psi$. The outer solutions are $Pe^{-\alpha(\tilde z-1)}$ above and $Qe^{\alpha(\tilde z+1)}$ below. In the middle the [endpoint derivative map for an evanescent wave layer](../../../../../endpoint-derivative-map-for-an-evanescent-wave-layer.md) gives

$$
\tilde\psi'(1^-)=\alpha[\coth(2\alpha)P-\operatorname{csch}(2\alpha)Q],\qquad
\tilde\psi'(-1^+)=\alpha[\operatorname{csch}(2\alpha)P-\coth(2\alpha)Q].
$$

These expressions follow by fitting a linear combination of $\cosh(\alpha\tilde z)$ and $\sinh(\alpha\tilde z)$ to its two endpoint values.

At the upper interface the shear drops from one to zero and the density drops from zero to minus one. At the lower interface they change from zero to one and from one to zero. Substitute those jumps, including the exterior derivatives $-\alpha P$ and $+\alpha Q$. Define

$$
a=\alpha[1+\coth(2\alpha)],\qquad b=\alpha\operatorname{csch}(2\alpha).
$$

Multiplication by the respective nonzero $U-c$ gives the homogeneous system

$$
\begin{pmatrix}
a(1-c)^2-(1-c)-J&-b(1-c)^2\\
-b(1+c)^2&a(1+c)^2-(1+c)-J
\end{pmatrix}
\begin{pmatrix}P\\Q\end{pmatrix}=0.
$$

For growing modes $\operatorname{Im}c>0$ the denominators cannot vanish. Neutral limiting values are interpreted by continuation of the matching calculation.

A nonzero disturbance requires the determinant to vanish. Put $T=1+J$, $\varepsilon=e^{-2\alpha}$ and $d=a^2-b^2=2\alpha a$, with $a=2\alpha/(1-\varepsilon^2)$ and $b=a\varepsilon$. The determinant is

$$
(a c^2+a-T)^2-(2a-1)^2c^2-b^2(1-c^2)^2=0.
$$

Dividing by $d$ and collecting powers proves the [quartic dispersion relation for a three-layer stratified shear flow](../../../../../quartic-dispersion-relation-for-a-three-layer-stratified-shear-flow.md):

$$
\boxed{c^4+Pc^2+Q_0=0,}
$$

where

$$
P=\frac{e^{-4\alpha}-(2\alpha-1)^2}{4\alpha^2}-1-\frac{J}{\alpha},\qquad
Q_0=\frac{[2\alpha-(1+J)]^2-e^{-4\alpha}(1+J)^2}{4\alpha^2}.
$$

Here $P$ as a polynomial coefficient is distinct from the endpoint amplitude used above. The result is the desired dispersion equation, derived from both shear and density jumps rather than a density-only matching rule.

Treat this as a quadratic in $X=c^2$. Whenever $Q_0<0$, its two roots are real with opposite signs: the discriminant $P^2-4Q_0$ is strictly positive and their product is negative. The negative root gives $c=+i\sqrt{-X}$, which grows under the convention $e^{ik(x-ct)}$. Factor the constant term:

$$
4\alpha^2Q_0=[2\alpha-T(1+\varepsilon)][2\alpha-T(1-\varepsilon)].
$$

The [unstable band of a three-layer stratified shear flow](../../../../../unstable-band-of-a-three-layer-stratified-shear-flow.md) follows immediately:

$$
\boxed{\frac{2\alpha}{1+e^{-2\alpha}}<1+J<\frac{2\alpha}{1-e^{-2\alpha}},}
$$

or equivalently $\alpha e^\alpha/\cosh\alpha<1+J<\alpha e^\alpha/\sinh\alpha$. The endpoints are neutral $c=0$ limits of this growing branch.

For large $\alpha$, the overlap of the two interface disturbances is exponentially small: $b\simeq2\alpha e^{-2\alpha}$. Dropping this coupling leaves the two independent [gravity-vorticity interface waves](../../../../../gravity-vorticity-interface-wave.md). Their relevant laboratory phase speeds are

$$
c_+=1-\frac{1+\sqrt{1+8\alpha J}}{4\alpha},\qquad
c_-=-1+\frac{1+\sqrt{1+8\alpha J}}{4\alpha}=-c_+.
$$

The upper wave propagates backward relative to its current and the lower wave forward relative to its current. They share a stationary laboratory phase when $J=2\alpha-1$. Restoring their small evanescent coupling produces [counterpropagating wave resonance in a three-layer shear flow](../../../../../counterpropagating-wave-resonance-in-a-three-layer-shear-flow.md), with the unstable interval

$$
1+J=2\alpha+O(\alpha e^{-2\alpha}).
$$

Near this resonance, the waves lock in phase and extract energy from the mean shear. At large wavenumber the resonance band is exponentially narrow; large wavenumber by itself does not make an arbitrary fixed-$J$ profile unstable.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
