# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_309.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Under [parallel transport](../../../fiber-bundle.md#parallel-transport), the gyroscope spin obeys $u^b\nabla_b s^a=0$, and its freely falling circular orbit is a [geodesic](../../../riemannian-geometry.md#geodesic), $u^b\nabla_bu^a=0$. Metric compatibility therefore gives

$$
u^c\nabla_c(s^au_a)
=(u^c\nabla_cs^a)u_a+s^au^c\nabla_cu_a=0.
$$

**Thus $s^au_a$ is constant along the orbit.**

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Initially $s^a$ is radial, whereas the circular-orbit four-velocity has only $t$ and $\phi$ components. The diagonal [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) therefore gives $s^au_a=0$ at $t=0$. By part i,

$$
\boxed{s^au_a=0}
$$

throughout the orbit.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In a [coordinate basis](../../../differential-geometry.md#coordinate-basis), parallel transport is

$$
\frac{ds^\mu}{d\tau}+\Gamma^\mu_{\rho\nu}\frac{dx^\rho}{d\tau}s^\nu=0.
$$

Along the circular orbit, $dr=d\theta=0$ and $d\phi/dt=\Omega$. Dividing by $dt/d\tau$ gives

$$
\boxed{\frac{ds^\mu}{dt}+\Gamma^\mu_{t\nu}s^\nu
+\Omega\Gamma^\mu_{\phi\nu}s^\nu=0}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On the equatorial plane, the only potentially relevant angular connection coefficient is $\Gamma^\theta_{\phi\phi}=-\sin\theta\cos\theta$, which vanishes at $\theta=\pi/2$. The $\theta$ transport equation is consequently $ds^\theta/dt=0$. Since the initially radial spin has $s^\theta(0)=0$,

$$
\boxed{s^\theta(t)=0}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Writing $f=1-2M/R$, orthogonality from part a gives

$$
0=u^t(-fs^t+R^2\Omega s^\phi),
\qquad
s^t=\frac{R^2\Omega}{f}s^\phi.
$$

The needed [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) are

$$
\Gamma^r_{tt}=\frac{fM}{R^2},
\qquad
\Gamma^r_{\phi\phi}=-fR,
\qquad
\Gamma^\phi_{\phi r}=\frac1R.
$$

The radial and azimuthal transport equations reduce to

$$
\dot s^r=\Omega(R-3M)s^\phi,
\qquad
\dot s^\phi=-\frac\Omega R s^r.
$$

Hence

$$
\ddot s^r+\Omega^2\left(1-\frac{3M}{R}\right)s^r=0.
$$

With the stated initial direction,

$$
\boxed{s^r=A\cos(\Omega' t),\qquad
s^\phi=-\frac{A\Omega}{\Omega'R}\sin(\Omega't)},
\qquad
\boxed{\Omega'=\Omega\sqrt{1-\frac{3M}{R}}}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Metric compatibility and parallel transport imply

$$
u^c\nabla_c(s^as_a)=2s_a u^c\nabla_cs^a=0.
$$

Using $s^t=R^2\Omega s^\phi/f$ gives

$$
s^2=\frac{(s^r)^2}{f}
+\left(R^2-\frac{R^4\Omega^2}{f}\right)(s^\phi)^2.
$$

Substitution of part d makes this independent of $t$ precisely when

$$
\boxed{\Omega^2=\frac{M}{R^3}},
$$

the relativistic circular-orbit form of [Kepler third law](../../../physics.md#kepler-s-third-law). One orbit takes $T=2\pi/\Omega$, during which the spin phase advances by $\Omega'T=2\pi\sqrt{1-3M/R}$. Relative to the radial direction, the spin therefore lags by the [geodetic precession](../../../general-relativity.md#geodetic-effect) angle

$$
\boxed{\alpha=2\pi\left[1-\sqrt{1-\frac{3M}{R}}\right]}.
$$

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Varying the inverse metric in $H_{abc}H^{abc}$ produces three identical terms. With $T_{ab}=-(2/\sqrt{-g})\delta S_H/\delta g^{ab}$,

$$
\boxed{T_{ab}=H_{acd}H_b{}^{cd}-\frac16g_{ab}H_{cde}H^{cde}}.
$$

In four dimensions use the [Hodge star operator](../../../differential-form.md#hodge-star-operator) to define the dual covector $v^a=(1/3!)\epsilon^{abcd}H_{bcd}$. Then $H^2=-6v^2$ and $H_{acd}H_b{}^{cd}=2(v_av_b-g_{ab}v^2)$, so equivalently

$$
\boxed{T_{ab}=2v_av_b-g_{ab}v^2}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Under an infinitesimal [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) generated by $\xi^a$,

$$
\delta g_{ab}=2\nabla_{(a}\xi_{b)},
\qquad
\delta\omega_a=\mathcal L_\xi\omega_a
=\xi^c\nabla_c\omega_a+\omega_c\nabla_a\xi^c.
$$

Insert these variations into

$$
\delta S_{\rm matter}=\int d^4x\sqrt{-g}
\left(-\frac12T^{ab}\delta g_{ab}+E^a\delta\omega_a\right)
$$

and integrate derivatives of $\xi^a$ by parts. Diffeomorphism invariance and arbitrariness of $\xi^b$ give the [Noether identity](../../../general-relativity.md#noether-identity)

$$
\boxed{\nabla_aT^a{}_b=E^a\nabla_b\omega_a-\nabla_a(E^a\omega_b)}.
$$

On the covector equation of motion $E^a=0$, this reduces to [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), $\nabla_aT^a{}_b=0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The projection $X\mapsto X_\parallel$ is tensorial. Although a covariant derivative is not $C^\infty$-linear in its second argument, the extra term in $\nabla_{X_\parallel}(fY_\parallel)$ is proportional to $Y_\parallel$, whose contraction with the normal vanishes. Thus $K(X,Y)$ is $C^\infty$-linear in both arguments and defines a $(0,2)$ tensor on the hypersurface.

Since $n_aY_\parallel^a=0$,

$$
-n_a\nabla_{X_\parallel}Y_\parallel^a
=(X_\parallel)^c(Y_\parallel)^d\nabla_cn_d.
$$

Therefore the [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature) is

$$
\boxed{K_{ab}=h_a{}^ch_b{}^d\nabla_cn_d}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

A hypersurface normal is locally proportional to the gradient of a defining function. The [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) therefore implies

$$
h_a{}^ch_b{}^d\nabla_{[c}n_{d]}=0.
$$

Taking the antisymmetric part of the formula in part i gives $K_{[ab]}=0$, hence

$$
\boxed{K_{ab}=K_{ba}}.
$$

Equivalently, torsion freedom gives $K(X,Y)-K(Y,X)=-n\mathbin\cdot[X,Y]=0$ because the bracket of tangent vector fields is tangent.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The affine geodesic equation gives

$$
U^a\nabla_a(U^bn_b)=U^aU^b\nabla_an_b.
$$

Unit normalization implies $n^b\nabla_an_b=0$, and decomposition of the first index gives

$$
\nabla_an_b=K_{ab}+n_a(n^c\nabla_cn_b).
$$

Consequently, at the intersection point,

$$
\boxed{U^a\nabla_a(U^bn_b)=K_{ab}U^aU^b+f,U^bn_b},
\qquad
f=U^an^c\nabla_cn_a.
$$

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

Choose any tangent vector $V^a\in T_p\Sigma$ and let the affinely parametrized geodesic with initial tangent $V^a$ start at $p$. If $\Sigma$ is [totally geodesic](../../../differential-geometry.md#totally-geodesic-hypersurface), then $U^an_a$ remains zero. Its initial derivative is therefore zero. Part iii, with $U^an_a=0$ at $p$, gives

$$
K_{ab}V^aV^b=0.
$$

This holds for every tangent $V$. Since $K$ is symmetric, the [polarization identity](../../../linear-algebra.md#polarization-identity) implies

$$
\boxed{K_{ab}=0}.
$$

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Assume a spatially compact source of size $d\ll r=|\mathbf x|$, internal speeds much smaller than one, and wavelength much larger than $d$. In the [radiation zone](../../../electromagnetism.md#radiation-zone),

$$
|\mathbf x-\mathbf x'|=r+O(d),
\qquad
t-|\mathbf x-\mathbf x'|=t-r+O(d),
$$

so

$$
\bar h_{ij}(t,\mathbf x)\simeq\frac4r\int d^3x'\,T_{ij}(t-r,\mathbf x').
$$

Define the mass quadrupole moment

$$
I_{ij}(t)=\int d^3x\,T_{00}(t,\mathbf x)x_ix_j.
$$

Twice using $\partial_\mu T^{\mu\nu}=0$, discarding boundary terms, gives

$$
\ddot I_{ij}=2\int d^3x\,T_{ij}.
$$

Hence

$$
\boxed{\bar h_{ij}(t,\mathbf x)\simeq\frac2r\ddot I_{ij}(t-r)}.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

In [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition), $\partial_\mu\bar h^{\mu\nu}=0$. A leading outgoing far-zone field depends on retarded time $u=t-r$, so $\partial_j=-\widehat x_j\partial_u+O(r^{-1})$. Taking $\nu=i$ and using $\bar h^{0i}=-\bar h_{0i}$ gives

$$
\partial_u\bar h_{0i}=-\widehat x_j\partial_u\bar h_{ji}.
$$

Dropping a nonradiative integration constant and using part i,

$$
\boxed{\bar h_{0i}(t,\mathbf x)
\simeq-\frac{2\widehat x_j}{r}\ddot I_{ij}(t-r)}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

With $u=t-r$, direct integration gives

$$
I_{xx}=\frac{ma^2}{3}\cos^2\omega u,
\quad
I_{yy}=\frac{ma^2}{3}\sin^2\omega u,
\quad
I_{xy}=\frac{ma^2}{3}\sin\omega u\cos\omega u,
\quad
I_{zz}=0.
$$

Therefore the time-dependent spatial field is

$$
\boxed{
\bar h_{ij}^{\rm rad}=\frac{4ma^2\omega^2}{3r}
\begin{pmatrix}
-\cos2\omega u&-\sin2\omega u&0\\
-\sin2\omega u&\cos2\omega u&0\\
0&0&0
\end{pmatrix}}.
$$

The [gravitational-wave frequency](../../../general-relativity.md#gravitational-wave-frequency) is $2\omega$. On the positive $z$-axis this matrix is transverse and traceless. It is a rotating combination of the [plus polarization](../../../general-relativity.md#plus-polarization) and [cross polarization](../../../general-relativity.md#cross-polarization), with amplitude proportional to $1/z$, exactly as for a plane wave propagating in the $z$ direction.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The [quadrupole formula](../../../general-relativity.md#quadrupole-formula) in units $G=c=1$ is

$$
P=\frac15\left\langle\dddot Q_{ij}\dddot Q_{ij}\right\rangle,
\qquad
Q_{ij}=I_{ij}-\frac13\delta_{ij}I_{kk}.
$$

Here $I_{kk}=ma^2/3$ is constant, so its trace subtraction has no third derivative. If $B=4ma^2\omega^3/3$, then

$$
\dddot I_{xx}=B\sin2\omega t,
\quad
\dddot I_{yy}=-B\sin2\omega t,
\quad
\dddot I_{xy}=-B\cos2\omega t.
$$

Thus $\dddot I_{ij}\dddot I_{ij}=2B^2$ and

$$
\boxed{\langle P\rangle=\frac{32}{45}m^2a^4\omega^6}.
$$

Restoring units multiplies this by $G/c^5$.

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the displayed frame,

$$
e^0(e_0)=1,
\quad e^0(e_2)=0,
\quad e^1(e_1)=1,
\quad e^2(e_2)=1,
$$

and all other pairings vanish. Hence the proposed one-forms are the dual coframe. Substitution into

$$
g=-(e^0)^2+(e^1)^2+(e^2)^2
$$

reproduces the metric, proving that the frame is an [orthonormal frame](../../../general-relativity.md#orthonormal-frame-in-spacetime) with signature $(-,+,+)$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The exterior derivatives of the coframe are

$$
de^0=\sqrt2,e^1\wedge e^2,
\qquad de^1=0,
\qquad de^2=e^1\wedge e^2.
$$

Insert the proposed connection into [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation) and use $\omega_{\mu\nu}=-\omega_{\nu\mu}$. The three equations give

$$
B-A=\sqrt2,
\qquad C=-A,
\qquad C=B,
\qquad D=-1.
$$

Thus

$$
\boxed{A=-\frac1{\sqrt2},\qquad B=C=\frac1{\sqrt2},\qquad D=-1}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Using [Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation) gives

$$
\boxed{\Theta_{01}=\frac12e^0\wedge e^1,
\qquad \Theta_{02}=\frac12e^0\wedge e^2,
\qquad \Theta_{12}=\frac12e^1\wedge e^2}.
$$

Since $\Theta_{\mu\nu}=R_{\mu\nu\rho\sigma}e^\rho\wedge e^\sigma/2$, the independent nonzero lowered [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) components are

$$
\boxed{R_{0101}=R_{0202}=R_{1212}=\frac12},
$$

with all others determined by the symmetries of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Contraction in the orthonormal frame yields

$$
R_{00}=1,
\qquad R_{11}=R_{22}=0,
\qquad R=-1.
$$

Hence

$$
G_{00}=G_{11}=G_{22}=\frac12.
$$

For $u^\mu=(1,0,0)$, pressureless matter has $T_{00}=\rho$ and vanishing spatial components. The spatial Einstein equations $G_{ii}+\Lambda\eta_{ii}=0$ give $\Lambda=-1/2$, while the time component gives $1=8\pi\rho$. Thus, for $G_N=1$,

$$
\boxed{\Lambda=-\frac12,\qquad \rho=\frac1{8\pi}}.
$$

If the convention is $G_{ab}+\Lambda g_{ab}=T_{ab}$, the corresponding density is simply $\rho=1$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Because the metric coefficients are independent of $t$ and $y$,

$$
\partial_t,qquad \partial_y
$$

are [Killing vector fields](../../../general-relativity.md#killing-vector-field). The maps

$$
\phi_s(t,x,y)=(t,x+s,e^{-s}y)
$$

satisfy $\phi_s\circ\phi_r=\phi_{s+r}$. Moreover, $dx$ is unchanged and both $e^xdy$ and $dt+\sqrt2e^xdy$ are invariant, so $\phi_s^*g=g$. Differentiating at $s=0$ produces the third Killing field

$$
\boxed{K=\partial_x-y\partial_y}.
$$

Given two points, first use $\phi_s$ to match their $x$ coordinates, then translations generated by $\partial_y$ and $\partial_t$ to match $y$ and $t$. The isometry group therefore acts transitively, so the spacetime is a [homogeneous space](../../../lie-theory.md#homogeneous-space).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
