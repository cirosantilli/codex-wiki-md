<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Define

$$
I_{jk}=\int \rho x_jx_k\,d^3x.
$$

Using mass conservation to differentiate a material moment gives

$$
\dot I_{jk}=\int\rho(x_j\langle v_k\rangle+x_k\langle v_j\rangle)\,d^3x.
$$

Multiply the [Jeans equation](../../../../../jeans-equation.md) for component $j$ by $x_k$, integrate over space, discard the surface term of an isolated system, and symmetrize in $j,k$. The result is

$$
\frac12\ddot I_{jk}
=\int\rho\langle v_jv_k\rangle\,d^3x
-\frac12\int\rho\left(x_k\Phi_{,j}+x_j\Phi_{,k}\right)d^3x.
$$

Decompose $\langle v_jv_k\rangle=\bar v_j\bar v_k+\sigma_{jk}^2$ and define

$$
T_{jk}=\frac12\int\rho\bar v_j\bar v_k\,d^3x,\qquad
\Pi_{jk}=\int\rho\sigma_{jk}^2\,d^3x,
$$



$$
W_{jk}=-\frac12\int\rho\left(x_k\Phi_{,j}+x_j\Phi_{,k}\right)d^3x.
$$

This proves the [tensor virial theorem](../../../../../tensor-virial-theorem.md)

$$
\boxed{\frac12\ddot I_{jk}=2T_{jk}+\Pi_{jk}+W_{jk}}.
$$

For a steady oblate system rotating about $z$, $T_{zz}=0$, while symmetry gives $T_{xx}=T_{yy}$. The $zz$ and $xx$ equations are

$$
\Pi_{zz}+W_{zz}=0,\qquad 2T_{xx}+\Pi_{xx}+W_{xx}=0.
$$

Using $\Pi_{zz}=(1-\delta)\Pi_{xx}$, $2T_{xx}=Mv_0^2$, and $\Pi_{xx}=M\sigma_0^2$ gives

$$
\boxed{\frac{v_0^2}{\sigma_0^2}=(1-\delta)\frac{W_{xx}}{W_{zz}}-1}.
$$

With $W_{xx}/W_{zz}\simeq(1-\epsilon)^{-0.9}$, the edge-on curves are

$$
\boxed{\frac{v_0}{\sigma_0}
=\left[(1-\delta)(1-\epsilon)^{-0.9}-1\right]^{1/2}},
\qquad
\delta=0,0.1,0.2,0.3.
$$

At fixed ellipticity, increasing anisotropy lowers $v_0/\sigma_0$; the curve starts only once $(1-\epsilon)^{-0.9}\geq(1-\delta)^{-1}$. The $\delta=0$ line is the [oblate isotropic rotator](../../../../../oblate-isotropic-rotator.md) reference.

At inclination $i<90^\circ$, line-of-sight rotation is reduced approximately by $\sin i$, and the projected ellipticity also decreases as the spheroid is viewed closer to its symmetry axis. A galaxy therefore moves down and left from its edge-on location, with the exact track set by intrinsic thickness and anisotropy.

Low-mass [elliptical galaxies](../../../../../elliptical-galaxy.md) mostly occupy the fast-rotating, flattened, nearly isotropic region close to the oblate-rotator line. High-mass systems mostly occupy the slow-rotating region below it and require anisotropy or triaxiality. Gas-rich dissipative evolution retains angular momentum, forms a compact rotating stellar component, and produces low-mass fast rotators. Repeated dry major mergers randomize orbits, lower specific angular momentum, scour central cores through black-hole binaries, and build massive slow rotators.

Four characteristic contrasts are:

- high-mass ellipticals rotate slowly, while low-mass ellipticals are commonly fast rotators;
- high-mass systems are anisotropic and often triaxial or boxy, while low-mass systems are closer to oblate and disky;
- high-mass systems commonly have shallow central cores, while low-mass systems have steep central cusps or extra central light;
- high-mass systems are generally older, redder, more alpha-enhanced, and richer in hot X-ray gas, while lower-mass systems more often show younger populations, cold gas, and residual star formation.

These are population trends rather than sharp boundaries in the [fast and slow rotator galaxy](../../../../../fast-and-slow-rotator-galaxy.md) classification.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
