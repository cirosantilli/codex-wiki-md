<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\mathbf t=(x_s,y_s)$ be the unit tangent of the [inextensible filament](../../../../../inextensible-filament.md). Define

$$
\rho=\frac{c_\parallel}{c_\perp},\qquad
\boxed{\beta=\frac1\Lambda\int_0^\Lambda x_s^2\,ds,\qquad
\delta=\frac1\Lambda\int_0^\Lambda x_sy_s\,ds.}
$$

These quantities are invariant under a shift of the periodic arclength coordinate. Since $x_s^2+y_s^2=1$, the average tangent tensor is $M=\left(\begin{smallmatrix}\beta&\delta\\\delta&1-\beta\end{smallmatrix}\right)$. Also $\int\mathbf t\,ds=\lambda\mathbf e_x$.

For [finite-amplitude propulsion of an inextensible periodic filament](../../../../../finite-amplitude-propulsion-of-an-inextensible-periodic-filament.md), distinguish axial phase speed from tangential material speed. The $V$ in the displayed formula is the axial speed of the travelling pattern relative to the mean filament motion. In the wave frame an inextensible material line slides backwards tangentially at the constant speed $Q=V\Lambda/\lambda$: its mean axial sliding is $Q\lambda/\Lambda=V$. If the filament translates at $-U\mathbf e_x$ in the laboratory, its local fluid-relative [velocity](../../../../../velocity.md) is

$$
\mathbf u=(V-U)\mathbf e_x-Q\mathbf t.
$$

This relation is the [axial and arclength travelling-wave speeds](../../../../../axial-and-arclength-travelling-wave-speeds.md) conversion. It ensures the arclength-averaged material [velocity](../../../../../velocity.md) is $-U\mathbf e_x$, rather than confusing wave propagation with material transport.

Integrating the [resistive-force theory](../../../../../resistive-force-theory.md) hydrodynamic [force](../../../../../force.md) over a period and imposing zero axial [force](../../../../../force.md) gives

$$
0=c_\perp\Lambda(V-U)[1+(\rho-1)\beta]-c_\parallel Q\lambda.
$$

Substitution of $Q\lambda=V\Lambda$ yields

$$
\boxed{\frac UV=\frac{(1-\rho)(1-\beta)}{1+\beta(\rho-1)}.}
$$

For $0<\rho<1$ and $\beta<1$ it is positive: anisotropic drag drives swimming opposite to the wave. A straight waveform has $\beta=1$ and gives no propulsion; isotropic drag $\rho=1$ also gives zero. The denominator $(1-\beta)+\rho\beta$ is positive. If instead $V$ denotes arclength propagation speed, the left-hand ratio acquires the extra factor $\lambda/\Lambda$; the two speeds are not interchangeable.

There is a geometric qualification to the asserted direction. For free swimming strictly along $x$, zero transverse [force](../../../../../force.md) also requires $\delta=0$, which holds for the usual reflection-symmetric waveforms. The periodicity assumptions alone do not imply that symmetry. A general waveform has [cross-resistance of an asymmetric planar waveform](../../../../../cross-resistance-of-an-asymmetric-planar-waveform.md) and can require a transverse translation. If the mean laboratory [velocity](../../../../../velocity.md) is $(-U_x,U_y)$, the full [force-free](../../../../../force-free.md) condition is

$$
[I+(\rho-1)M]\binom{V-U_x}{U_y}=\rho V\binom10.
$$

Writing $A_0=1+(\rho-1)\beta$, $B_0=1+(\rho-1)(1-\beta)$ and $\mathcal D=A_0B_0-(\rho-1)^2\delta^2$, one obtains

$$
\boxed{\frac{U_x}V=1-\frac{\rho B_0}{\mathcal D},\qquad
\frac{U_y}V=-\frac{\rho(\rho-1)\delta}{\mathcal D}.}
$$

The printed expression is recovered when $\delta=0$, or as the axial [force](../../../../../force.md)-balance result if transverse motion is externally constrained. For an explicit permitted asymmetric shape, concatenate tangents $(\sqrt3/2,1/2)$ and $(1/2,-\sqrt3/2)$ with arclength fractions $p=\sqrt3/(1+\sqrt3)$ and $1-p$. Their mean vertical tangent is zero, but $\delta=\sqrt3(2p-1)/4\ne0$. Repeating the segments gives a periodic graph; the corners can be smoothed without removing the nonzero cross integral. Thus **pure opposite-to-wave free swimming also needs a zero cross-resistance assumption**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
