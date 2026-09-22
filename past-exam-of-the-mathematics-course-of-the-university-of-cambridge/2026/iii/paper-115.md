# Paper 115

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20115.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20115.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\overline\nabla$ be the Euclidean connection and split the ambient tangent bundle along the [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) as $T\mathbb R^{n+m}|_M=TM\oplus NM$. The [second fundamental form](../../../second-fundamental-form.md) is the normal-bundle-valued bilinear form

$$
A(X,Y)=(\overline\nabla_XY)^\perp.
$$

It is symmetric because $\overline\nabla$ is torsion-free and the Lie bracket of tangent vector fields remains tangent:

$$
A(X,Y)-A(Y,X)
=\bigl(\overline\nabla_XY-\overline\nabla_YX\bigr)^\perp
=[X,Y]^\perp=0.
$$

This is the [symmetry of the second fundamental form](../../../second-fundamental-form.md#symmetry-of-the-second-fundamental-form).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

With the curvature convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, the [Gauss equation](../../../second-fundamental-form.md#gauss-equation) for a Euclidean embedded submanifold is

$$
\langle R(X,Y)Z,W\rangle
=\langle A(X,W),A(Y,Z)\rangle
-\langle A(X,Z),A(Y,W)\rangle.
$$

The [Codazzi equation](../../../second-fundamental-form.md#codazzi-equation) is

$$
(\nabla_XA)(Y,Z)=(\nabla_YA)(X,Z),
$$

where the derivative uses the Levi-Civita connection on tangent arguments and the normal connection on the value of $A$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On the unit sphere $S^n\subseteq\mathbb R^{n+1}$ choose the outward unit normal $N(x)=x$. For tangent vector fields $X,Y$,

$$
0=X\langle Y,N\rangle
=\langle\overline\nabla_XY,N\rangle+\langle Y,X\rangle,
$$

so

$$
A(X,Y)=-\langle X,Y\rangle N.
$$

If $X,Y$ are orthonormal, the [Gauss equation](../../../second-fundamental-form.md#gauss-equation) gives

$$
\langle R(X,Y)Y,X\rangle
=\langle A(X,X),A(Y,Y)\rangle-|A(X,Y)|^2=1.
$$

Thus the round unit sphere has [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) one. Tracing over an orthonormal basis gives its [scalar curvature](../../../second-fundamental-form.md#scalar-curvature)

$$
\boxed{\operatorname{Scal}_{S^n}=n(n-1).}
$$

## 2

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The metric and orientation determine the [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form): in a positively oriented coordinate chart $(x^1,\ldots,x^n)$,

$$
d\operatorname{vol}_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

Writing $|g|=\det(g_{ij})$ and $(g^{ij})=(g_{ij})^{-1}$, the [Dirichlet energy on a Riemannian manifold](../../../differential-geometry.md#dirichlet-energy-on-a-riemannian-manifold) with source $f$ is

$$
\boxed{E(u)=\int_M\left(\frac12g^{ij}(x)\,\partial_i u\,\partial_j u-fu\right)\sqrt{|g|}\,dx^1\cdots dx^n.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For an arbitrary smooth variation $u_t=u+t\varphi$, differentiation under the integral gives

$$
\left.\frac d{dt}E(u_t)\right|_{t=0}
=\int_M\left(g^{ij}\partial_i u\,\partial_j\varphi-f\varphi\right)\sqrt{|g|}\,dx.
$$

Since $M$ is compact without boundary, integration by parts turns this into

$$
-\int_M\left[
\frac1{\sqrt{|g|}}\partial_j\left(\sqrt{|g|}g^{ij}\partial_i u\right)+f
\right]\varphi\,d\operatorname{vol}_g.
$$

The [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
-\frac1{\sqrt{|g|}}\partial_j\left(\sqrt{|g|}g^{ij}\partial_i u\right)=f,
$$

or equivalently $-\Delta_gu=f$ for the [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Integrating the Euler-Lagrange equation and applying the [divergence theorem](../../../calculus.md#divergence-theorem) on the compact boundaryless manifold gives

$$
\int_M f\,d\operatorname{vol}_g
=-\int_M\Delta_gu\,d\operatorname{vol}_g=0.
$$

Equivalently, if this integral were nonzero, replacing $u$ by $u+C$ would leave the gradient term unchanged and make the energy unbounded below in one direction, so no minimizer could exist.

## 3

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write

$$
\Omega=\begin{pmatrix}0&I_n\\-I_n&0\end{pmatrix}.
$$

The identity belongs to $G$. If $A,B\in G$, then

$$
(AB)^T\Omega(AB)=B^T(A^T\Omega A)B=B^T\Omega B=\Omega.
$$

Taking determinants in $A^T\Omega A=\Omega$ shows that $A$ is invertible, and multiplying that identity by $A^{-T}$ and $A^{-1}$ gives $(A^{-1})^T\Omega A^{-1}=\Omega$. Thus $G$ is a group.

Let $\operatorname{Skew}_{2n}(\mathbb R)$ denote the vector space of skew-symmetric $2n\times2n$ matrices and define

$$
F:M_{2n}(\mathbb R)\longrightarrow\operatorname{Skew}_{2n}(\mathbb R),
\qquad F(A)=A^T\Omega A.
$$

Then $G=F^{-1}(\Omega)$. At $A\in G$,

$$
DF_A(H)=H^T\Omega A+A^T\Omega H.
$$

Given any skew-symmetric matrix $S$, set $H=AB$ with $B=-\frac12\Omega S$. Since $A^T\Omega A=\Omega$, a direct calculation gives

$$
DF_A(AB)=B^T\Omega+\Omega B=S.
$$

The derivative is therefore surjective at every point of $F^{-1}(\Omega)$. The [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) proves that the [symplectic group](../../../symplectic-geometry.md#symplectic-group) is an embedded submanifold of $M_{2n}(\mathbb R)$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The ambient matrix space has dimension $4n^2$, while the space of skew-symmetric $2n\times2n$ matrices has dimension

$$
\binom{2n}{2}=n(2n-1).
$$

Because $\Omega$ is a regular value, the codimension of its level set is the dimension of the target. Hence

$$
\boxed{\dim Sp(2n,\mathbb R)
=4n^2-n(2n-1)
=n(2n+1).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Ambient matrix multiplication

$$
M_{2n}(\mathbb R)\times M_{2n}(\mathbb R)\longrightarrow M_{2n}(\mathbb R),
\qquad(A,B)\longmapsto AB,
$$

is bilinear and therefore smooth. Its restriction to the embedded submanifold $G\times G$ is smooth, and part a shows that its image lies in $G$. By the defining smooth structure on an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold), this restriction is a smooth map $G\times G\to G$.

## 4

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the convention

$$
A(X,Y)=(\overline\nabla_XY)^\perp,
\qquad
\mathbf H=\sum_{i=1}^nA(e_i,e_i).
$$

An embedded submanifold is [minimal](../../../second-fundamental-form.md#minimal-surface) when its mean curvature vector $\mathbf H$ vanishes identically. For a variation $M_t$ with velocity field $V$, the [first variation of area](../../../second-fundamental-form.md#first-variation-of-area-formula) is

$$
\left.\frac d{dt}\operatorname{Area}(M_t)\right|_{t=0}
=-\int_M\langle\mathbf H,V\rangle,d\mu
+\int_{\partial M}\langle V,\eta\rangle,d\sigma,
$$

where $\eta$ is the outward unit conormal. For a boundaryless $M$, only the first integral remains. This sign convention is consistent with the outward variation of a round sphere increasing its area, because its $\mathbf H$ points inward.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $\overline\nabla f$ and $\overline{\operatorname{Hess}}f$ be the ambient gradient and Hessian. The [Laplacian of a restricted ambient function](../../../second-fundamental-form.md#laplacian-of-a-restricted-ambient-function) is

$$
\Delta_M(f|_M)
=\operatorname{tr}_{TM}(\overline{\operatorname{Hess}}f)
+\langle\overline\nabla f,\mathbf H\rangle.
$$

To prove it, choose a local orthonormal tangent frame $e_1,\ldots,e_n$ with $\nabla^M_{e_i}e_j=0$ at the point under consideration. There,

$$
\begin{aligned}
\Delta_M(f|_M)
&=\sum_i e_i(e_i f)\\
&=\sum_i\left(\overline{\operatorname{Hess}}f(e_i,e_i)
+\langle\overline\nabla f,\overline\nabla_{e_i}e_i\rangle\right)\\
&=\sum_i\overline{\operatorname{Hess}}f(e_i,e_i)
+\left\langle\overline\nabla f,\sum_iA(e_i,e_i)\right\rangle.
\end{aligned}
$$

Both sides are intrinsic scalars, so the pointwise calculation proves the formula everywhere.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Suppose that a positive-dimensional compact boundaryless minimal submanifold $M^n\subseteq\mathbb R^{n+m}$ existed. Apply part b to the squared ambient distance $f(x)=|x|^2$. Its ambient Hessian is $2$ times the Euclidean metric, its gradient is $2x$, and $\mathbf H=0$, so

$$
\Delta_M|x|^2=2n.
$$

Compactness makes $|x|^2$ attain a maximum. The [Laplacian at a local maximum](../../../differential-geometry.md#laplacian-at-a-local-maximum) is nonpositive, contradicting $2n>0$. Hence no such compact Euclidean minimal submanifold exists.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
