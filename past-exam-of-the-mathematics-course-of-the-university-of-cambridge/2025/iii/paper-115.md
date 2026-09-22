# Paper 115

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20115.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20115.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A smooth map $i:N\to M$ is a [smooth embedding](../../../differential-geometry.md#smooth-embedding) when it is an injective [immersion](../../../differential-geometry.md#immersion) and a homeomorphism onto its image with the subspace topology. The unit sphere is the inverse image of the regular value $1$ under $x\mapsto|x|^2$, so the [preimage theorem](../../../differential-geometry.md#preimage-theorem) makes it a smooth submanifold of $\mathbb R^{n+1}$ and its inclusion an immersion. It is injective, and a continuous injection from the compact sphere into the Hausdorff Euclidean space is a homeomorphism onto its image. Thus the inclusion is an embedding.

Products of spheres can be embedded by iterated spinning. Start with a round $S^{n_1}\subset\mathbb R^{n_1+1}$ translated into the half-space whose last coordinate $r$ is positive. If a compact $m$-manifold $N$ is embedded by

$$
x\longmapsto(y(x),r(x))\in\mathbb R^m\times(0,\infty),
$$

then

$$
N\times S^q\longrightarrow\mathbb R^m\times\mathbb R^{q+1},
\qquad(x,u)\longmapsto(y(x),r(x)u)
$$

is an injective immersion; compactness again makes it an embedding. Iterating with $q=n_2,\ldots,n_k$ embeds $S^{n_1}\times\cdots\times S^{n_k}$ in $\mathbb R^{n+1}$, where $n=\sum_i n_i$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) is

$$
H^p_{\mathrm{dR}}(M)=\ker(d:\Omega^p\to\Omega^{p+1})/operatorname{im}(d:\Omega^{p-1}\to\Omega^p).
$$

The [Poincaré lemma](../../../differential-form.md#poincare-lemma) says that every closed positive-degree differential form is locally exact, and is exact on every star-shaped open subset of Euclidean space.

Let $n>1$ and let $\alpha$ be a closed one-form on $M$. The hypothesis gives $\alpha=dg$ on $M\setminus B$. Choose a slightly larger coordinate ball $B'$ around $B$. The Poincare lemma gives $\alpha=dh$ on $B'$. The annulus $B'\setminus B$ is connected when $n>1$, so $d(g-h)=0$ there and $g-h$ is constant. Adjusting $h$ by this constant makes $g$ and $h$ agree on the overlap, and they glue to a global primitive of $\alpha$. Hence $H^1(M)=0$. For $n=1$ the claim fails: remove a closed proper interval from $S^1$. Its complement is an interval and has vanishing first de Rham cohomology, whereas $H^1(S^1)\cong\mathbb R$.

Finally choose a nowhere-vanishing $n$-form $\omega$ on $S^n$ and a coordinate $t$ on the finite interval $I$. Every $(n+1)$-form on $S^n\times I$ is $a(x,t)\omega\wedge dt$. Fix $t_0\in I$ and put

$$
A(x,t)=\int_{t_0}^t a(x,s)\,ds.
$$

Since $d_{S^n}A\wedge\omega=0$ for dimensional reasons,

$$
d((-1)^nA\omega)=a\omega\wedge dt.
$$

Every top-degree form is exact, so $H^{n+1}(S^n\times I)=0$ without using the de Rham theorem.

## 2

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms) is the alternating tensor product

$$
(\alpha\wedge\beta)(v_1,\ldots,v_{p+q})
=\frac1{p!q!}\sum_{\sigma\in S_{p+q}}\operatorname{sgn}(\sigma)
\alpha(v_{\sigma(1)},\ldots,v_{\sigma(p)})
\beta(v_{\sigma(p+1)},\ldots,v_{\sigma(p+q)}).
$$

For nonzero $\eta\in\Lambda^{n-1}((\mathbb R^n)^*)$, choose a volume form $\mu$. There is a nonzero vector $v$ with $\eta=\iota_v\mu$. Extend $v$ to a basis and use its dual coframe; then $\eta$ is a scalar multiple of $e^2\wedge\cdots\wedge e^n$, hence equals $\xi\wedge\eta_0$. The zero form is immediate.

To integrate a top form on a compact oriented $n$-manifold, choose a finite oriented atlas and a subordinate [partition of unity](../../../differential-geometry.md#partition-of-unity); integrate each compactly supported coordinate expression and sum. A smooth map pulls forms back by

$$
(\phi^*\alpha)_x(v_1,\ldots,v_p)=
\alpha_{\phi(x)}(d\phi_xv_1,\ldots,d\phi_xv_p).
$$

If $F^*\omega=\omega$ for a nowhere-zero top form, $F$ preserves its orientation. The change-of-variables theorem gives

$$
\boxed{\int_M(h\circ F)\omega
=\int_MF^*(h\omega)
=\int_Mh\omega.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The metric on covectors is induced by the inverse matrix $g^{-1}$, and on $p$-forms by the determinant pairing

$$
\langle\alpha_1\wedge\cdots\wedge\alpha_p,
\beta_1\wedge\cdots\wedge\beta_p\rangle
=\det(\langle\alpha_i,\beta_j\rangle).
$$

The [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) is the unique positive top form taking value one on every oriented orthonormal frame. The [Hodge star operator](../../../differential-form.md#hodge-star-operator) is uniquely determined by

$$
\beta\wedge *\alpha=\langle\beta,\alpha\rangle\omega_g.
$$

Nondegeneracy of the wedge pairing proves existence and uniqueness pointwise, and the smooth metric dependence makes $*$ a well-defined smooth bundle map.

On compactly supported forms, [Stokes theorem](../../../calculus.md#stokes-theorem) and the graded Leibniz rule give

$$
\delta|_{\Omega^p}=(-1)^{m(p+1)+1}*d*,
$$

where $m=\dim M$; this is the formal $L^2$ adjoint of $d$. The Hodge [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) is

$$
\Delta=d\delta+\delta d.
$$

For $g_f=e^{2f}g$, the covector metric scales by $e^{-2f}$, the $p$-form metric by $e^{-2pf}$, and the volume form by $e^{mf}$. Therefore

$$
*_f\alpha=e^{(m-2p)f}*\alpha.
$$

If $f$ is constant, the two star factors in the codifferential contribute $e^{-2f}$, so $\delta_f=e^{-2f}\delta$. Since $d$ is metric-independent,

$$
\boxed{\Delta_f\alpha=e^{-2f}\Delta\alpha.}
$$

## 3

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

If $E$ has local frame transition matrices $g_{ab}$ and the cotangent bundle has transitions $J_{ab}^{-T}$, then $E\otimes\Lambda^rT^*B$ has local trivializations with transitions

$$
g_{ab}\otimes\Lambda^r(J_{ab}^{-T}),
$$

which satisfy the cocycle condition. Thus it is a well-defined [tensor product of vector bundles](../../../fiber-bundle.md#tensor-product-of-vector-bundles).

A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) is a linear map

$$
\nabla:\Gamma(E)\to\Omega^1(B;E)
$$

satisfying $\nabla(fs)=df\otimes s+f\nabla s$. Contracting with a vector field gives the covariant derivative $\nabla_Xs$. In a local frame, $\nabla=d+A$ for a matrix-valued one-form $A$; under a frame change $g$ the matrix transforms as

$$
A'=g^{-1}Ag+g^{-1}dg.
$$

Its [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) is defined by

$$
d_A(s\otimes\alpha)=\nabla s\wedge\alpha+s\otimes d\alpha,
$$

and locally

$$
d_A\eta=d\eta+A\wedge\eta.
$$

This formula and the graded Leibniz rule show that definitions in different frames agree.

The [curvature form of a connection](../../../fiber-bundle.md#curvature-form) is $F(A)=d_A^2$. Locally,

$$
F(A)=dA+A\wedge A.
$$

Its covariant derivative satisfies the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity)

$$
d_AF=dF+A\wedge F-F\wedge A=0.
$$

Indeed, substituting $F=dA+A\wedge A$, using $d^2=0$, and applying the graded Leibniz rule leaves equal and opposite terms.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The induced [dual connection](../../../fiber-bundle.md#dual-connection) is uniquely defined by

$$
(\nabla_X\alpha)(Y)=X(\alpha(Y))-\alpha(\nabla_XY),
$$

which immediately gives the required pairing identity. If

$$
\nabla_{\partial_i}\partial_j=\Gamma^k_{ij}\partial_k,
$$

then

$$
\nabla_{\partial_i}dx^k=-\Gamma^k_{ij}dx^j.
$$

A connection on $TB$ is symmetric, or [torsion-free](../../../fiber-bundle.md#torsion-free-connection), when

$$
T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]=0,
$$

equivalently $\Gamma^k_{ij}=\Gamma^k_{ji}$ in coordinates. With $\operatorname{Alt}B(X,Y)=B(X,Y)-B(Y,X)$,

$$
\begin{aligned}
(\operatorname{Alt}\nabla\alpha)(X,Y)
&=X\alpha(Y)-Y\alpha(X)-\alpha(\nabla_XY-\nabla_YX)\\
&=X\alpha(Y)-Y\alpha(X)-\alpha([X,Y])\\
&=d\alpha(X,Y).
\end{aligned}
$$

## 4

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [horizontal lift](../../../fiber-bundle.md#horizontal-lift) of $\gamma$ from $p$ is a curve $\widetilde\gamma$ in $E$ projecting to $\gamma$, starting at $p$, and tangent to the horizontal distribution of the connection. In a local frame write $\widetilde\gamma(t)=(\gamma(t),v(t))$. Horizontality is the linear ordinary differential equation

$$
v'(t)+A_{\gamma(t)}(\dot\gamma(t))v(t)=0,
$$

whose initial-value theorem gives local existence and uniqueness; successive trivializations continue the lift.

A [geodesic](../../../riemannian-geometry.md#geodesic) satisfies $\nabla_{\dot\gamma}\dot\gamma=0$, and

$$
\exp_p(v)=\gamma_v(1)
$$

for the geodesic with initial velocity $v$. Since $d(\exp_p)_0=1$, the [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $\exp_p$ a diffeomorphism near zero; its inverse gives [normal coordinates](../../../general-relativity.md#normal-coordinates). A geodesic sphere is $\exp_p(\{v:|v|=r\})$ inside such a normal neighborhood.

The [Gauss lemma](../../../riemannian-geometry.md#gauss-s-lemma-riemannian-geometry) states

$$
\langle d(\exp_p)_v(v),d(\exp_p)_v(w)\rangle=\langle v,w\rangle.
$$

For the variation $\gamma_s(t)=\exp_p(t(v+sw))$, let $J=\partial_s\gamma_s|_{s=0}$. The coordinate vector fields commute, so metric compatibility and constant geodesic speed give

$$
\frac d{dt}\langle\dot\gamma,J\rangle
=\frac12\partial_s|\dot\gamma_s|^2\big|_{s=0}
=\langle v,w\rangle.
$$

Since $J(0)=0$, evaluation at $t=1$ proves the formula. In particular radial and spherical directions are orthogonal.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose a normal ball on which $\exp_p$ is a diffeomorphism, and take $\varepsilon$ smaller than half its radius. For $|X|<\varepsilon$, $t\mapsto\exp_p(tX)$ is a geodesic of length $|X|$. If a competing curve remains in the normal ball, write it in polar form. The [Gauss lemma](../../../riemannian-geometry.md#gauss-s-lemma-riemannian-geometry) makes radial and angular velocities orthogonal, so its speed is at least the absolute radial speed and its length is at least $|X|$. A curve leaving the larger normal ball already accumulates more than $|X|$ in radial variation. Thus the radial geodesic minimizes length.

At $q$, both $X$ and the geodesic sphere $\Sigma$ are hypersurfaces. If their tangent hyperplanes were distinct, they would be transverse. The [transverse intersection theorem](../../../differential-geometry.md#transverse-intersection-theorem) would then make $X\cap\Sigma$ a submanifold of dimension

$$
(m-1)+(m-1)-m=m-2.
$$

For $m\geq3$ this has positive dimension near $q$, contradicting that the intersection is the singleton $\{q\}$. Therefore $T_qX=T_q\Sigma$.

The conclusion fails in dimension two because a transverse intersection is zero-dimensional and may be isolated. In the Euclidean plane, let $\Sigma$ be the unit circle, $q=(1,0)$, and let $X=\{(x,0):1/2<x<3/2\}$. Then $X\cap\Sigma=\{q\}$, but $T_qX$ is horizontal whereas $T_q\Sigma$ is vertical.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
