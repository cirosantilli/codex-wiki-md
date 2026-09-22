# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_309.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $q$ denote the quotient map and write $[X]$ for a point of [Real projective space](../../../algebraic-topology.md#real-projective-space). For $i=1,\ldots,n+1$, take the open set

$$
U_i=\{[X]:X_i\ne0\}.
$$

It is open in the [quotient topology](../../../topology.md#quotient-topology) because its inverse image under $q$ is the open set $\{X:X_i\ne0\}$. These sets cover, since a nonzero vector has at least one nonzero coordinate. Define the [manifold chart](../../../differential-geometry.md#manifold-chart)

$$
\varphi_i([X])=(X_1/X_i,\ldots,\widehat{X_i/X_i},\ldots,X_{n+1}/X_i)\in\mathbb R^n.
$$

The hat means that the $i$th coordinate is omitted. Ratios are unchanged by multiplying $X$ by any nonzero real number, so the chart is well defined. Its inverse inserts $1$ into position $i$ and takes the resulting equivalence class. The ratios and this inverse are continuous, giving a [homeomorphism](../../../topology.md#homeomorphism) $U_i\to\mathbb R^n$.

For a compact description of the [smooth transition maps](../../../differential-geometry.md#smooth-transition-map), write $a_i=1$ and let $a_k=X_k/X_i$ for $k\ne i$. On $U_i\cap U_j$ one has $a_j\ne0$, and

$$
\boxed{(\varphi_j\circ\varphi_i^{-1})(a)_k=\frac{a_k}{a_j}\quad(k\ne j).}
$$

Each coordinate is a rational [smooth function](../../../analysis.md#smooth-function) on the open domain $a_j\ne0$; reversing $i,j$ gives a smooth inverse. Thus these $n+1$ charts form the [standard affine atlas of real projective space](../../../algebraic-topology.md#standard-affine-atlas-of-real-projective-space).

For completeness, the underlying space is [Hausdorff](../../../topology.md#hausdorff-space): normalizing $X$ identifies it with the antipodal quotient of the [unit sphere](../../../topology.md#unit-sphere), and the continuous injective map $[X]\mapsto XX^T/(X^TX)$ into the space of [symmetric matrices](../../../linear-algebra.md#symmetric-matrix) separates any two distinct classes by disjoint open neighborhoods. It is also a [second-countable space](../../../topology.md#second-countable-space): pull back the countable bases of rational balls in these finitely many charts, and take their union. Therefore

$$
\boxed{\mathbb{RP}^n\text{ is a smooth manifold of dimension }n,\text{ with an atlas of }n+1\text{ charts}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the numerator in the original PDF: it contains all $n+1$ squared differentials. The local TeX ends that numerator at $n-1$, which would not give the stated [Riemannian metric](../../../differential-geometry.md#riemannian-metric).

For the [pullback of a Riemannian metric](../../../differential-geometry.md#pullback-of-a-riemannian-metric), substitute the embedding $\pi(y)=(y_1,\ldots,y_n,1)$. Its differential sends a tangent vector $v$ to $(v_1,\ldots,v_n,0)$, so $dX_i=dy_i$ for $i\le n$ and $dX_{n+1}=0$. Consequently

$$
\boxed{g=\pi^*G=\frac{\sum_{i=1}^n dy_i^2}{1+\sum_{i=1}^n y_i^2},\qquad
g_{ij}(y)=\frac{\delta_{ij}}{1+|y|^2}.}
$$

The denominator is everywhere positive. For any nonzero tangent vector,

$$
g_y(v,v)=\frac{|v|^2}{1+|y|^2}>0,
$$

so this is indeed a smooth positive-definite [Riemannian metric](../../../differential-geometry.md#riemannian-metric) on $U$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $r^2=y_1^2+y_2^2$ and write the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) as a [conformal rescaling of a Riemannian metric](../../../differential-geometry.md#conformal-rescaling-of-a-riemannian-metric):

$$
g=e^{2\omega}\delta,\qquad \omega=-\frac12\log(1+r^2).
$$

The base metric is flat, so its [Ricci scalar](../../../general-relativity.md#ricci-scalar) is zero and its [Laplacian](../../../calculus.md#laplacian) is $\Delta=\partial_1^2+\partial_2^2$. The formula for [scalar curvature under conformal rescaling](../../../differential-geometry.md#scalar-curvature-under-conformal-rescaling) simplifies in dimension two to

$$
R_g=-2e^{-2\omega}\Delta\omega.
$$

Differentiate explicitly:

$$
\partial_i\omega=-\frac{y_i}{1+r^2},\qquad
\Delta\omega=-\frac2{1+r^2}+\frac{2r^2}{(1+r^2)^2}
=-\frac2{(1+r^2)^2}.
$$

Since $e^{-2\omega}=1+r^2$, the required [Ricci scalar](../../../general-relativity.md#ricci-scalar) is

$$
\boxed{R_g(y_1,y_2)=\frac4{1+y_1^2+y_2^2}.}
$$

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the curvature convention $[\nabla_b,\nabla_c]V^d=R^d{}_{abc}V^a$, consistent with the coordinate formula later in the paper. Choose [normal coordinates](../../../general-relativity.md#normal-coordinates) at an arbitrary point $p$. The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) has $\Gamma^d{}_{ab}(p)=0$ and is torsion free, so $\Gamma^d{}_{ab}=\Gamma^d{}_{ba}$. At $p$,

$$
R^d{}_{abc}=\partial_b\Gamma^d{}_{ac}-\partial_c\Gamma^d{}_{ab}.
$$

Hence the cyclic sum is

$$
\begin{aligned}
R^d{}_{abc}+R^d{}_{bca}+R^d{}_{cab}
={}&\partial_b\Gamma^d{}_{ac}-\partial_c\Gamma^d{}_{ab}
+\partial_c\Gamma^d{}_{ba}-\partial_a\Gamma^d{}_{bc}\\
&+\partial_a\Gamma^d{}_{cb}-\partial_b\Gamma^d{}_{ca}=0.
\end{aligned}
$$

Each derivative cancels using symmetry of the two lower connection indices. Because the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) is antisymmetric in its last two indices, full antisymmetrization over $a,b,c$ equals one third of this cyclic sum. Thus

$$
\boxed{R^d{}_{[abc]}=0.}
$$

The statement is tensorial and $p$ was arbitrary, so it holds in all coordinates everywhere. This is the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $D_{abc}=\nabla_a\nabla_bK_c$. Differentiating the [Killing equation](../../../general-relativity.md#killing-equation) gives $D_{abc}=-D_{acb}$. For a covector, the [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) is

$$
D_{abc}-D_{bac}=-R^d{}_{cab}K_d=R_{cdab}K^d.
$$

Call this difference $C_{abc}$. The differentiated [Killing equation](../../../general-relativity.md#killing-equation) then gives

$$
C_{abc}=D_{abc}+D_{bca},\quad
C_{bca}=D_{bca}+D_{cab},\quad
C_{cab}=D_{cab}+D_{abc}.
$$

Taking the first minus the second plus the third yields

$$
2D_{abc}=(R_{cdab}-R_{adbc}+R_{bdca})K^d.
$$

The pair symmetries of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) and the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity) reduce the coefficient to $2R_{cbad}$. Therefore the [second covariant derivative of a Killing vector](../../../general-relativity.md#second-covariant-derivative-of-a-killing-vector) is

$$
\boxed{\nabla_a\nabla_bK_c=R_{cbad}K^d,\qquad
\nabla_a\nabla_bK^c=R^c{}_{bad}K^d.}
$$

For an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\lambda$ on a [geodesic](../../../riemannian-geometry.md#geodesic), its tangent obeys $V^b\nabla_bV^a=0$. Thus

$$
\frac{d}{d\lambda}(K_aV^a)
=V^bV^a\nabla_bK_a+K_aV^b\nabla_bV^a=0.
$$

The second term vanishes by the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation); the first contracts a symmetric product $V^aV^b$ with the antisymmetric derivative from the [Killing equation](../../../general-relativity.md#killing-equation). This establishes the [geodesic conserved quantity from a Killing vector](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector):

$$
\boxed{K_aV^a\text{ is constant along every affinely parametrized geodesic}.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

In Cartesian coordinates on [Euclidean space](../../../functional-analysis.md#euclidean-norm), the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) vanish. The [second covariant derivative of a Killing vector](../../../general-relativity.md#second-covariant-derivative-of-a-killing-vector) therefore gives

$$
\partial_\mu\partial_\rho K^\nu=0.
$$

Every first partial derivative is constant on the connected space $\mathbb R^n$. Integrating once more gives $K^\nu=A^\nu+M_\mu{}^\nu x^\mu$, with constant coefficients. The [Killing equation](../../../general-relativity.md#killing-equation) now becomes

$$
0=\partial_\mu K_\nu+\partial_\nu K_\mu=M_{\mu\nu}+M_{\nu\mu},\qquad
M_{\mu\nu}=M_\mu{}^\kappa\delta_{\kappa\nu}.
$$

Thus the coefficient is an [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix). Conversely, any such constant coefficients satisfy the [Killing equation](../../../general-relativity.md#killing-equation). The complete [Euclidean Killing vector field](../../../general-relativity.md#euclidean-killing-vector-field) is therefore

$$
\boxed{K=A^\nu\frac{\partial}{\partial x^\nu}
+M_\mu{}^\nu x^\mu\frac{\partial}{\partial x^\nu},\qquad M^T=-M.}
$$

The $n$ translation parameters and $n(n-1)/2$ rotation parameters give $n(n+1)/2$ independent [Killing vector fields](../../../general-relativity.md#killing-vector-field).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

The index order in $M_\mu{}^\nu x^\mu$ fixes the rotation sign. With the entries specified in the paper, the [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) satisfy

$$
\frac{dx^1}{d\lambda}=A^1+x^2,\qquad
\frac{dx^2}{d\lambda}=A^2-x^1,\qquad
\frac{dx^j}{d\lambda}=A^j\quad(j\ge3).
$$

Shift to $u=x^1-A^2$, $v=x^2+A^1$. Then $\dot u=v$, $\dot v=-u$, so $u^2+v^2$ is constant. If $x(0)=x_0$, put $u_0=x_0^1-A^2$ and $v_0=x_0^2+A^1$. Solving this linear [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) gives the full [local flow](../../../differential-geometry.md#local-flow):

$$
\boxed{\begin{aligned}
x^1(\lambda)&=A^2+u_0\cos\lambda+v_0\sin\lambda,\\
x^2(\lambda)&=-A^1+v_0\cos\lambda-u_0\sin\lambda,\\
x^j(\lambda)&=x_0^j+A^j\lambda\quad(j\ge3).
\end{aligned}}
$$

The planar motion is a circle centred at $(A^2,-A^1)$, traversed clockwise as $\lambda$ increases. A nonzero vector $(A^3,\ldots,A^n)$ produces a [helical orbit of a Euclidean Killing vector](../../../general-relativity.md#helical-orbit-of-a-euclidean-killing-vector); zero drift gives a circle. At zero radius the curves are straight lines in the remaining directions, or stationary points if that drift also vanishes. These formulas are defined for every real $\lambda$.

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use geometrized units $G=c=1$ and signature $(-,+,+,+)$. The original PDF starts with the [d'Alembert operator](../../../wave-equation.md#d-alembert-operator) $\Box\bar h_{\mu\nu}=-16\pi T_{\mu\nu}$; the local TeX incorrectly transcribes its derivative indices. The harmonic condition is the [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity).

Choose the retarded solution, excluding an incoming homogeneous wave. For a spatially localized source, the [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations) give

$$
\bar h_{\mu\nu}(t,\mathbf x)
=4\int\frac{T_{\mu\nu}(t-|\mathbf x-\mathbf y|,\mathbf y)}{|\mathbf x-\mathbf y|}\,d^3y.
$$

Let the source size be $D$ and the characteristic angular frequency be $\omega$. Assume the [weak-field approximation](../../../general-relativity.md#weak-field-approximation), nonrelativistic source velocities, and $D\ll\omega^{-1}\ll r$ for a radiative far-zone measurement. Then $|\mathbf x-\mathbf y|=r-\mathbf n\cdot\mathbf y+O(D^2/r)$. At leading order in $D/r$ and $\omega D$, one may replace the denominator by $r$ and the retarded time throughout the source by $t-r$, obtaining

$$
\bar h_{ij}(t,\mathbf x)\simeq\frac4r\int T_{ij}(t-r,\mathbf y)\,d^3y.
$$

To identify this integral, use [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) $\partial_\mu T^{\mu\nu}=0$ for a symmetric source tensor. Compact support or sufficient decay permits [integration by parts](../../../calculus.md#integration-by-parts) with no boundary flux. Because $T^{00}=T_{00}$ in this signature, the [second mass moment tensor](../../../general-relativity.md#second-mass-moment-tensor) satisfies

$$
\begin{aligned}
\dot I_{ij}
&=-\int\partial_kT^{k0}\,y_i y_j\,d^3y
=\int(T^{i0}y_j+T^{j0}y_i)\,d^3y,\\
\ddot I_{ij}
&=-\int\bigl(\partial_kT^{ki}\,y_j+\partial_kT^{kj}\,y_i\bigr)\,d^3y
=2\int T^{ij}\,d^3y.
\end{aligned}
$$

Spatial indices are raised with $\delta_{ij}$, so $T^{ij}=T_{ij}$. Substitution gives the [retarded quadrupole field](../../../general-relativity.md#retarded-quadrupole-field):

$$
\boxed{\bar h_{ij}(t,\mathbf x)\simeq\frac2r\ddot I_{ij}(t-r).}
$$

The assumptions are an isolated conserved source, retarded boundary conditions, weak gravity, a source small compared with the wavelength, and observation far from it. The physical radiative field follows by the [transverse-traceless projector](../../../general-relativity.md#transverse-traceless-projector) applied to this [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Write $I_a=\bar I_{aa}$ and use the right-handed rotation

$$
L(t)=\begin{pmatrix}\cos\Omega t&-\sin\Omega t&0\\
\sin\Omega t&\cos\Omega t&0\\0&0&1\end{pmatrix}.
$$

In the integral defining the [second mass moment tensor](../../../general-relativity.md#second-mass-moment-tensor), change variables to $\mathbf y=L^{-1}\mathbf x$. The [determinant](../../../linear-algebra.md#determinant) is one and $x_i=L_{ik}y_k$, giving

$$
I_{ij}(t)=\int\rho(\mathbf y)L_{ik}y_kL_{jl}y_l\,d^3y
=L_{ik}L_{jl}\bar I_{kl},\qquad \boxed{I(t)=L(t)\bar I L(t)^T.}
$$

Set $C=(I_1+I_2)/2$ and $\Delta=I_1-I_2$. Multiplication gives

$$
\boxed{\begin{aligned}
I_{11}(t)&=C+\frac\Delta2\cos(2\Omega t),\\
I_{22}(t)&=C-\frac\Delta2\cos(2\Omega t),\\
I_{12}(t)=I_{21}(t)&=\frac\Delta2\sin(2\Omega t),\\
I_{33}(t)&=I_3,\qquad I_{13}(t)=I_{23}(t)=0.
\end{aligned}}
$$

In particular, $I_{kk}=I_1+I_2+I_3$ is constant. These expressions also show how the rotating anisotropy enters the [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The time-dependent components of the [second mass moment tensor](../../../general-relativity.md#second-mass-moment-tensor) contain $\sin(2\Omega t)$ and $\cos(2\Omega t)$. Taking two time derivatives for the [retarded quadrupole field](../../../general-relativity.md#retarded-quadrupole-field) leaves that frequency unchanged. Hence the [gravitational-wave frequency](../../../general-relativity.md#gravitational-wave-frequency) is

$$
\boxed{\omega_{\mathrm{GW}}=2|\Omega|,\qquad
f_{\mathrm{GW}}=\frac{|\Omega|}{\pi}.}
$$

Here $\omega_{\mathrm{GW}}$ is angular frequency and $f_{\mathrm{GW}}$ counts cycles per unit time. If $I_1=I_2$, the [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment) is time independent, so the leading [gravitational wave](../../../general-relativity.md#gravitational-wave) amplitude vanishes and there is no emitted quadrupole frequency to measure.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Remove the constant trace from the [second mass moment tensor](../../../general-relativity.md#second-mass-moment-tensor) to obtain the [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment) $Q_{ij}=I_{ij}-\delta_{ij}I_{kk}/3$. Since $I_{kk}$ is constant, $\dddot Q_{ij}=\dddot I_{ij}$. In units $G=c=1$, the [quadrupole formula](../../../general-relativity.md#quadrupole-formula) gives

$$
\langle P\rangle=\frac15\left\langle\dddot Q_{ij}\dddot Q_{ij}\right\rangle.
$$

Its normalization can also be seen from the [gravitational-wave energy flux](../../../general-relativity.md#gravitational-wave-energy-flux): $h^{\mathrm{TT}}_{ij}=2\Lambda_{ij,kl}\ddot Q_{kl}/r$, where $\Lambda$ is the [transverse-traceless projector](../../../general-relativity.md#transverse-traceless-projector). With $S_{ij}=\dddot Q_{ij}$ and $P_{ij}=\delta_{ij}-n_i n_j$, the projection is $S^{\mathrm{TT}}_{ij}=P_{ik}P_{jl}S_{kl}-P_{ij}P_{kl}S_{kl}/2$. For a symmetric trace-free $S$,

$$
S^{\mathrm{TT}}_{ij}S^{\mathrm{TT}}_{ij}
=S_{ij}S_{ij}-2n_iS_{ij}S_{jk}n_k+\frac12(n_iS_{ij}n_j)^2.
$$

The [isotropic tensor integrals](../../../geometry-and-topology.md#isotropic-tensor-integral) $\int n_i n_j\,d\Omega=4\pi\delta_{ij}/3$ and $\int n_i n_j n_k n_l\,d\Omega=4\pi(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk})/15$ therefore give $\int |S^{\mathrm{TT}}|^2d\Omega=8\pi S_{ij}S_{ij}/5$. Integrating the flux yields $\langle P\rangle=(8\pi)^{-1}\int\langle |S^{\mathrm{TT}}|^2\rangle d\Omega=\langle S_{ij}S_{ij}\rangle/5$, as above.

Now differentiate the components from part (i). With $\Delta=I_1-I_2$,

$$
\begin{aligned}
\dddot I_{11}&=4\Delta\Omega^3\sin(2\Omega t),&
\dddot I_{22}&=-4\Delta\Omega^3\sin(2\Omega t),\\
\dddot I_{12}=\dddot I_{21}&=-4\Delta\Omega^3\cos(2\Omega t),&
\dddot I_{33}&=0.
\end{aligned}
$$

The off-diagonal component occurs twice in the contraction. Thus

$$
\dddot I_{ij}\dddot I_{ij}
=32\Delta^2\Omega^6[\sin^2(2\Omega t)+\cos^2(2\Omega t)]
=32\Delta^2\Omega^6.
$$

It is already time independent, so averaging gives

$$
\boxed{\langle P\rangle=\frac{32}{5}\Omega^6(I_1-I_2)^2.}
$$

This is the leading [gravitational radiation from a rotating triaxial body](../../../general-relativity.md#gravitational-radiation-from-a-rotating-triaxial-body); restoring units multiplies it by $G/c^5$. The source is treated as rotating uniformly over an averaging interval, with radiation reaction negligible at this order.

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $h_{ab}=\delta g_{ab}$, $h=g^{ab}h_{ab}$, and $h^{ab}=g^{ac}g^{bd}h_{cd}$. Throughout this part use the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention printed in the paper. Varying $g^{ac}g_{cb}=\delta^a{}_b$ gives the inverse-metric variation. The [determinant](../../../linear-algebra.md#determinant) identity $\delta\log|\det g|=g^{ab}h_{ab}$ gives the [volume form](../../../differential-form.md#volume-form) variation. Together these are

$$
\boxed{\delta g^{ab}=-h^{ab},\qquad
\delta(d\operatorname{vol}_g)=\frac12h\,d\operatorname{vol}_g.}
$$

In Lorentzian coordinates the latter reads $\delta\sqrt{-g}=\frac12\sqrt{-g}\,h$.

For the connection, vary [metric compatibility](../../../fiber-bundle.md#metric-compatibility) $\nabla_a g_{bc}=0$:

$$
\nabla_a h_{bc}=g_{dc}\delta\Gamma^d{}_{ab}+g_{bd}\delta\Gamma^d{}_{ac}.
$$

Add the equations with derivatives $a,b$, subtract that with derivative $c$, and use symmetry of the lower indices of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). This gives

$$
\boxed{\delta\Gamma^c{}_{ab}=\frac12g^{cd}
(\nabla_a h_{bd}+\nabla_b h_{ad}-\nabla_d h_{ab}).}
$$

The difference of two connections is a tensor, so this formula is covariant.

Varying the coordinate curvature formula yields the [Palatini identity](../../../general-relativity.md#palatini-identity)

$$
\delta R_{ab}=\nabla_c\delta\Gamma^c{}_{ab}-\nabla_b\delta\Gamma^c{}_{ac}.
$$

The contractions of the connection variation are

$$
g^{ab}\delta\Gamma^c{}_{ab}=\nabla_a h^{ac}-\frac12\nabla^c h,\qquad
\delta\Gamma^c{}_{ac}=\frac12\nabla_a h.
$$

Finally, $\delta R=(\delta g^{ab})R_{ab}+g^{ab}\delta R_{ab}$ gives the [metric variation of scalar curvature](../../../general-relativity.md#metric-variation-of-scalar-curvature):

$$
\boxed{\delta R=-R^{ab}h_{ab}-\nabla^c\nabla_c h+\nabla^a\nabla^b h_{ab},
\qquad\alpha=-1,\quad\beta=1.}
$$

The double divergence may equivalently be written $\nabla_a\nabla_bh^{ab}$: relabeling the contracted dummy indices and using symmetry of $h^{ab}$ gives the same expression. The derivative terms are a [covariant divergence](../../../general-relativity.md#covariant-divergence), useful when varying a curvature-dependent action.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Define the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) by [metric variation](../../../general-relativity.md#metric-variation) with the scalar held fixed:

$$
\delta S=\frac12\int d^4x\,\sqrt{-g}\,T^{ab}\delta g_{ab}.
$$

Use compactly supported variations to remove boundary terms. The first [covariant derivative](../../../general-relativity.md#covariant-derivative) of a [scalar field](../../../quantum-field-theory.md#scalar-field) is an ordinary derivative, so it has no connection variation. Varying the kinetic term and the [volume form](../../../differential-form.md#volume-form) gives

$$
T^{\mathrm{kin}}_{ab}=\nabla_a\Phi\nabla_b\Phi-\frac12g_{ab}\nabla_c\Phi\nabla^c\Phi.
$$

For the curvature term set $f=\Phi^2$. Using part (a), its variation is

$$
\delta S_\xi=-\xi\int\sqrt{-g}\left[
\left(\frac12Rf\,g^{ab}-fR^{ab}\right)h_{ab}
-f\Box h+f\nabla^a\nabla^b h_{ab}\right]d^4x.
$$

Applying [integration by parts](../../../calculus.md#integration-by-parts) twice moves each pair of derivatives from the metric variation onto $f$. The result is

$$
\delta S_\xi=\xi\int\sqrt{-g}
\left[fG^{ab}+g^{ab}\Box f-\nabla^a\nabla^b f\right]h_{ab}\,d^4x,
$$

where $G_{ab}=R_{ab}-Rg_{ab}/2$ is the [Einstein tensor](../../../general-relativity.md#einstein-tensor) and $\Box=\nabla^c\nabla_c$ is the [d'Alembert operator](../../../wave-equation.md#d-alembert-operator). Comparing with the defining variation gives the [stress-energy tensor of a nonminimally coupled scalar field](../../../general-relativity.md#stress-energy-tensor-of-a-nonminimally-coupled-scalar-field):

$$
\boxed{T_{ab}=\nabla_a\Phi\nabla_b\Phi
-\frac12g_{ab}(\nabla\Phi)^2
+2\xi\left[\Phi^2G_{ab}+g_{ab}\Box(\Phi^2)-\nabla_a\nabla_b(\Phi^2)\right].}
$$

The factor $2\xi$ follows from the action's coupling $-\xi R\Phi^2$; a convention using $-\xi R\Phi^2/2$ would instead give $\xi$ in that bracket. At $\xi=0$ this reduces to the massless [Klein-Gordon scalar stress-energy tensor](../../../general-relativity.md#klein-gordon-scalar-stress-energy-tensor).

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

The [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) obtained by varying the [nonminimally coupled scalar field](../../../scalar-field-theory.md#nonminimally-coupled-scalar-field) is

$$
\boxed{\Box\Phi-2\xi R\Phi=0.}
$$

One can check [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) directly. The divergence of the kinetic contribution is $(\Box\Phi)\nabla_b\Phi$, because second derivatives of a scalar commute. With $f=\Phi^2$, the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) gives $\nabla^aG_{ab}=0$, while the [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) gives

$$
\Box\nabla_bf=\nabla_b\Box f+R_b{}^c\nabla_cf.
$$

Consequently

$$
\begin{aligned}
\nabla^a\left[fG_{ab}+g_{ab}\Box f-\nabla_a\nabla_bf\right]
&=G_{ab}\nabla^af+\nabla_b\Box f-\Box\nabla_bf\\
&=(G_{ab}-R_{ab})\nabla^af=-\frac12R\nabla_bf.
\end{aligned}
$$

Since $\nabla_bf=2\Phi\nabla_b\Phi$, the full [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) satisfies

$$
\boxed{\nabla^aT_{ab}=(\Box\Phi-2\xi R\Phi)\nabla_b\Phi=0\quad\text{on shell}.}
$$

The general reason is the [diffeomorphism Noether identity for a scalar field](../../../general-relativity.md#diffeomorphism-noether-identity-for-a-scalar-field). Under the [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) along a compactly supported [vector field](../../../calculus.md#vector-field) $X$, $\delta g_{ab}=2\nabla_{(a}X_{b)}$ and $\delta\Phi=X^a\nabla_a\Phi$. Invariance of the action under [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism) gives, after [integration by parts](../../../calculus.md#integration-by-parts),

$$
0=\int\sqrt{-g}\,X^b\left[-\nabla^aT_{ab}
+\frac1{\sqrt{-g}}\frac{\delta S}{\delta\Phi}\nabla_b\Phi\right]d^4x.
$$

Arbitrariness of $X$ gives the same divergence identity. Conservation requires the scalar equation of motion, with no need to impose the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) for the background metric.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
