# Paper 2

↑ **Parent:** [2003](../2003.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2003/PaperNST_IB_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2003/PaperNST_IB_2.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [Solution](#7/solution)
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
  - [iii](#7/iii)
    - [Solution](#7/iii/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a vacuum [electric potential](../../electric-field.md#electric-potential), put $\Phi=R(r)Y(\theta)$ in [Laplace's equation](../../partial-differential-equation.md#laplace-equation) in [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system). Multiplication by $r^2/(RY)$ separates the radial and angular terms. With separation constant $\ell(\ell+1)$ and $x=\cos\theta$, the angular [Legendre differential equation](../../linear-ordinary-differential-equation.md#legendre-differential-equation) is

$$
\boxed{\frac d{dx}\left[(1-x^2)\frac{dP_\ell}{dx}\right]+\ell(\ell+1)P_\ell=0.}
$$

Regularity at both polar axes selects nonnegative [integers](../../integer.md) $\ell$ and the [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial). The radial equation is $(r^2R')'-\ell(\ell+1)R=0$, whose independent solutions are $r^\ell$ and $r^{-\ell-1}$. Hence the angularly regular axisymmetric vacuum solution is

$$
\boxed{\Phi(r,\theta)=\sum_{\ell=0}^\infty(A_\ell r^\ell+B_\ell r^{-\ell-1})P_\ell(\cos\theta).}
$$

The radial [domain](../../topology.md#domain-mathematical-analysis) and its [boundary conditions](../../differential-equation.md#boundary-condition) determine which terms are admissible.

For the given [charge density](../../electric-charge.md#charge-density), only $P_1(\cos\theta)=\cos\theta$ is forced. Write $\Phi=f(r)\cos\theta$. The interior radial [Poisson equation](../../partial-differential-equation.md#poisson-s-equation) is $f''+2f'/r-2f/r^2=-4$. The identity for the [Poisson equation with a spherical harmonic source](../../partial-differential-equation.md#poisson-equation-with-a-spherical-harmonic-source) gives the particular solution $f_p=-r^2$, since the radial operator takes $r^2$ to four. Finiteness at zero and decay at infinity therefore give

$$
\Phi_{\rm in}=(Ar-r^2)\cos\theta,\qquad\Phi_{\rm out}=Br^{-2}\cos\theta.
$$

Continuity of the [electric potential](../../electric-field.md#electric-potential) and its radial [derivative](../../calculus.md#derivative) at $a$ requires $Aa-a^2=B/a^2$ and $A-2a=-2B/a^3$. Solving gives $A=4a/3$, $B=a^4/3$, so

$$
\boxed{\Phi(r,\theta)=\begin{cases}(\tfrac43ar-r^2)\cos\theta,&0\leq r\leq a,\\\dfrac{a^4}{3r^2}\cos\theta,&r\geq a.\end{cases}}
$$

All other angular modes have zero coefficients after imposing regularity, matching and decay. At the origin the interior expression is $(4a/3)z-rz$, which extends with a continuous [gradient](../../multivariable-calculus.md#gradient) and value zero. The angular [charge density](../../electric-charge.md#charge-density) has no unique value exactly at that point; [Poisson's equation](../../partial-differential-equation.md#poisson-s-equation) holds classically for $r>0$ and as a [weak solution](../../partial-differential-equation.md#weak-solution) through the origin. There is no additional point charge.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Expand the [divergence](../../multivariable-calculus.md#divergence) of $\Phi\nabla\Psi-\Psi\nabla\Phi$. The cross terms cancel, leaving $\Phi\Delta\Psi-\Psi\Delta\Phi$. The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives [Green's second identity](../../partial-differential-equation.md#green-second-identity),

$$
\int_V(\Phi\Delta\Psi-\Psi\Delta\Phi)dV=\int_S(\Phi\partial_n\Psi-\Psi\partial_n\Phi)dS.
$$

Use the [Green function](../../green-s-function.md) convention $\Delta_xG(x,x_0)=\delta(x-x_0)$. Integrating over a bounded [domain](../../topology.md#domain-mathematical-analysis) containing $x_0$ yields $\boxed{\int_S\partial_nG\,dS=1}$. Thus zero [Neumann boundary data](../../differential-equation.md#neumann-boundary-data) would be incompatible with this unit [Dirac delta](../../distribution-theory.md#dirac-delta-function) source. A suitable [Neumann Green function with constant boundary flux](../../green-s-function.md#neumann-green-function-with-constant-boundary-flux) instead has $\partial_nG=1/|S|$, where $|S|$ is the boundary area. Substituting $\Psi=G$, $\Delta\Phi=\sigma$, $\partial_n\Phi=f$ gives

$$
\boxed{\Phi(x_0)=\int_VG\sigma\,dV-\int_SGf\,dS+\frac1{|S|}\int_S\Phi\,dS.}
$$

The last term is an undetermined constant. The data must obey the [Neumann Poisson problem](../../partial-differential-equation.md#neumann-poisson-problem) compatibility condition $\int_V\sigma\,dV=\int_Sf\,dS$, obtained by integrating the original equation. Under this condition an additive constant in $G$ cancels from the first two terms.

For the upper half-space, reflect the source to $x_0^*=(x_{0,1},x_{0,2},-x_{0,3})$. The [method of images](../../mathematics.md#method-of-images) with equal-sign sources gives

$$
\boxed{G(x,x_0)=-\frac1{4\pi}\left(\frac1{|x-x_0|}+\frac1{|x-x_0^*|}\right).}
$$

The reflected singularity lies outside the [domain](../../topology.md#domain-mathematical-analysis); on $z=0$ the two normal [derivatives](../../calculus.md#derivative) cancel, so $\partial_nG=-\partial_zG=0$. Its total unit flux passes through a large hemisphere at infinity, where $G\sim-1/(2\pi R)$. This is why the bounded-domain condition on the boundary flux cannot be applied to the infinite plane alone.

With zero interior source and the given point boundary source, the boundary representation is $\Phi(x_0)=-G((0,0,0),x_0)$. The terms at infinity vanish for this resulting $1/R$ field. Therefore

$$
\boxed{\Phi(x,y,z)=\frac1{2\pi\sqrt{x^2+y^2+z^2}},\qquad z>0.}
$$

To check the singular boundary condition, $-\partial_z\Phi=z/[2\pi(x^2+y^2+z^2)^{3/2}]$ is the [Poisson kernel for the upper half-space](../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-space). Its [integral](../../integral.md) over a horizontal plane is one and its [mass](../../classical-mechanics.md#mass) concentrates at the origin as $z\downarrow0$, giving $\partial_n\Phi=\delta(x)\delta(y)$ in the distributional sense. This is the [Neumann point source on a half-space boundary](../../partial-differential-equation.md#neumann-point-source-on-a-half-space-boundary).

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Choose the [square root of one minus z squared](../../algebra.md#square-root-of-one-minus-z-squared) with $f(0)=1$: explicitly $f(z)=\sqrt{1-z}\sqrt{1+z}$ with principal [square roots](../../algebra.md#square-root). It is single valued and [holomorphic](../../holomorphic-function.md) away from the two specified exterior real [branch cuts](../../analysis.md#branch-cut). If $q(x)=\sqrt{x^2-1}>0$ for $|x|>1$, its boundary values are

$$
\boxed{\begin{array}{c|cc}&f(x+i0)&f(x-i0)\\\hline x>1&-iq(x)&+iq(x)\\x<-1&+iq(x)&-iq(x)\end{array}.}
$$

For example, above the right cut $1-z$ approaches the negative real axis from below, selecting $-i\sqrt{x-1}$; above the left cut $1+z$ approaches it from above, selecting $+i\sqrt{-x-1}$. Continuing once around either [branch point](../../complex-analysis.md#branch-point) changes the sign, which explains the need for cuts.

Apply the [residue theorem](../../analysis.md#residue-theorem) to $F(z)=1/[zf(z)]$ on a large disk slit along both cuts, with small arcs excluding $\pm1$. The only enclosed [pole](../../isolated-singularity.md#pole) is at zero, and its [residue](../../analysis.md#residue) is $1/f(0)=1$. On the positively oriented boundary of the slit domain, the upper right lip runs from one to $R$, and the lower right lip returns from $R$ to one. The jump in $F$ gives their combined [integral](../../integral.md) as $2iI_R$, where $I_R=\int_1^Rdx/[x\sqrt{x^2-1}]$. The left lips similarly give $2iI_R$ after the substitution $x=-t$.

<a id="3/image-a-contour-around-the-two-exterior-square-root-cuts"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2-two-cut-contour.png)

**[Figure 1](#3/image-a-contour-around-the-two-exterior-square-root-cuts). A contour around the two exterior square-root cuts**. Original schematic. The two slit boundaries are traversed with the retained domain on the left; each contributes twice the same real integral multiplied by i. The sole enclosed pole is at zero.

The small arcs contribute $O(\sqrt\varepsilon)$ because the branch singularities have order $-1/2$. The large arc contributes $O(R^{-1})$ because $F(z)=O(|z|^{-2})$. Taking [limits](../../calculus.md#limit-of-a-function) therefore yields $4iI=2\pi i$, and hence

$$
\boxed{I=\frac\pi2.}
$$

The real substitution $x=\sec\theta$ independently reduces the [integral](../../integral.md) to $\int_0^{\pi/2}d\theta$, confirming its value and sign.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Compute the [complex derivative](../../holomorphic-function.md#complex-derivative) along horizontal and vertical increments. Along the real direction, $f'=u_x+iv_x$; along the imaginary direction, $f'=(u_y+iv_y)/i=v_y-iu_y$. Equality gives the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations)

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

The real and imaginary parts of a [holomorphic function](../../holomorphic-function.md) are smooth. Equality of their [mixed partial derivatives](../../multivariable-calculus.md#mixed-partial-derivative) then gives $u_{xx}+u_{yy}=v_{yx}-v_{xy}=0$ and $v_{xx}+v_{yy}=-u_{yx}+u_{xy}=0$, proving that both are [harmonic functions](../../partial-differential-equation.md#harmonic-function).

For the first real part, $u_x=2x$ and $u_y=-2y$. The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) require $v_y=2x$ and $v_x=2y$, so its [harmonic conjugate](../../partial-differential-equation.md#harmonic-conjugate) is $v=2xy+C$. Therefore

$$
\boxed{f(z)=z^2+iC,\qquad C\in\mathbb R.}
$$

For the second real part, $u=x/(x^2+y^2)$ is the real part of $1/z$. Its [harmonic conjugate](../../partial-differential-equation.md#harmonic-conjugate) is $-y/(x^2+y^2)+C$, giving

$$
\boxed{f(z)=\frac1z+iC,\qquad C\in\mathbb R,\quad z\ne0.}
$$

These are the most general answers on a connected open [domain](../../topology.md#domain-mathematical-analysis): the difference of two candidates has zero real part, so the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) make its imaginary part constant. The second [function](../../function.md) cannot extend [holomorphically](../../holomorphic-function.md) through zero.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [Laplace transform](../../integral-transform.md#laplace-transform) is $\overline f(p)=\int_0^\infty e^{-pt}f(t)dt$ wherever it converges. For sufficiently large $\operatorname{Re}p$, suitable exponential bounds justify [integration by parts](../../calculus.md#integration-by-parts) and [differentiation under the integral sign](../../analysis.md#differentiation-under-the-integral-sign), giving

$$
\boxed{\mathcal L[f'](p)=p\overline f(p)-f(0^+),\qquad\mathcal L[tf](p)=-\overline f'(p).}
$$

For a nonnegative [integer](../../integer.md) $n$ and real $p>0$, substitute $u=pt$ in the [gamma integral](../../complex-analysis.md#gamma-integral). The result extends holomorphically to $\operatorname{Re}p>0$, giving

$$
\boxed{\mathcal L[t^n](p)=\frac{n!}{p^{n+1}},\qquad\operatorname{Re}p>0.}
$$

This also follows recursively from the second identity, starting with $\mathcal L[1]=1/p$.

Put $G=\overline g$, $g_0=g(0^+)$ and $g_1=g'(0^+)$. For a solution with finite initial values and the required transform bounds, the transformed equation is

$$
-\frac d{dp}(p^2G-pg_0-g_1)+(pG-g_0)+\frac d{dp}(pG-g_0)+2G=0.
$$

The initial-value terms cancel, leaving $(p-p^2)G'+(3-p)G=0$. On the real interval $p>1$, a nonzero solution satisfies

$$
\frac{G'}G=\frac{3-p}{p^2-p}=-\frac3p+\frac2{p-1}.
$$

Integration gives $G=C(p-1)^2/p^3=C(1/p-2/p^2+1/p^3)$. Inverting term by term yields

$$
\boxed{g(t)=C\left(1-2t+\frac{t^2}2\right).}
$$

Taking $C=1$ gives a nonzero solution, verified by direct substitution. It is $L_2(t)$, and the rational transform agrees with the general [Laplace transform of a Laguerre polynomial](../../linear-operator-theory.md#laplace-transform-of-a-laguerre-polynomial). No claim about solutions with singular initial behavior is needed to produce this regular solution.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Under an orthogonal Cartesian change of axes $Q$, the [vector](../../vector-space.md#vector) components transform as $v_i'=Q_{ia}v_a$, while $v_k'v_k'=v_av_a$ and $\delta_{ij}=Q_{ia}Q_{ja}$. Substitution gives

$$
P_{ij}'=\delta_{ij}-\frac{Q_{ia}v_aQ_{jb}v_b}{v_cv_c}=Q_{ia}Q_{jb}\left(\delta_{ab}-\frac{v_av_b}{v_cv_c}\right)=Q_{ia}Q_{jb}P_{ab}.
$$

This is the rank-two [Cartesian tensor](../../multilinear-algebra.md#cartesian-tensor) transformation law. The nonzero assumption ensures that the denominator is positive. In [matrix](../../vector-space.md#matrix) form $P=I-vv^T/(v^Tv)$ is the [orthogonal projection matrix](../../inner-product.md#orthogonal-projection-matrix) onto the [orthogonal complement](../../hilbert-space.md#orthogonal-complement) of $v$.

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

Contract with $v_j$ and use its squared [Euclidean norm](../../normed-vector-space.md#euclidean-norm):

$$
\boxed{P_{ij}v_j=v_i-v_i\frac{v_jv_j}{v_kv_k}=0.}
$$

Thus $v$ lies in the [kernel](../../kernel-of-a-linear-map.md) of this [orthogonal projection](../../hilbert-space.md#orthogonal-projection).

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

The [orthogonality](../../inner-product.md#orthogonal-vectors) condition is $v_ju_j=0$, so

$$
\boxed{P_{ij}u_j=u_i-v_i\frac{v_ju_j}{v_kv_k}=u_i.}
$$

Every [vector](../../vector-space.md#vector) in the [orthogonal complement](../../hilbert-space.md#orthogonal-complement) is fixed by the [orthogonal projection](../../hilbert-space.md#orthogonal-projection).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [Cartesian tensor](../../multilinear-algebra.md#cartesian-tensor) law is $T'_{ik}=Q_{ia}Q_{kb}T_{ab}$. In every complete [tensor contraction](../../multilinear-algebra.md#tensor-contraction), summation over a transformed index contracts a pair of $Q$ factors to a [Kronecker delta](../../multilinear-algebra.md#kronecker-delta). In detail,

$$
\alpha'=Q_{ia}Q_{ib}T_{ab}=\delta_{ab}T_{ab}=\alpha,
$$



$$
\beta'=Q_{ia}Q_{kb}Q_{kc}Q_{id}T_{ab}T_{cd}=\delta_{bc}\delta_{ad}T_{ab}T_{cd}=T_{ab}T_{ba}=\beta,
$$



$$
\gamma'=Q_{ia}Q_{kb}Q_{kc}Q_{md}Q_{me}Q_{if}T_{ab}T_{cd}T_{ef}=\delta_{bc}\delta_{de}\delta_{af}T_{ab}T_{cd}T_{ef}=T_{ab}T_{bd}T_{da}=\gamma.
$$

Thus all three are invariant under [rotations](../../riemannian-geometry.md#rotation-mathematics). They are $\operatorname{tr}T$, $\operatorname{tr}(T^2)$ and $\operatorname{tr}(T^3)$. For a real [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor), [orthogonal diagonalization](../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix) gives

$$
\alpha=\sum_i\lambda_i,\qquad\beta=\sum_i\lambda_i^2,\qquad\gamma=\sum_i\lambda_i^3.
$$

Expanding $\prod_i(\lambda-\lambda_i)$ and using [Newton's identities](../../polynomial.md#newton-s-identities) to recover the [characteristic polynomial from traces of powers](../../polynomial.md#characteristic-polynomial-from-traces-of-powers) yields

$$
\boxed{\lambda^3-\alpha\lambda^2+\frac{\alpha^2-\beta}{2}\lambda-\frac{\alpha^3-3\alpha\beta+2\gamma}{6}=0.}
$$

Comparison identifies $\boxed{c_2=-1,\qquad c_1=\tfrac12,\qquad c_0=-\tfrac16}$.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

Use the ordered displacement [vector](../../vector-space.md#vector) $q=(x_1,y_1,x_2,y_2,x_3,y_3,x_4,y_4)^T$, and define $K$ by $V=\tfrac12q^TKq$. For an unstretched [spring](../../elasticity-physics.md#spring), the extension to first order is the [dot product](../../inner-product.md#dot-product) of the relative [displacement](../../classical-mechanics.md#displacement) with its equilibrium [unit vector](../../vector-space.md#unit-vector). Summing its squared extensions gives the [central spring stiffness matrix](../../elasticity-physics.md#central-spring-stiffness-matrix). The four side [springs](../../elasticity-physics.md#spring) and two diagonal [springs](../../elasticity-physics.md#spring) give

$$
V=\frac k2\left[(x_1-x_2)^2+(y_1-y_3)^2+(y_2-y_4)^2+(x_3-x_4)^2+\frac{(x_4-x_1-y_4+y_1)^2}2+\frac{(x_3-x_2+y_3-y_2)^2}2\right].
$$

Therefore

$$
K=\frac k2\begin{pmatrix}
3&-1&-2&0&0&0&-1&1\\
-1&3&0&0&0&-2&1&-1\\
-2&0&3&1&-1&-1&0&0\\
0&0&1&3&-1&-1&0&-2\\
0&0&-1&-1&3&1&-2&0\\
0&-2&-1&-1&1&3&0&0\\
-1&1&0&0&-2&0&3&-1\\
1&-1&0&-2&0&0&-1&3
\end{pmatrix}.
$$

The [kinetic energy](../../energy.md#kinetic-energy) is $\tfrac m2\dot q^T\dot q$, so a [normal mode](../../wave-equation.md#normal-mode) satisfies $Kq=m\omega^2q$. Keeping the factor $1/2$ in the definition of $V$ fixes the normalization of $K$ and the resulting frequencies.

<a id="7/image-rigid-rotation-breathing-and-modes-with-reflection-symmetry"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2-square-spring-modes.png)

**[Figure 2](#7/image-rigid-rotation-breathing-and-modes-with-reflection-symmetry). Rigid rotation, breathing and modes with reflection symmetry**. Original displacement diagrams. Grey lines show all six equilibrium springs; arrows show representative mode vectors. The rotation has zero frequency, the breathing mode has squared frequency 4k/m, and the two other modes have squared frequency 2k/m.

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

The first two [vectors](../../vector-space.md#vector) displace every particle identically in the horizontal or vertical direction. Every relative [displacement](../../classical-mechanics.md#displacement) is zero, so every [spring](../../elasticity-physics.md#spring) has zero extension to first order. The third [vector](../../vector-space.md#vector) is $(y_i,-x_i)$ evaluated at the equilibrium points, which is an infinitesimal clockwise [rotation](../../riemannian-geometry.md#rotation-mathematics). For any edge the relative [displacement](../../classical-mechanics.md#displacement) is perpendicular to that edge, again giving zero extension.

These are the [rigid-motion zero modes of a spring framework](../../linear-operator-theory.md#rigid-motion-zero-modes-of-a-spring-framework): **two [translations](../../geometry-and-topology.md#translation-geometry) and one infinitesimal [rotation](../../riemannian-geometry.md#rotation-mathematics)**. Each has $Kq=0$, so $\boxed{\omega=0}$. In the linearized dynamics its amplitude has the form $A+Bt$, expressing free rigid motion rather than a restoring oscillation. Exact finite rigid [rotations](../../riemannian-geometry.md#rotation-mathematics) also preserve every [spring](../../elasticity-physics.md#spring) length; the mode [vector](../../vector-space.md#vector) is their first-order tangent.

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

In a [breathing mode](../../wave-equation.md#breathing-mode), each [displacement](../../classical-mechanics.md#displacement) is proportional to its equilibrium position. A representative [vector](../../vector-space.md#vector) is

$$
q_b=(-1,1,1,1,-1,-1,1,-1)^T.
$$

Multiplying by the [stiffness matrix](../../finite-element-method.md#stiffness-matrix) gives $Kq_b=4kq_b$. Thus

$$
\boxed{q\propto q_b,\qquad\omega^2=\frac{4k}m,\qquad\omega=2\sqrt{\frac km}.}
$$

Positive and negative amplitudes are uniform expansion and contraction about the center.

<h3 id="7/iii">iii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7/iii)

For the proposed [vector](../../vector-space.md#vector), the first horizontal component of $Kq$ is $-k(\alpha+\beta)/2$. Since the corresponding component of $q$ is zero, a [normal mode](../../wave-equation.md#normal-mode) requires $\beta=-\alpha$. The vertical components then give $Kq=2kq$. With an arbitrary nonzero overall amplitude, choose $\alpha=1$ to obtain

$$
\boxed{q_y=(0,1,0,-1,0,-1,0,1)^T,\qquad\omega=\sqrt{\frac{2k}m}.}
$$

The analogous pattern invariant under [reflection](../../linear-algebra.md#reflection-mathematics) across the vertical axis is

$$
\boxed{q_x=(1,0,-1,0,-1,0,1,0)^T,\qquad\omega=\sqrt{\frac{2k}m}.}
$$

Direct multiplication confirms $Kq_x=2kq_x$. The two patterns give independent [eigenvectors](../../linear-operator-theory.md#eigenvector) with the same [eigenvalue](../../linear-operator-theory.md#eigenvalue), as expected from the square's [rotation](../../riemannian-geometry.md#rotation-mathematics) symmetry.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

A [group](../../group.md) is a nonempty [set](../../set.md) with a closed [binary operation](../../algebraic-operation.md#binary-operation) that is [associative](../../algebraic-operation.md#associative-property), has an [identity element](../../algebraic-operation.md#identity-element), and gives every element an [inverse element](../../algebraic-operation.md#inverse-element). A [subgroup](../../group.md#subgroup) is a subset that is itself a [group](../../group.md) under the inherited operation. The left [coset](../../group-theory.md#coset) of $H$ represented by $g$ is $gH=\{gh:h\in H\}$; right [cosets](../../group-theory.md#coset) are defined analogously. Left [cosets](../../group-theory.md#coset) partition a finite [group](../../group.md), and $h\mapsto gh$ is a [bijection](../../function.md#bijection) from $H$ to $gH$. Therefore $|G|=[G:H]|H|$, proving [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) and the required divisibility.

For the given [matrices](../../vector-space.md#matrix), put $a=A$ and $c=AB=iI$. Since $B=iA$, the generators commute; $a^2=I$, $c^4=I$, and the generated elements are

$$
G=\{I,c,c^2,c^3,a,ca,c^2a,c^3a\},\qquad B=ca.
$$

They are distinct, and $(c^ra^s)(c^{r'}a^{s'})=c^{r+r'}a^{s+s'}$, with exponents reduced modulo four and two. The [Cayley table](../../algebraic-operation.md#cayley-table) is

$$
\begin{array}{c|cccccccc}
&I&c&c^2&c^3&a&ca&c^2a&c^3a\\\hline
I&I&c&c^2&c^3&a&ca&c^2a&c^3a\\
c&c&c^2&c^3&I&ca&c^2a&c^3a&a\\
c^2&c^2&c^3&I&c&c^2a&c^3a&a&ca\\
c^3&c^3&I&c&c^2&c^3a&a&ca&c^2a\\
a&a&ca&c^2a&c^3a&I&c&c^2&c^3\\
ca&ca&c^2a&c^3a&a&c&c^2&c^3&I\\
c^2a&c^2a&c^3a&a&ca&c^2&c^3&I&c\\
c^3a&c^3a&a&ca&c^2a&c^3&I&c&c^2\\
\end{array}
$$

The table proves closure and identifies $I$ as the identity. The [inverse element](../../algebraic-operation.md#inverse-element) of $c^ra^s$ is $c^{-r}a^s$, and [associativity](../../algebraic-operation.md#associative-property) follows from [matrix multiplication](../../vector-space.md#matrix-multiplication). Thus this is the [direct product of cyclic groups of orders four and two](../../group-theory.md#direct-product-of-cyclic-groups-of-orders-four-and-two), an [abelian group](../../group.md#abelian-group) of order eight.

Its [subgroups](../../group.md#subgroup) are exactly

$$
\{I\},\quad\{I,c^2\},\quad\{I,a\},\quad\{I,c^2a\},
$$



$$
\{I,c,c^2,c^3\},\quad\{I,ca,c^2,c^3a\},\quad\{I,c^2,a,c^2a\},\quad G.
$$

To see the list is complete, [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) leaves orders one, two, four and eight. There are exactly three elements of order two, giving the three order-two [subgroups](../../group.md#subgroup). An order-four [subgroup](../../group.md#subgroup) containing an element of order four must be one of the two [cyclic groups](../../group.md#cyclic-group) displayed; without such an element it must be the four-element set of elements whose squares are $I$. This is the enumeration in [subgroups of C4 times C2](../../group-theory.md#subgroups-of-c4-times-c2).

For example choose $H=\{I,c,c^2,c^3\}$. A complete set of [cosets](../../group-theory.md#coset) is $\boxed{H,\qquad aH=\{a,ca,c^2a,c^3a\}}$. Since $G$ is [Abelian](../../group.md#abelian-group), the left and right [cosets](../../group-theory.md#coset) coincide.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

A [group homomorphism](../../group-theory.md#group-homomorphism) $h:G\to F$ preserves multiplication: $h(g_1g_2)=h(g_1)h(g_2)$. It sends the [identity element](../../algebraic-operation.md#identity-element) to the identity and [inverse elements](../../algebraic-operation.md#inverse-element) to [inverse elements](../../algebraic-operation.md#inverse-element). Its [group kernel](../../group-theory.md#kernel-of-a-group-homomorphism) is $K=\{g\in G:h(g)=e_F\}$. This contains $e_G$ and is closed under multiplication and [inverse elements](../../algebraic-operation.md#inverse-element), so it is a [subgroup](../../group.md#subgroup). For $k\in K$ and $g\in G$,

$$
h(gkg^{-1})=h(g)e_Fh(g)^{-1}=e_F.
$$

Thus $gKg^{-1}\subseteq K$; applying the same argument with $g^{-1}$ gives equality. Hence **the [group kernel](../../group-theory.md#kernel-of-a-group-homomorphism) is a [normal subgroup](../../group-theory.md#normal-subgroup)**.

Let $S_2=\{e,\tau\}$ with $\tau=(12)$. The [parity of a permutation](../../finite-group-theory.md#parity-of-a-permutation) defines the desired map from $S_3$:

$$
\boxed{h(e)=h((123))=h((132))=e,\qquad h((12))=h((13))=h((23))=\tau.}
$$

The [sign of a permutation](../../finite-group-theory.md#sign-of-a-permutation) is multiplicative, so parity adds modulo two under composition, exactly matching $\tau^2=e$. Thus this is a [group homomorphism](../../group-theory.md#group-homomorphism); it is surjective because a transposition maps to $\tau$. Its [group kernel](../../group-theory.md#kernel-of-a-group-homomorphism) is

$$
\boxed{K=A_3=\{e,(123),(132)\}.}
$$

This is the [alternating group](../../finite-group-theory.md#alternating-group) on three objects, a [normal subgroup](../../group-theory.md#normal-subgroup) of index two in $S_3$.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

Write the [symmetry group of a square](../../finite-group-theory.md#symmetry-group-of-a-square) as $D_4=\langle r,s\mid r^4=s^2=e,\ srs=r^{-1}\rangle$, with $r$ a counterclockwise quarter-turn and $s$ [reflection](../../linear-algebra.md#reflection-mathematics) across the horizontal axis. The [conjugacy classes of the symmetry group of a square](../../finite-group-theory.md#conjugacy-classes-of-the-symmetry-group-of-a-square) are

$$
\boxed{\{e\},\qquad\{r^2\},\qquad\{r,r^3\},\qquad\{s,r^2s\},\qquad\{rs,r^3s\}.}
$$

Here $r^2$ is the half-turn and $r^3$ the clockwise quarter-turn. The two members of the fourth class reflect across the horizontal and vertical axes. Those of the fifth reflect across $y=x$ and $y=-x$. The identity and half-turn are [central elements](../../group-theory.md#central-element-of-a-group), giving singleton classes. The relations $srs=r^3$, $rsr^{-1}=r^2s$, and $r(rs)r^{-1}=r^3s$ show that each displayed pair consists of conjugate elements. More generally, conjugating $r^ks$ by $r$ changes $k$ to $k+2$, and conjugating by $s$ changes $k$ to $-k$; parity is preserved, so the two [reflection](../../linear-algebra.md#reflection-mathematics) pairs cannot merge.

In a [one-dimensional representation](../../representation-theory.md#one-dimensional-representation), the relation $srs=r^{-1}$ forces the image of $r$ to equal its inverse. Thus $r$ and $s$ can be assigned independent signs $\alpha,\beta\in\{1,-1\}$. These four choices give four [irreducible characters](../../representation-theory.md#irreducible-character). The ordinary two-dimensional action on the plane gives one more [character](../../representation-theory.md#character-of-a-representation): a [rotation](../../riemannian-geometry.md#rotation-mathematics) through $\theta$ has [trace](../../linear-algebra.md#matrix-trace) $2\cos\theta$, and a [reflection](../../linear-algebra.md#reflection-mathematics) has [trace](../../linear-algebra.md#matrix-trace) zero. Therefore the [character table of the symmetry group of a square](../../finite-group-theory.md#character-table-of-the-symmetry-group-of-a-square) is

$$
\begin{array}{c|rrrrr}
&e&r^2&\{r,r^3\}&\{s,r^2s\}&\{rs,r^3s\}\\\hline
\text{class size}&1&1&2&2&2\\\hline
A_1&1&1&1&1&1\\A_2&1&1&1&-1&-1\\B_1&1&1&-1&1&-1\\B_2&1&1&-1&-1&1\\E&2&-2&0&0&0
\end{array}.
$$

For instance the last row has squared character norm $(4+4)/8=1$, so the planar [representation](../../representation-theory.md#group-representation) is [irreducible](../../representation-theory.md#irreducible-representation); its inner product with each one-dimensional row is zero. All five rows obey [character orthogonality](../../representation-theory.md#character-orthogonality). Their squared dimensions sum to $1+1+1+1+4=8$, so they exhaust the [irreducible representations](../../representation-theory.md#irreducible-representation) of this order-eight [group](../../group.md).

## ↑ Ancestors (10)

1. [2003](../2003.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
