# Paper 115

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_115.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_115.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
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
  - [d](#3/d)
    - [Solution](#3/d/solution)
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

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [submersion](../../../differential-geometry.md#submersion) is a [smooth map between manifolds](../../../differential-geometry.md#smooth-map-between-manifolds) $F:X^n\to Y^m$ for which

$$
D_pF:T_pX\longrightarrow T_{F(p)}Y
$$

is surjective at every $p\in X$.

The local submersion theorem says that around every $p\in X$ there are coordinates $(x^1,\ldots,x^n)$ centered at $p$ and $(y^1,\ldots,y^m)$ centered at $F(p)$ in which

$$
F(x^1,\ldots,x^n)=(x^1,\ldots,x^m).
$$

To prove it, surjectivity lets us choose $m$ source coordinates such that $dF^1,\ldots,dF^m$ are independent. Complete them by source coordinates $x^{m+1},\ldots,x^n$ and define

$$
G=(F^1,\ldots,F^m,x^{m+1},\ldots,x^n).
$$

The derivative of $G$ is invertible at $p$, so the [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $G$ a local coordinate system; in these coordinates $F$ is the displayed projection.

For $q\in Y$, the fiber is locally given by

$$
x^1=q^1,\ldots,x^m=q^m.
$$

These are slice coordinates, so $F^{-1}(q)$ is an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) of dimension $n-m$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Choose a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) on $X$, using a [partition of unity](../../../differential-geometry.md#partition-of-unity) if necessary. For each $p$, let

$$
H_p=(\ker D_pF)^\perp.
$$

Since $F$ is a submersion, $D_pF|_{H_p}:H_p\to T_{F(p)}Y$ is an isomorphism. Its inverse depends smoothly on $p$, so

$$
v(p)=\left(D_pF|_{H_p}\right)^{-1}w(F(p))
$$

defines a smooth [vector field](../../../calculus.md#vector-field) on $X$ satisfying $D_pF(v(p))=w(F(p))$. The formula also gives $v(p)=0$ whenever $w(F(p))=0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Choose a coordinate ball $W$ around $q_1$ and a smaller convex coordinate ball $U$ whose closure lies in $W$. For $q_2\in U$, let $a$ be the constant coordinate vector from $q_1$ to $q_2$. Choose a [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) $\rho$ supported in $W$ and equal to one on $U$, and define in the chart

$$
w=\rho a,
$$

extending it by zero outside $W$. This is a compactly supported smooth vector field. The segment $q_1+ta$ stays in $U$, where $w=a$, so uniqueness for ordinary differential equations gives

$$
\Psi^t(q_1)=q_1+ta,\qquad 0\leq t\leq1.
$$

In particular, $\Psi^1(q_1)=q_2$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Fix $q_1$ and choose $U$ as in part c. For $q_2\in U$, choose the compactly supported $w$ moving $q_1$ to $q_2$, and lift it by part b to $v$. The support of $v$ is contained in

$$
F^{-1}(\operatorname{supp}w),
$$

which is compact because $F$ is a [proper map](../../../cohomology.md#proper-map). Hence $v$ is compactly supported and complete. If $\Phi^t$ and $\Psi^t$ are the flows of $v$ and $w$, then

$$
\frac d{dt}F(\Phi^t(p))
=D_{\Phi^t(p)}F(v)=w(F(\Phi^t(p))).
$$

Uniqueness of integral curves gives

$$
F\circ\Phi^t=\Psi^t\circ F.
$$

Therefore the diffeomorphism $\Phi^1$ maps $F^{-1}(q_1)$ onto $F^{-1}(q_2)$. Every equivalence class is open. Its complement, being a union of the other open classes, is also open; thus each class is clopen. If $Y$ is connected, there is only one class. This proves the fiber-diffeomorphism conclusion of the [Ehresmann fibration theorem](../../../fiber-bundle.md#ehresmann-fibration-theorem).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Properness is essential. The projection

$$
F:\mathbb R^2\setminus\{(0,0)\}\longrightarrow\mathbb R,
\qquad F(x,y)=x,
$$

is a submersion but is not proper. Its fiber over $x\ne0$ is diffeomorphic to $\mathbb R$, whereas its fiber over zero is $\mathbb R\setminus\{0\}$ and has two connected components.

Merely requiring every fiber to be a submanifold is also insufficient. The surjective map

$$
f:\mathbb R\longrightarrow\mathbb R,\qquad f(x)=x^3-x,
$$

has every fiber finite and therefore a zero-dimensional [embedded submanifold](../../../differential-geometry.md#embedded-submanifold). Some regular values have three preimages and others have one, so the fibers are not all diffeomorphic. The map fails to be a submersion at $x=\pm1/\sqrt3$.

## 2

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In local coordinates, for

$$
\alpha=\frac1{r!}\alpha_{i_1\ldots i_r}\,
dx^{i_1}\wedge\cdots\wedge dx^{i_r},
$$

the [exterior derivative](../../../differential-form.md#exterior-derivative) is

$$
d\alpha=\frac1{r!}\frac{\partial\alpha_{i_1\ldots i_r}}{\partial x^j}
dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.
$$

Applying $d$ again gives symmetric second partial derivatives contracted with the antisymmetric wedge $dx^k\wedge dx^j$, hence $d^2=0$. Expanding coefficients and moving $d\alpha$ past a degree-$r$ form gives the graded Leibniz rule

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta.
$$

For a function $f$ and smooth $F:X\to Y$, the chain rule gives

$$
d(F^*f)=d(f\circ F)=F^*(df).
$$

Every differential form is locally a sum of products $f_0\,df_1\wedge\cdots\wedge df_r$. Since pullback preserves products and wedge products, the function case and the graded Leibniz rule imply

$$
d(F^*\alpha)=F^*(d\alpha)
$$

for every form.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) of $X$ is

$$
H^r_{\mathrm{dR}}(X)
=\frac{\ker(d:\Omega^r(X)\to\Omega^{r+1}(X))}
{\operatorname{im}(d:\Omega^{r-1}(X)\to\Omega^r(X))}.
$$

Because pullback commutes with $d$, it sends [closed forms](../../../differential-form.md#closed-differential-form) to closed forms and [exact forms](../../../differential-form.md#exact-differential-form) to exact forms. Thus a smooth map induces

$$
F^*:H^r_{\mathrm{dR}}(Y)\longrightarrow H^r_{\mathrm{dR}}(X).
$$

Let $H:X\times I\to Y$ be a smooth homotopy and write $H_t(x)=H(x,t)$. If $V=\partial_t$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
\frac d{dt}H_t^*\omega
=H_t^*(\mathcal L_V\omega)
=d\,H_t^*(\iota_V\omega)+H_t^*(\iota_Vd\omega).
$$

Integrating defines a degree-minus-one operator $K$ satisfying

$$
H_1^*-H_0^*=dK+Kd.
$$

For closed $\omega$, the difference is exact, so smoothly homotopic maps induce the same map on de Rham cohomology.

If $F:X\to Y$ is a [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence) with inverse up to homotopy $G$, functoriality and homotopy invariance give

$$
G^*F^*=\operatorname{id},\qquad F^*G^*=\operatorname{id}.
$$

**Hence $F^*$ is an isomorphism.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

We induct on $n$. The claim is immediate for $\mathbb{CP}^0$. In the stated cover, $U=U_0\cong\mathbb C^n$ is contractible. The homotopy

$$
[z_0:z_1:\cdots:z_n]\longmapsto[t z_0:z_1:\cdots:z_n]
$$

deformation retracts $V$ onto the hyperplane $z_0=0$, which is $\mathbb{CP}^{n-1}$. Moreover,

$$
U\cap V\cong\mathbb C^n\setminus\{0\}
$$

deformation retracts onto $S^{2n-1}$.

The [Mayer--Vietoris sequence](../../../algebraic-topology.md#mayer-vietoris-sequence) for the de Rham complex contains

$$
H^{i-1}_{\mathrm{dR}}(U\cap V)
\longrightarrow H^i_{\mathrm{dR}}(\mathbb{CP}^n)
\longrightarrow H^i_{\mathrm{dR}}(U)\oplus H^i_{\mathrm{dR}}(V).
$$

For odd $i>1$, the group on the right vanishes by contractibility and the induction hypothesis, while the group on the left vanishes because $i-1$ is positive and even and is neither $0$ nor $2n-1$. Thus the middle group vanishes. For $i=1$, the preceding map

$$
H^0(U)\oplus H^0(V)\longrightarrow H^0(U\cap V)
$$

is surjective because all three spaces are connected, so the connecting map into $H^1(\mathbb{CP}^n)$ is zero. Therefore all odd de Rham cohomology groups of $\mathbb{CP}^n$ vanish.

## 3

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In a local frame of $E$, a [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) has the form

$$
d^{\mathcal A}=d+A\wedge,
$$

where $A$ is a matrix of one-forms. Under a frame change $g$, its matrix transforms as

$$
A'=g^{-1}Ag+g^{-1}dg.
$$

The [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) on an $E$-valued $r$-form $\sigma$ is

$$
d^{\mathcal A}\sigma=d\sigma+A\wedge\sigma.
$$

The [curvature form of a connection](../../../fiber-bundle.md#curvature-form) is

$$
F=dA+A\wedge A.
$$

Using the graded Leibniz rule,

$$
(d^{\mathcal A})^2\sigma
=d(A\wedge\sigma)+A\wedge d\sigma+A\wedge A\wedge\sigma
=(dA+A\wedge A)\wedge\sigma
=F\wedge\sigma.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Regard an $E^\vee$-valued $r$-form $\lambda$ as a row vector and an $\operatorname{End}(E)$-valued $r$-form $\mu$ as a matrix. The [dual connection](../../../fiber-bundle.md#dual-connection) and endomorphism connection are

$$
d^{\mathcal A^\vee}\lambda
=d\lambda-(-1)^r\lambda\wedge A,
$$



$$
d^{\operatorname{End}(\mathcal A)}\mu
=d\mu+A\wedge\mu-(-1)^r\mu\wedge A.
$$

For the curvature two-form,

$$
d^{\operatorname{End}(\mathcal A)}F=dF+A\wedge F-F\wedge A=0,
$$

because substituting $F=dA+A\wedge A$ makes all terms cancel. This is the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity).

For an endomorphism-valued $r$-form $\mu$ and an $E$-valued form $\sigma$, direct expansion gives the compatible Leibniz rule

$$
d^{\mathcal A}(\mu\wedge\sigma)
=d^{\operatorname{End}(\mathcal A)}\mu\wedge\sigma
+(-1)^r\mu\wedge d^{\mathcal A}\sigma.
$$

The cancellation of the two middle $A$-terms proves the identity.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For a path $\gamma:[0,1]\to B$, a section $s(t)$ of $\gamma^*E$ is parallel when

$$
\dot s+A(\dot\gamma)s=0.
$$

Existence and uniqueness for this linear ordinary differential equation define the [parallel transport](../../../fiber-bundle.md#parallel-transport)

$$
\mathcal P_\gamma^{\mathcal A}:E_{\gamma(0)}\longrightarrow E_{\gamma(1)}.
$$

Transport along the reversed path solves the inverse initial-value problem, so

$$
\mathcal P_{\bar\gamma}^{\mathcal A}
=(\mathcal P_\gamma^{\mathcal A})^{-1}.
$$

If $P(t)$ denotes transport from $0$ to $t$, then

$$
\mu(t)=P(t)\mu(0)P(t)^{-1}
$$

satisfies the horizontal equation for the induced endomorphism connection. Uniqueness therefore gives

$$
\boxed{\mathcal P_\gamma^{\operatorname{End}(\mathcal A)}(\mu)
=\mathcal P_\gamma^{\mathcal A}\,
\mu\,
(\mathcal P_\gamma^{\mathcal A})^{-1}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $b'\in B$. Since $B$ is path-connected, choose a path $\gamma$ from $b$ to $b'$. Horizontality of $\mu$ and part c imply

$$
\mu(b')
=\mathcal P_\gamma^{\mathcal A}\,
\mu(b)\,
(\mathcal P_\gamma^{\mathcal A})^{-1}.
$$

**Thus $\mu(b')$ is conjugate to the isomorphism $\mu(b)$ and is itself an isomorphism. Since $b'$ was arbitrary, $\mu$ is fiberwise invertible everywhere.**

## 4

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [solder form](../../../fiber-bundle.md#solder-form) on $X$ is the $TX$-valued one-form

$$
\theta(V)=V.
$$

In a coordinate frame it is $\theta=dx^i\otimes\partial_i$. The torsion form of $\nabla$ is

$$
T=d^\nabla\theta.
$$

Equivalently, for vector fields $U,V$,

$$
T(U,V)=\nabla_UV-\nabla_VU-[U,V].
$$

Writing

$$
\nabla_{\partial_i}\partial_j=\Gamma^k{}_{ji}\partial_k,
$$

and using $[\partial_i,\partial_j]=0$ gives

$$
T(\partial_i,\partial_j)
=(\Gamma^k{}_{ji}-\Gamma^k{}_{ij})\partial_k.
$$

Hence $\nabla$ is [torsion-free](../../../fiber-bundle.md#torsion-free-connection) exactly when

$$
\Gamma^k{}_{ji}=\Gamma^k{}_{ij}
$$

for every $i,j,k$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The connection is orthogonal, or metric-compatible, when $\nabla g=0$; equivalently, its [parallel transport](../../../fiber-bundle.md#parallel-transport) preserves the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Compatibility of the induced connections with tensor contraction gives

$$
\partial_i(g(U,V))
=g(\nabla_{\partial_i}U,V)+g(U,\nabla_{\partial_i}V)
$$

for all vector fields $U,V$. Taking $U=\partial_j$ and $V=\partial_k$ yields

$$
\frac{\partial g_{jk}}{\partial x^i}
=\Gamma^\ell{}_{ji}g_{\ell k}
+\Gamma^\ell{}_{ki}g_{j\ell}
=\Gamma_{jki}+\Gamma_{kji}.
$$

Conversely, this coordinate identity makes every component of $\nabla g$ vanish, so it is equivalent to orthogonality.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For forms of the same degree, define the Hodge inner product by

$$
\langle\alpha,\beta\rangle_X
=\int_X\alpha\wedge *\beta.
$$

On a $p$-form $\beta$, define the [codifferential](../../../differential-form.md#codifferential)

$$
\delta\beta=(-1)^p*^{-1}d*\beta,
$$

equivalently $\delta=(-1)^{n(p+1)+1}*d*$ in dimension $n$. If $\alpha$ has degree $p-1$, [Stokes theorem](../../../calculus.md#stokes-theorem) on the compact boundaryless manifold gives

$$
0=\int_Xd(\alpha\wedge *\beta)
=\int_Xd\alpha\wedge *\beta+(-1)^{p-1}\int_X\alpha\wedge d*\beta.
$$

Rearranging and using the definition of $\delta$ gives

$$
\langle d\alpha,\beta\rangle_X
=\langle\alpha,\delta\beta\rangle_X.
$$

**Thus $\delta$ is the formal adjoint of $d$.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

A form is [harmonic](../../../differential-form.md#harmonic-differential-form) when

$$
\Delta\alpha=(d\delta+\delta d)\alpha=0.
$$

Adjointness gives

$$
\langle\Delta\alpha,\alpha\rangle_X
=\lVert d\alpha\rVert^2+\lVert\delta\alpha\rVert^2.
$$

Therefore $\Delta\alpha=0$ implies $d\alpha=0$ and $\delta\alpha=0$; the converse follows immediately from the definition of $\Delta$.

The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) states in particular that every de Rham cohomology class has a unique harmonic representative. Hence

$$
\boxed{\mathcal H^p(X)\xrightarrow{\sim}H^p_{\mathrm{dR}}(X),
\qquad \alpha\longmapsto[\alpha].}
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For the stated flat metric and orientation,

$$
*dx^i=(-1)^{i-1}
dx^1\wedge\cdots\wedge\widehat{dx^i}\wedge\cdots\wedge dx^n.
$$

Because the metric coefficients and the coordinate one-forms are constant, the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) acts coefficientwise:

$$
\Delta(\alpha_i\,dx^i)=(\Delta\alpha_i)\,dx^i.
$$

Thus a harmonic one-form $\alpha=\sum_i\alpha_i dx^i$ has harmonic coefficient functions. Every harmonic function on the compact connected torus is constant by the [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions). Hence

$$
\mathcal H^1(T^n)
=\operatorname{span}_{\mathbb R}\{dx^1,\ldots,dx^n\}
\cong\mathbb R^n.
$$

The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) now gives

$$
\boxed{H^1_{\mathrm{dR}}(T^n)\cong\mathbb R^n.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
