# Paper 2

↑ **Parent:** [2011](../2011.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2011/PaperNST_IB_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2011/PaperNST_IB_2.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)
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

For two real [eigenfunctions](../../linear-operator-theory.md#eigenfunction), multiply the equation for $y_n$ by $y_m$ and the equation for $y_m$ by $y_n$, then subtract. The $q$ terms cancel. The resulting [Lagrange identity for a Sturm-Liouville operator](../../sturm-liouville-theory.md#lagrange-identity-for-a-sturm-liouville-operator) is

$$
\left[p(y_my_n'-y_ny_m')\right]'+(\lambda_n-\lambda_m)r y_my_n=0.
$$

Integrating first over $[\epsilon,R]$ and then taking the endpoint limits gives

$$
(\lambda_n-\lambda_m)\int_0^\infty r y_my_n\,dx=-\left[p(y_my_n'-y_ny_m')\right]_0^\infty.
$$

The needed assumptions are that the [improper integral](../../real-analysis.md#improper-integral) exists and that the displayed boundary expression tends to zero at both endpoints. Bounded $y_m,y_n$ and their first [derivatives](../../calculus.md#derivative) are sufficient because $p\to0$, but are stronger than necessary. Merely knowing that $p\to0$ does not control arbitrarily growing [eigenfunctions](../../linear-operator-theory.md#eigenfunction). With the vanishing boundary form and distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue), division by $\lambda_n-\lambda_m$ proves [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions):

$$
\boxed{\int_0^\infty r(x)y_m(x)y_n(x)\,dx=0\quad(m\ne n).}
$$

For complex [eigenfunctions](../../linear-operator-theory.md#eigenfunction) in a real [self-adjoint differential operator](../../sturm-liouville-theory.md#self-adjoint-differential-operator) problem, use $\overline{y_m}$ instead, giving the corresponding [weighted inner product](../../inner-product.md#weighted-inner-product).

Multiplying the particular equation by $e^{-x}$ puts it in [Sturm-Liouville form](../../sturm-liouville-theory.md#sturm-liouville-form):

$$
(xe^{-x}y')'+\lambda e^{-x}y=0.
$$

Consequently

$$
\boxed{p(x)=xe^{-x},\qquad q(x)=0,\qquad r(x)=e^{-x}.}
$$

Its polynomial [eigenfunctions](../../linear-operator-theory.md#eigenfunction) are the [Laguerre polynomials](../../linear-operator-theory.md#laguerre-polynomial). Products of these [polynomials](../../polynomial.md), with or without one [derivative](../../calculus.md#derivative), grow only algebraically at infinity. The exponential in $p$ therefore makes the boundary form vanish there; its factor $x$ makes it vanish at zero. Their [orthogonality](../../inner-product.md#orthogonal-vectors) is thus

$$
\int_0^\infty e^{-x}y_m(x)y_n(x)\,dx=0\quad(m\ne n).
$$

For $\lambda=1$, substitution of $Ax+B$ gives $A+B=0$. For $\lambda=2$, substitution of $Ax^2+Bx+C$ gives $4A+B=0$ and $B+2C=0$. Choosing $y_n(0)=1$, which fixes the otherwise arbitrary nonzero multiplicative constants, yields

$$
\boxed{y_1=1-x,\qquad y_2=1-2x+\frac{x^2}{2}.}
$$

Their product is $1-3x+\tfrac52x^2-\tfrac12x^3$. Using the [Gamma function](../../complex-analysis.md#gamma-function) identity $\int_0^\infty x^ke^{-x}dx=k!$, also obtainable by repeated [integration by parts](../../calculus.md#integration-by-parts), verifies the required [orthogonality](../../inner-product.md#orthogonal-vectors) directly:

$$
\int_0^\infty e^{-x}y_1y_2\,dx=1-3(1!)+\frac52(2!)-\frac12(3!)=0.
$$

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Dirichlet uniqueness for the Poisson equation](../../analysis.md#dirichlet-uniqueness-for-the-poisson-equation) follows from a positive integral. Suppose $T_a,T_b$ satisfy the same data, and put $w=T_a-T_b$. Then $w$ is a [harmonic function](../../partial-differential-equation.md#harmonic-function) in $V$ and vanishes on $S$. [Green's first identity](../../partial-differential-equation.md#green-s-first-identity), applied with both arguments $w$, gives

$$
\int_V|\nabla w|^2dV=\int_Sw\,\partial_nw\,dS-\int_Vw\Delta w\,dV=0.
$$

Thus $\nabla w=0$, and $w$ is constant on the connected body. Its zero boundary value makes that constant zero. This proves **at most one temperature field**; it does not require an independent existence construction. As usual, the argument assumes a bounded body and sufficient regularity for [Green's first identity](../../partial-differential-equation.md#green-s-first-identity), or the corresponding finite-energy weak formulation.

For the composite body, let $w_-$ and $w_+$ be the differences in $V_1$ and $V_2$. They are [harmonic functions](../../partial-differential-equation.md#harmonic-function), have a common interface value $w$, and obey

$$
\alpha\partial_nw_+=\beta\partial_nw_-,\qquad w_+|_{S_2}=0.
$$

The [unit normal vector](../../differential-geometry.md#unit-normal) $n$ points out of $V_1$; the outward normal of $V_2$ on its inner boundary is $-n$. Keeping that sign in [Green's first identity](../../partial-differential-equation.md#green-s-first-identity) gives

$$
E_1:=\int_{V_1}|\nabla w_-|^2dV=\int_{S_1}w\,\partial_nw_-\,dS,
\qquad
E_2:=\int_{V_2}|\nabla w_+|^2dV=-\int_{S_1}w\,\partial_nw_+\,dS.
$$

The outer boundary term in $E_2$ is zero. Weight these equations by the positive coefficients that match the flux condition:

$$
\boxed{\beta E_1+\alpha E_2=\int_{S_1}w\left(\beta\partial_nw_--\alpha\partial_nw_+\right)dS=0.}
$$

Both [Dirichlet energies](../../differential-geometry.md#dirichlet-energy) must vanish. Hence both differences are constants; the outer data set the constant in $V_2$ to zero, and interface continuity sets the constant in $V_1$ to zero. This establishes [uniqueness for a harmonic transmission problem](../../analysis.md#uniqueness-for-a-harmonic-transmission-problem). Physically $\beta$ and $\alpha$ play the roles of the inner and outer [thermal conductivities](../../heat.md#thermal-conductivity); continuity of temperature and normal heat flux is what cancels the interface contribution.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $\rho=|\mathbf x-\mathbf y|$. A rotationally symmetric [fundamental solution of the Laplace equation](../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation) is [harmonic](../../partial-differential-equation.md#harmonic-function) for $\rho>0$. The [Laplace equation in polar coordinates](../../partial-differential-equation.md#laplace-equation-in-polar-coordinates) reduces to $(\rho G')'=0$, so $G=A\log\rho+B$. Integrate $-\Delta G=\delta^{(2)}(\mathbf x-\mathbf y)$ over a disk of radius $\epsilon$ around the source. The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives

$$
1=-\int_{\partial D_\epsilon}\partial_\rho G\,ds=-2\pi A.
$$

Taking $B=0$ therefore gives

$$
\boxed{G(\mathbf x,\mathbf y)=-\frac1{2\pi}\log|\mathbf x-\mathbf y|.}
$$

Changing the reference length inside the logarithm merely adds a constant. Notice the sign convention: the potential equation in this question is $\Delta V=q\delta^{(2)}$, whereas this [Green function](../../green-s-function.md) satisfies $-\Delta G=\delta^{(2)}$. Thus the point-source potential used below is $-qG=+(q/2\pi)\log\rho$.

For the two insulating walls, successive [Euclidean reflections](../../linear-algebra.md#reflection-mathematics) in $x=b$ and $x=-b$ generate sources of strength $q$ at $(2nb,0)$ for every [integer](../../integer.md) $n$. Only $n=0$ lies inside the physical strip. This is the [Neumann image lattice for a point source in a strip](../../mathematics.md#neumann-image-lattice-for-a-point-source-in-a-strip). Set

$$
r_n=\sqrt{(x-2nb)^2+y^2}.
$$

The raw sum of logarithmic potentials diverges by additive constants. A well-defined potential is obtained by pairing opposite images and subtracting their constant reference terms:

$$
\boxed{V(x,y)=\frac q{2\pi}\left[\log r_0+\sum_{n=1}^\infty\left(\log r_n+\log r_{-n}-2\log(2nb)\right)\right]+C.}
$$

Each paired summand is $O(n^{-2})$ on compact subsets away from the source. The [series](../../sequence-and-series.md#series-mathematics) therefore has local [uniform convergence](../../sequence-and-series.md#uniform-convergence), as do the required derivative series. It gives

$$
\boxed{\frac{\partial V}{\partial y}=\frac q{2\pi}\sum_{n\in\mathbb Z}\frac{y}{(x-2nb)^2+y^2}.}
$$

In the corresponding $x$-derivative, the images pair as $n$ and $1-n$ at $x=b$, and as $n$ and $-1-n$ at $x=-b$. Their opposite horizontal separations make the derivatives cancel. Thus both homogeneous [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition) hold. The constructed solution is even in $y$; without a condition at infinity the side conditions alone would allow further homogeneous [harmonic functions](../../partial-differential-equation.md#harmonic-function).

For fixed $y>0$, [uniform convergence](../../sequence-and-series.md#uniform-convergence) on $[-b,b]$ permits integration term by term. The $n$th term has integral

$$
\int_{-b}^b\frac{y\,dx}{(x-2nb)^2+y^2}=\arctan\frac{(2n+1)b}{y}-\arctan\frac{(2n-1)b}{y}.
$$

Here $\arctan$ is the ordinary real [inverse trigonometric function](../../geometry-and-topology.md#inverse-trigonometric-functions), taking values in $(-\pi/2,\pi/2)$. Summing from $-N$ to $N$ makes a [telescoping series](../../sequence-and-series.md#telescoping-series):

$$
\int_{-b}^b\partial_yV\,dx=\frac q{2\pi}\lim_{N\to\infty}2\arctan\frac{(2N+1)b}{y}=\boxed{\frac q2}.
$$

The source flux splits equally between the upper and lower parts of the strip. The next two parts give the single-wall constructions that underlie the image lattice.

<a id="3/image-equal-sign-image-sources-and-the-physical-strip-between-two-insulating-boundaries"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2-2011-ib-neumann-images.png)

**[Figure 1](#3/image-equal-sign-image-sources-and-the-physical-strip-between-two-insulating-boundaries). Equal-sign image sources and the physical strip between two insulating boundaries**.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For the grounded wall, use an image charge $-q$ at $(2b,0)$. Define the [Euclidean distances](../../topological-analysis.md#euclidean-distance) $r=\sqrt{x^2+y^2}$ and $r_* =\sqrt{(x-2b)^2+y^2}$. The [method of images](../../mathematics.md#method-of-images) gives

$$
\boxed{V_D(x,y)=\frac q{2\pi}\log\frac r{r_*},\qquad x<b.}
$$

The real source has the required [Dirac delta function](../../distribution-theory.md#dirac-delta-function) coefficient, and the image is outside the domain. On $x=b$, $r=r_*$, so $V_D=0$ exactly. This verifies the [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) rather than only its derivative.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For the insulating wall, the image instead has the same strength $q$. With the distances defined above,

$$
\boxed{V_N(x,y)=\frac q{2\pi}(\log r+\log r_*)+C,\qquad x<b.}
$$

It has the required source in the physical domain. Its normal [derivative](../../calculus.md#derivative) is

$$
\partial_xV_N=\frac q{2\pi}\left[\frac{x}{x^2+y^2}+\frac{x-2b}{(x-2b)^2+y^2}\right].
$$

At $x=b$ the terms are $b/(b^2+y^2)$ and $-b/(b^2+y^2)$, so they cancel. The [Neumann boundary condition](../../differential-equation.md#neumann-boundary-condition) leaves the additive constant $C$ free.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a positively oriented simple closed [contour](../../complex-analysis.md#complex-integration-contour) $C$, with no [pole](../../isolated-singularity.md#pole) on $C$ and with $f$ [holomorphic](../../holomorphic-function.md) inside except at finitely many poles, the [residue theorem](../../analysis.md#residue-theorem) states

$$
\oint_Cf(z)\,dz=2\pi i\sum_{z_j\text{ inside }C}\operatorname{Res}(f,z_j).
$$

For a more general closed contour, each [residue](../../analysis.md#residue) is multiplied by its [winding number](../../complex-analysis.md#winding-number) about the pole.

The powers must be defined using the same [branch of the complex logarithm](../../analysis.md#branch-of-the-complex-logarithm) as the numerator. A branch suitable for both requested calculations is

$$
\operatorname{Log}z=\log|z|+i\arg z,\qquad -\delta<\arg z<2\pi-\delta,
\quad 0<\delta<2\pi-\max\left(\pi,\frac{2\pi}{\beta}\right).
$$

The [branch cut](../../analysis.md#branch-cut) is a ray just below the positive real axis, and $z^\beta:=e^{\beta\operatorname{Log}z}$. Since $\beta>1$, the displayed choice of $\delta$ is possible. It includes the required upper half-plane and the sector used below. The origin remains an excluded [branch point](../../complex-analysis.md#branch-point).

In $0\leq\arg z<\pi$, all zeros of $1+z^\beta$ are

$$
\zeta_j=\exp\frac{(2j+1)\pi i}{\beta},\qquad j=0,1,\ldots,\quad 2j+1<\beta.
$$

Each is a [simple pole](../../isolated-singularity.md#simple-pole), since $\beta\zeta_j^{\beta-1}=-\beta/\zeta_j\ne0$. Its [residue](../../analysis.md#residue) is

$$
\boxed{\operatorname{Res}(f,\zeta_j)=-\frac{\zeta_j\operatorname{Log}\zeta_j}{\beta}=-\frac{i(2j+1)\pi}{\beta^2}\exp\frac{(2j+1)\pi i}{\beta}.}
$$

The strict inequality matters if a root lies on the negative real axis, which is outside the specified region.

To evaluate the two [improper integrals](../../real-analysis.md#improper-integral), write them as $I$ for the logarithmic numerator and $J$ for numerator one, and set $\theta=\pi/\beta$, $\alpha=2\theta$. Use a counterclockwise annular sector with $\epsilon<|z|<R$ and $0<\arg z<\alpha$. It encloses precisely $\zeta_0=e^{i\theta}$. The outward positive-axis segment contributes $I$ in the limit. On the inward segment $z=re^{i\alpha}$, the logarithm is $\log r+i\alpha$ and $z^\beta=r^\beta$, so that segment contributes $-e^{i\alpha}(I+i\alpha J)$.

The small arc is $O(\epsilon|\log\epsilon|)$, and the large arc is $O(R^{1-\beta}\log R)$; both vanish. These estimates follow from the arc lengths and $|1+z^\beta|\geq\big||z|^\beta-1\big|$. The real integrals also converge absolutely at both endpoints for $\beta>1$. The [residue theorem](../../analysis.md#residue-theorem) now gives

$$
(1-e^{2i\theta})I-2i\theta e^{2i\theta}J=2\theta^2e^{i\theta}.
$$

After division by $e^{i\theta}$, the real and imaginary parts are

$$
2\theta\sin\theta\,J=2\theta^2,\qquad -2\sin\theta\,I-2\theta\cos\theta\,J=0.
$$

Since $0<\theta<\pi$, $\sin\theta>0$. Hence the [logarithmic beta integral from a sector contour](../../analysis.md#logarithmic-beta-integral-from-a-sector-contour) yields

$$
\boxed{J=\frac{\pi}{\beta\sin(\pi/\beta)},\qquad I=-\frac{\pi^2\cos(\pi/\beta)}{\beta^2\sin^2(\pi/\beta)}.}
$$

For $1<\beta<2$ the sector angle exceeds $\pi$. This is why choosing the [principal complex logarithm](../../analysis.md#principal-complex-logarithm) on the whole sector would be invalid; the displaced cut above handles that range as well as $\beta\geq2$.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

First prove the [convolution theorem](../../fourier-analysis.md#convolution-theorem) with the stated negative-exponential [Fourier transform](../../fourier-transform.md). Assuming absolute integrability sufficient for [Fubini's theorem](../../measure-theory.md#fubini-s-theorem), change variables $u=t-s$:

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikt}f(s)g(t-s)\,ds\,dt\\
&=\int_{\mathbb R}f(s)e^{-iks}ds\int_{\mathbb R}g(u)e^{-iku}du
=\widetilde f(k)\widetilde g(k).
\end{aligned}
$$

For the differential equation, [integration by parts](../../calculus.md#integration-by-parts) gives

$$
\widetilde {y'}=[e^{-ikt}y]_{-\infty}^\infty+ik\widetilde y=ik\widetilde y,
\qquad \widetilde {y''}=ik\widetilde {y'}=-k^2\widetilde y.
$$

The boundary terms vanish by the assumed decay of $y,y'$. As with the convolution step, the transforms can first be justified for integrable functions and derivatives; the resulting kernel gives the desired decaying response. Thus

$$
\boxed{\widetilde y(k)=\frac{\widetilde f(k)}{(a+ik)(b+ik)}=\widetilde f(k)\widetilde G(k).}
$$

The [convolution theorem](../../fourier-analysis.md#convolution-theorem) and [Fourier inversion theorem](../../fourier-analysis.md#fourier-inversion-theorem) imply $y=f*G$.

For the inverse transform of $\widetilde G$, use

$$
\widetilde G(k)=\frac1{a-b}\left(\frac1{b+ik}-\frac1{a+ik}\right).
$$

The [poles](../../isolated-singularity.md#pole) are at $ib,ia$. For $t>0$, close the inverse-transform contour above; the residues of $e^{ikt}\widetilde G(k)$ there are $-ie^{-bt}/(a-b)$ and $ie^{-at}/(a-b)$. The inverse-transform factor $1/(2\pi)$ makes the answer $i$ times their sum. For $t<0$, close below, enclosing no poles. The large arcs vanish: the complete rational factor is $O(|k|^{-2})$ and the exponential is bounded on the appropriate semicircle. Therefore the [causal Green function of an overdamped oscillator](../../analysis.md#causal-green-function-of-an-overdamped-oscillator) is

$$
\boxed{G(t)=\begin{cases}0,&t<0,\\(e^{-bt}-e^{-at})/(a-b),&t\geq0.\end{cases}}
$$

It is continuous, with $G(0)=0$ and $G'(0^+)=1$, so $(D_t+a)(D_t+b)G=\delta(t)$. The response can also be written $y(t)=\int_{-\infty}^tG(t-s)f(s)ds$.

For the bilateral exponential forcing, split the real [integral](../../integral.md) at zero:

$$
\widetilde f(k)=\int_{-\infty}^0e^{(1-ik)t}dt+\int_0^\infty e^{-(1+ik)t}dt
=\frac1{1-ik}+\frac1{1+ik}=\boxed{\frac2{1+k^2}}.
$$

Consequently

$$
\boxed{\widetilde y(k)=\frac2{(1+k^2)(a+ik)(b+ik)}.}
$$

For negative time the lower half-plane contains only $k=-i$. The [residue](../../analysis.md#residue) of $e^{ikt}\widetilde y$ there is $ie^t/[(a+1)(b+1)]$. Clockwise closure makes the inverse transform $-i$ times that residue. For positive time the three upper [residues](../../analysis.md#residue), at $i,ia,ib$ respectively, are

$$
-\frac{ie^{-t}}{(a-1)(b-1)},\qquad
-\frac{2ie^{-at}}{(a^2-1)(a-b)},\qquad
\frac{2ie^{-bt}}{(b^2-1)(a-b)}.
$$

Multiplication of their sum by $i$ gives the [bilateral exponential forcing of an overdamped oscillator](../../analysis.md#bilateral-exponential-forcing-of-an-overdamped-oscillator):

$$
\boxed{y(t)=\begin{cases}
\dfrac{e^t}{(a+1)(b+1)},&t\leq0,\\
\dfrac{e^{-t}}{(a-1)(b-1)}+\dfrac2{a-b}\left(\dfrac{e^{-at}}{a^2-1}-\dfrac{e^{-bt}}{b^2-1}\right),&t\geq0.
\end{cases}}
$$

Both expressions have $y(0)=y'(0)=1/[(a+1)(b+1)]$. This verifies the matching that prevents an extra [Dirac delta function](../../distribution-theory.md#dirac-delta-function) at zero. Direct substitution gives the forcing on either side, and all terms decay at their corresponding infinities. A causal [Green function](../../green-s-function.md) does not imply zero response before $t=0$ when the forcing has already been acting at negative times. The assumptions $a,b\ne1$ avoid repeated poles; their limiting cases would contain polynomial times exponential terms.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Let $Q$ be the [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix) taking old components to new ones, so $x'_i=Q_{ip}x_p$. With repeated indices summed, the [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law) is

$$
\boxed{t'_{ij}=Q_{ip}Q_{jq}t_{pq},\qquad u'_{ijkl}=Q_{ip}Q_{jq}Q_{kr}Q_{ls}u_{pqrs}.}
$$

An [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor) has the same components after every proper [rotation](../../riemannian-geometry.md#rotation-mathematics). Since $Q_{ip}Q_{jp}=\delta_{ij}$, the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta) is invariant. Applying this identity to each factor shows that $a\delta_{ij}$ and every linear combination $b\delta_{ij}\delta_{kl}+c\delta_{ik}\delta_{jl}+d\delta_{il}\delta_{jk}$ are invariant as well.

To show that an [isotropic second-rank tensor](../../multilinear-algebra.md#isotropic-second-rank-tensor) must be scalar, start with any matrix $t$, without assuming symmetry. Invariance under quarter-turns about axes 1 and 2 implies invariance under their squares, the half-turns

$$
Q_1^2=\operatorname{diag}(1,-1,-1),\qquad Q_2^2=\operatorname{diag}(-1,1,-1).
$$

The first forces $t_{12},t_{21},t_{13},t_{31}$ to vanish. The second also forces $t_{23},t_{32}$ to vanish. The matrix is therefore diagonal. A quarter-turn about axis 1 interchanges its 22 and 33 entries; one about axis 2 interchanges its 11 and 33 entries. All three must agree, giving $t=aI$.

A [rotation](../../riemannian-geometry.md#rotation-mathematics) preserves the ball $V_R$, $|x|^2$ and the [volume element](../../integral.md#volume-element). Changing integration variables by that rotation shows that $A$ and $B$ are [isotropic tensors](../../multilinear-algebra.md#isotropic-tensor). Write $A_{ij}=a\delta_{ij}$. Taking its [tensor contraction](../../multilinear-algebra.md#tensor-contraction) gives

$$
3a=A_{ii}=\int_{V_R}|x|^4dV=4\pi\int_0^Rr^6dr=\frac{4\pi R^7}{7},
$$

so $a=4\pi R^7/21$. Every permutation of the indices of $B$ leaves its integrand unchanged. Its complete symmetry therefore makes all three isotropic coefficients equal, say $d$:

$$
B_{ijkl}=d(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

Double contraction gives $15d=B_{iikk}=\int_{V_R}|x|^4dV=4\pi R^7/7$. Thus the [isotropic fourth moment of a ball](../../multilinear-algebra.md#isotropic-fourth-moment-of-a-ball) and its radial contraction are

$$
\boxed{A_{ij}=\frac{4\pi R^7}{21}\delta_{ij},\qquad
B_{ijkl}=\frac{4\pi R^7}{105}(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).}
$$

Put $d=4\pi R^7/105$, so that $a=5d$. Contract $B$ with the prescribed [unit vector](../../vector-space.md#unit-vector) twice:

$$
C_{ij}=A_{ij}+B_{ijkl}n_kn_l=d(6\delta_{ij}+2n_in_j).
$$

This has the [spectrum of a scalar matrix plus a rank-one projector](../../linear-algebra.md#spectrum-of-a-scalar-matrix-plus-a-rank-one-projector). In the direction $n$, the [outer product](../../vector-space.md#outer-product) $nn^T$ acts as the identity; on the plane perpendicular to $n$, it acts as zero. Therefore

$$
\boxed{Cn=\frac{32\pi R^7}{105}n,\qquad Cv=\frac{8\pi R^7}{35}v\quad\text{for }v\cdot n=0.}
$$

Any nonzero multiple of $n$ is a parallel [eigenvector](../../linear-operator-theory.md#eigenvector), and any nonzero vector in the perpendicular plane is a transverse [eigenvector](../../linear-operator-theory.md#eigenvector). The transverse [eigenvalue](../../linear-operator-theory.md#eigenvalue) has multiplicity two; an [orthonormal basis](../../inner-product.md#orthonormal-basis) of that plane completes a set of principal axes.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

The [Lagrangian](../../calculus-of-variations.md#lagrangian) is $\mathcal L=T-\mathcal V$, and the [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) are

$$
\frac d{dt}\frac{\partial\mathcal L}{\partial\dot q_i}-\frac{\partial\mathcal L}{\partial q_i}=0.
$$

At a rest [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) $q=0$, $\partial_i\mathcal V(0)=0$ for all three coordinates. The [Taylor expansion](../../calculus.md#taylor-expansion) therefore starts as

$$
\mathcal V(q)=\mathcal V(0)+\frac12\sum_{ij}q_i\left.\frac{\partial^2\mathcal V}{\partial q_i\partial q_j}\right|_0q_j+O(|q|^3).
$$

The symmetric [Hessian matrix](../../multivariable-calculus.md#hessian-matrix) is the matrix $\mathsf V$ of the quadratic [potential energy](../../energy.md#potential-energy). If a quadratic coefficient vanishes along a direction, higher-order terms can be the first nonconstant terms there; equilibrium by itself does not imply strict stability.

Write $\mathsf T_0=\mathsf T(0)$. Terms involving the variation of $\mathsf T(q)$ are cubic in small displacements and velocities, so the quadratic [small oscillation](../../lagrangian-mechanics.md#small-oscillation) Lagrangian is

$$
\mathcal L_2=\frac12\dot q^T\mathsf T_0\dot q-\frac12q^T\mathsf Vq,
\qquad \mathsf T_0\ddot q+\mathsf Vq=0.
$$

A [normal mode](../../wave-equation.md#normal-mode) has fixed displacement ratios, $q(t)=v\cos(\omega t+\phi)$. Its [angular frequency](../../lagrangian-mechanics.md#angular-frequency) $\omega$ is an [eigenfrequency](../../wave-equation.md#eigenfrequency), or normal frequency, and satisfies the [generalized eigenvalue problem for small oscillations](../../lagrangian-mechanics.md#generalized-eigenvalue-problem-for-small-oscillations)

$$
\mathsf Vv=\omega^2\mathsf T_0v,\qquad \det(\mathsf V-\omega^2\mathsf T_0)=0.
$$

Here $\mathsf T_0$ is positive definite for independent physical coordinates and positive masses. A stable quadratic minimum makes $\omega^2\geq0$; a negative value would describe exponential instability rather than oscillation.

For the suspended bar, let $\kappa_0$ and $\kappa_1$ denote the actual incremental [spring constants](../../elasticity-physics.md#spring-constant) of the upper and each lower [spring](../../elasticity-physics.md#spring). The physical displacement of the bar is $q_1$, while the lower spring extensions change by $q_2-q_1$ and $q_3-q_1$. Consequently

$$
T=\frac12\left(M\dot q_1^2+m\dot q_2^2+m\dot q_3^2\right),\quad
\mathcal V_2=\frac12\kappa_0q_1^2+\frac12\kappa_1\left[(q_2-q_1)^2+(q_3-q_1)^2\right].
$$

The linear gravitational and elastic terms cancel at the loaded [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). Expanding the remaining squares gives the [small-oscillation mass and stiffness matrices](../../lagrangian-mechanics.md#small-oscillation-mass-and-stiffness-matrices)

$$
\mathsf T_0=\begin{pmatrix}M&0&0\\0&m&0\\0&0&m\end{pmatrix},\qquad
\mathsf V=\begin{pmatrix}\kappa_0+2\kappa_1&-\kappa_1&-\kappa_1\\-\kappa_1&\kappa_1&0\\-\kappa_1&0&\kappa_1\end{pmatrix}.
$$

Thus

$$
\boxed{\mathcal L_2=\frac12\left[M\dot q_1^2+m\dot q_2^2+m\dot q_3^2-\kappa_0q_1^2-\kappa_1(q_2-q_1)^2-\kappa_1(q_3-q_1)^2\right].}
$$

**Source convention:** the printed matrix is obtained by setting $\kappa_0=\lambda/L$ and $\kappa_1=\mu/l$. Although the PDF prose calls $\lambda,\mu$ spring constants, that matrix treats them as elastic parameters whose ratios to the stated lengths are the incremental stiffnesses. If they are read literally as Hooke-law [spring constants](../../elasticity-physics.md#spring-constant), the divisions by $L,l$ should instead be omitted. The numerical case has $L=l=1$, so this discrepancy does not affect its results.

With the numerical parameters, $\mathsf T_0=\operatorname{diag}(2,1,1)$ and

$$
\mathsf V=\begin{pmatrix}6&-1&-1\\-1&1&0\\-1&0&1\end{pmatrix}.
$$

Use the exchange symmetry of the lower masses to find the [vertical modes of a horizontally constrained suspended bar](../../lagrangian-mechanics.md#vertical-modes-of-a-horizontally-constrained-suspended-bar). The antisymmetric vector $v_a=(0,1,-1)^T$ obeys $\mathsf Vv_a=\mathsf T_0v_a$, giving $\omega_a=1$. In the symmetric sector put $v=(A,B,B)^T$ and $s=\omega^2$. The two independent equations are

$$
(6-2s)A-2B=0,\qquad -A+(1-s)B=0.
$$

Their determinant gives $s^2-4s+2=0$, so $s=2\pm\sqrt2$. Taking $A=1$, the full set is

$$
\boxed{\begin{array}{c|c}
\text{angular frequency}&\text{relative displacements }(q_1,q_2,q_3)\\\hline
\sqrt{2-\sqrt2}&(1,1+\sqrt2,1+\sqrt2)\\
1&(0,1,-1)\\
\sqrt{2+\sqrt2}&(1,1-\sqrt2,1-\sqrt2)
\end{array}.}
$$

In the lowest [normal mode](../../wave-equation.md#normal-mode), all three masses move in phase, with the lower masses moving about $2.414$ times as far as the bar. In the antisymmetric [normal mode](../../wave-equation.md#normal-mode), the bar stays still and the lower masses move equally in opposite directions; their changing forces on the bar cancel. In the highest [normal mode](../../wave-equation.md#normal-mode), the lower masses move together against the bar, with magnitude about $0.414$ of its displacement. Any small motion is a superposition of these three modes.

<a id="7/image-relative-vertical-displacements-in-the-three-normal-modes-with-the-bar-constrained-to-remain-horizontal"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2-2011-ib-suspended-bar-modes.png)

**[Figure 2](#7/image-relative-vertical-displacements-in-the-three-normal-modes-with-the-bar-constrained-to-remain-horizontal). Relative vertical displacements in the three normal modes, with the bar constrained to remain horizontal**.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

The [group order](../../group.md#order-of-a-finite-group) of a finite [group](../../group.md) is its number of elements, $|G|$. The [order of a group element](../../group-theory.md#order-of-a-group-element) $g$ is the least positive [integer](../../integer.md) $r$ with $g^r=e$. Such an $r$ exists in a finite group because two powers must coincide, and cancellation then gives a positive power equal to the [identity element](../../algebraic-operation.md#identity-element).

For the [direct product of groups](../../group-theory.md#direct-product-of-groups), the componentwise operation is closed because each factor is closed. [Associativity](../../algebraic-operation.md#associative-property) holds in each coordinate:

$$
[(g,h)(g',h')](g'',h'')=(gg'g'',hh'h'')=(g,h)[(g',h')(g'',h'')].
$$

The [identity element](../../algebraic-operation.md#identity-element) is $(e_1,e_2)$, and the [inverse element](../../algebraic-operation.md#inverse-element) of $(g,h)$ is $(g^{-1},h^{-1})$. Thus all [group axioms](../../group.md#group-axioms) hold. For finite factors, the [multiplication principle](../../combinatorics.md#rule-of-product) gives

$$
\boxed{|G_1\times G_2|=|G_1||G_2|.}
$$

For $\mathbb Z_2\times\mathbb Z_2$, write $E=(e,e)$, $u=(w,e)$, $v=(e,w)$, $z=(w,w)$, with $w^2=e$. Its [Cayley table](../../algebraic-operation.md#cayley-table), with the row element multiplying the column element, is

$$
\begin{array}{c|cccc}
 &E&u&v&z\\\hline
E&E&u&v&z\\
u&u&E&z&v\\
v&v&z&E&u\\
z&z&v&u&E
\end{array}.
$$

This is the [Klein four-group](../../finite-group-theory.md#klein-four-group): every nonidentity element has order two.

In the [cyclic group](../../group.md#cyclic-group) $\mathbb Z_4=\langle a\rangle$, the set $\{e,a^2\}$ is closed because $(a^2)^2=e$, and both elements have inverses in the set. It is therefore a proper [subgroup](../../group.md#subgroup) of order two. By [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem), a proper subgroup has order one or two. An order-two subgroup must be generated by an element of order two. Neither $a$ nor $a^3$ has order two, whereas $a^2$ does. Hence

$$
\boxed{\text{the proper subgroups of }\mathbb Z_4\text{ are }\{e\}\text{ and }\{e,a^2\}.}
$$

**The PDF's claim needs “nontrivial”:** $\{e,a^2\}$ is the only nontrivial proper subgroup, but $\{e\}$ is also a proper subgroup under the usual definition.

A [group isomorphism](../../algebra.md#group-isomorphism) preserves element orders: $\phi(g)^r=e$ if and only if $g^r=e$, using the homomorphism property and injectivity. Since $\mathbb Z_4$ has elements of order four and the [Klein four-group](../../finite-group-theory.md#klein-four-group) does not,

$$
\boxed{\mathbb Z_2\times\mathbb Z_2\not\cong\mathbb Z_4.}
$$

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

The [intersection](../../set.md#set-intersection) $H\cap K$ contains the [identity element](../../algebraic-operation.md#identity-element). If $a,b\in H\cap K$, then $ab^{-1}$ belongs to both $H$ and $K$, so it belongs to their intersection. The [subgroup test](../../group.md#subgroup-test) proves that $H\cap K$ is a [subgroup](../../group.md#subgroup) of $G$, with the inherited operation. Explicitly, closure and inverses come from this test, and [associativity](../../algebraic-operation.md#associative-property) is inherited from $G$.

Label the vertices of the [equilateral triangle](../../euclidean-geometry.md#equilateral-triangle) $1,2,3$ counterclockwise. For the [dihedral group](../../finite-group-theory.md#dihedral-group) of order six, let $r=(123)$ be the counterclockwise rotation by $120^\circ$, and let $s=(23)$ be reflection in the line through vertex 1 and the opposite side's midpoint. Choose

$$
I=e,\quad A=r,\quad B=r^2,\quad C=s,\quad D=rs,\quad E=r^2s.
$$

Then $B$ rotates by $240^\circ$. The three [Euclidean reflections](../../linear-algebra.md#reflection-mathematics) $C,D,E$ fix vertices $1,3,2$ respectively. Products act on a vertex from right to left. The relations $r^3=s^2=e$ and $sr=r^{-1}s$ give

$$
(r^is^\epsilon)(r^js^\eta)=r^{\,i+(-1)^\epsilon j}s^{\epsilon+\eta},
$$

where exponents of $r$ are reduced modulo three and those of $s$ modulo two. This constructs the entire [Cayley table](../../algebraic-operation.md#cayley-table):

$$
\begin{array}{c|cccccc}
 &I&A&B&C&D&E\\\hline
I&I&A&B&C&D&E\\
A&A&B&I&D&E&C\\
B&B&I&A&E&C&D\\
C&C&E&D&I&B&A\\
D&D&C&E&A&I&B\\
E&E&D&C&B&A&I
\end{array}.
$$

For example $AC=D$ whereas $CA=E$, so the group is **nonabelian**.

A subgroup of order two is generated by its unique nonidentity element, which must have order two. The rotations $A,B$ have order three, and each reflection has order two. Thus there are exactly

$$
\boxed{\langle C\rangle=\{I,C\},\qquad\langle D\rangle=\{I,D\},\qquad\langle E\rangle=\{I,E\}.}
$$

None is a [normal subgroup](../../group-theory.md#normal-subgroup). Conjugation by $A$ sends the reflection $r^js$ to $r^{j+2}s$, cycling the three reflections. For example $ACA^{-1}=E\notin\langle C\rangle$. Each of the other two subgroups fails the same conjugation test.

Finally, take two distinct such subgroups. For instance their [union](../../set.md#set-union) is $\langle C\rangle\cup\langle D\rangle=\{I,C,D\}$, but $CD=B$ lies outside it. Thus it is **not closed under the inherited group operation** and is not a [group](../../group.md). The distinctness is necessary: the union of a subgroup with itself is that subgroup.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

A [group homomorphism](../../group-theory.md#group-homomorphism) $D:G_1\to G_2$ satisfies $D(gh)=D(g)D(h)$ for all $g,h\in G_1$. Its [group kernel](../../group-theory.md#kernel-of-a-group-homomorphism) is

$$
\ker D=\{g\in G_1:D(g)=e_{G_2}\}.
$$

For the matrices, put $X=R(x)$, $Y=R(y)$ and $z=e^{2\pi i/3}$. Since $z^3=1$, $z\ne1$ and $1+z+z^2=0$, direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives

$$
X^2=I_2,\qquad Y^2=\begin{pmatrix}z^2&0\\0&z\end{pmatrix},\qquad Y^3=I_2,
$$



$$
XY=\begin{pmatrix}0&z^2\\z&0\end{pmatrix},\qquad
XY^2=\begin{pmatrix}0&z\\z^2&0\end{pmatrix}=YX,\qquad
Y^2X=XY.
$$

These verify the listed matrices and the defining relations, with $R(e)=I_2$. To check every product explicitly through a single calculation, write elements in the unique form $x^\epsilon y^j$, with $\epsilon=0,1$ and $j=0,1,2$. The relations give

$$
(x^\epsilon y^j)(x^\eta y^k)=x^{\epsilon+\eta}y^{(-1)^\eta j+k}.
$$

The displayed matrices obey $Y^jX=XY^{-j}$, so their product has exactly the same form:

$$
(X^\epsilon Y^j)(X^\eta Y^k)=X^{\epsilon+\eta}Y^{(-1)^\eta j+k}=R\big((x^\epsilon y^j)(x^\eta y^k)\big).
$$

All exponents are reduced modulo two or three respectively. Thus this verifies all 36 products, and $R$ is a two-dimensional complex [group representation](../../representation-theory.md#group-representation). It is given to be an [irreducible representation](../../representation-theory.md#irreducible-representation).

For a one-dimensional complex [group representation](../../representation-theory.md#group-representation) $U$, let $u=U(x)$ and $v=U(y)$, which are nonzero complex numbers. The relations require

$$
u^2=1,\qquad v^3=1,\qquad vu=uv^2.
$$

Since scalar multiplication commutes and $u\ne0$, the last relation gives $v=v^2$, hence $v=1$. Then $u=\pm1$. The choice $u=1$ is the [trivial representation](../../representation-theory.md#trivial-representation); the unique nontrivial choice is the [sign representation](../../representation-theory-of-the-symmetric-group.md#sign-representation):

$$
\boxed{U(e)=U(y)=U(y^2)=1,\qquad U(x)=U(xy)=U(xy^2)=-1.}
$$

Its [group kernel](../../group-theory.md#kernel-of-a-group-homomorphism) is

$$
\boxed{\ker U=\{e,y,y^2\}.}
$$

A [faithful representation](../../representation-theory.md#faithful-representation) is injective and has trivial kernel. Here the kernel has three elements, so **$U$ is not faithful**.

Both one-dimensional representations are [irreducible representations](../../representation-theory.md#irreducible-representation), and they are inequivalent to each other and to the given two-dimensional one. The [sum of squares of irreducible representation dimensions](../../representation-theory.md#sum-of-squares-of-irreducible-representation-dimensions) gives

$$
1^2+1^2+2^2=6=|S_3|.
$$

These exhaust all complex [irreducible representations](../../representation-theory.md#irreducible-representation). Their number equals the number of [conjugacy classes](../../group-action.md#conjugacy-class), so there are **three conjugacy classes**. Explicitly they are

$$
\boxed{\{e\},\qquad\{y,y^2\},\qquad\{x,xy,xy^2\}.}
$$

The last two sets consist of the 3-cycles and transpositions respectively.

## ↑ Ancestors (10)

1. [2011](../2011.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
