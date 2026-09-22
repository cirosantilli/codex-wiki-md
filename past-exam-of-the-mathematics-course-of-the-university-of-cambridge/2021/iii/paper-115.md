# Paper 115

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/Paper_115.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/Paper_115.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
  - [h](#2/h)
    - [Solution](#2/h/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
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
  - [f](#4/f)
    - [Solution](#4/f/solution)

## 1

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [orientable smooth manifold](../../../differential-geometry.md#orientable-smooth-manifold) is a smooth $n$-manifold that admits a smoothly varying orientation of its tangent spaces. Equivalently, it has an atlas whose coordinate-transition [Jacobian determinants](../../../calculus.md#jacobian-determinant) are positive, or a nowhere-vanishing smooth top-degree [differential form](../../../differential-form.md).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The zero section $C=\{t=0\}\subset M$ is a circle. Its [normal bundle](../../../algebraic-geometry.md#normal-bundle) is the real line bundle obtained from

$$
(x,v)\sim(x+2\pi,-v),
$$

so its clutching map reverses sign once around $C$. Its [mod-two Euler class of a real line bundle](../../../fiber-bundle.md#mod-two-euler-class-of-a-real-line-bundle), equivalently its first [Stiefel–Whitney class](../../../fiber-bundle.md#stiefel-whitney-class), therefore satisfies

$$
\langle w_1(\nu_C),[C]_{\mathbb F_2}\rangle=1.
$$

If $M$ were orientable, the splitting

$$
TM|_C\cong TC\oplus\nu_C
$$

and the orientation of the circle would orient $\nu_C$, forcing this mod-two Euler number to vanish. This contradiction proves that the [Möbius band](../../../topology.md#mobius-band) is nonorientable.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Choose a locally finite cover $(U_\alpha)$ such that on every chart meeting $Y$ there is a smooth defining function $f_\alpha$ with

$$
Y\cap U_\alpha=f_\alpha^{-1}(0),
\qquad df_\alpha|_Y\ne0,
$$

and take $f_\alpha=1$ on charts disjoint from $Y$. On an overlap, the supplied division lemma extends

$$
g_{\alpha\beta}=\frac{f_\alpha}{f_\beta}
$$

smoothly across $Y$. After shrinking the charts, this extension is nowhere zero. The identities $g_{\alpha\beta}g_{\beta\gamma}=g_{\alpha\gamma}$ make these functions transition functions for a [real line bundle](../../../fiber-bundle.md#real-line-bundle) $L\to X$.

Choose local frames $e_\alpha$ with $e_\beta=g_{\alpha\beta}e_\alpha$. Then the local sections

$$
s|_{U_\alpha}=f_\alpha e_\alpha
$$

agree on overlaps and define a global section. Its zero set is exactly $Y$. Along $Y$, its vertical derivative is represented by the nonzero covector $df_\alpha$, so $s$ is transverse to the zero section, as in the [transverse intersection theorem](../../../differential-geometry.md#transverse-intersection-theorem). This is the [defining line bundle of a properly embedded hypersurface](../../../differential-geometry.md#defining-line-bundle-of-a-properly-embedded-hypersurface).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Real line bundles over a paracompact space $X$ are classified by

$$
w_1(L)\in H^1(X;\mathbb F_2).
$$

Euclidean space $\mathbb R^n$ is a [contractible space](../../../algebraic-topology.md#contractible-space), so its first cohomology vanishes and every real line bundle on it is trivial. Apply this to the defining bundle from part (c). In a global trivialization, $s$ is a smooth real function with $Y=s^{-1}(0)$ and $ds|_Y\ne0$. Thus $ds$, or a metric-dual normal vector field, gives a global orientation of the normal line. Combining this with the standard orientation of $\mathbb R^n$ gives an orientation of $Y$ using the same normal-first convention as the [outward-normal-first boundary orientation](../../../differential-geometry.md#outward-normal-first-boundary-orientation). Hence every properly embedded hypersurface in $\mathbb R^n$ is orientable.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

**Yes.** For any $R>1$, the formula

$$
[(x,t)]\longmapsto
\bigl((R+t\cos(x/2))\cos x,
(R+t\cos(x/2))\sin x,
t\sin(x/2)\bigr)
$$

defines the standard smooth embedding of the open [Möbius band](../../../topology.md#mobius-band) into $\mathbb R^3$. Replacing $(x,t)$ by $(x+2\pi,-t)$ leaves the displayed point unchanged. The image is the interior of a compact Möbius strip, so the embedding fails to be a [proper map](../../../cohomology.md#proper-map); this is why it does not contradict part (d).

## 2

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The integral of an [exact differential form](../../../differential-form.md#exact-differential-form) over the closed curve $S^1$ is zero by [Stokes theorem](../../../calculus.md#stokes-theorem), so the map is well defined on [de Rham cohomology](../../../differential-form.md#de-rham-cohomology). It is surjective because the angular form $d\theta$ has integral $2\pi$. If a closed one-form $\alpha$ has zero integral, define

$$
F(e^{i\theta})=\int_0^\theta\alpha.
$$

The zero period makes this definition $2\pi$-periodic, and $dF=\alpha$. Thus the kernel is zero and

$$
H^1_{\mathrm{dR}}(S^1)\xrightarrow{\int_{S^1}}\mathbb R
$$

is an isomorphism.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The overlap $U_0\cap U_1$ is $\mathbb C^*$ in the coordinate $z$, and radial projection $z\mapsto z/|z|$ is a [deformation retraction](../../../algebraic-topology.md#deformation-retraction) onto $S^1$. The [homotopy invariance of de Rham cohomology](../../../differential-form.md#homotopy-invariance-of-de-rham-cohomology) identifies its first de Rham cohomology with that of $S^1$, and the identification is compatible with integration around the unit circle. Hence the same integral map is an isomorphism.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Each $U_j$ is isomorphic to $\mathbb C$ and is therefore contractible. Every [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) over a contractible paracompact space is trivial, so $L|_{U_0}$ and $L|_{U_1}$ admit the required trivializations.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Since $\beta=f^{-1}df$,

$$
\frac d{dt}f(\gamma(t))
=f(\gamma(t))\,\beta_{\gamma(t)}(\dot\gamma(t)).
$$

The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and the [chain rule](../../../calculus.md#chain-rule) then give

$$
F'(t)
=e^{-\int_0^t\gamma^*\beta}
\left(\frac d{dt}f(\gamma(t))-f(\gamma(t))\beta(\dot\gamma(t))\right)=0.
$$

**Thus $F$ is constant.**

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Parametrize the unit circle by a loop $\gamma:[0,2\pi]\to\mathbb C^*$. Part (d) and $f(\gamma(0))=f(\gamma(2\pi))$ imply

$$
\exp\left(-\int_{S^1}\beta\right)=1.
$$

The kernel of the [complex exponential function](../../../calculus.md#complex-exponential-function) is $2\pi i\mathbb Z$, so

$$
\int_{S^1}\beta=2\pi i k
$$

for some $k\in\mathbb Z$. This integer is the [winding number](../../../complex-analysis.md#winding-number) of $f|_{S^1}$.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

For $h=z^{-k}f$,

$$
\alpha=h^{-1}dh=\beta-kz^{-1}dz.
$$

The scalar-valued form $h^{-1}dh$ is closed, and

$$
\int_{S^1}\alpha=2\pi ik-k\int_{S^1}z^{-1}dz=0.
$$

By the period isomorphism from part (b), $[\alpha]=0$ in complexified [de Rham cohomology](../../../differential-form.md#de-rham-cohomology). Hence there is a smooth complex-valued function $\varphi$ on $U_0\cap U_1$ with $\alpha=d\varphi$.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

Using $d\varphi=h^{-1}dh$,

$$
d(he^{-\varphi})=e^{-\varphi}(dh-h,d\varphi)=0.
$$

The overlap $\mathbb C^*$ is connected, so $he^{-\varphi}=c$ for some $c\in\mathbb C^*$. Choose $C\in\mathbb C$ with $e^C=c$ and replace $\varphi$ by $\varphi+C$. Then $h=e^\varphi$.

<h3 id="2/h">h</h3>

↑ **Parent:** [2](#2)

<h4 id="2/h/solution">Solution</h4>

↑ **Parent:** [H](#2/h)

Let $(\rho_0,\rho_1)$ be a smooth [partition of unity](../../../differential-geometry.md#partition-of-unity) subordinate to $(U_0,U_1)$. On $U_0$, extend $\rho_1\varphi$ by zero away from the overlap, and on $U_1$ extend $\rho_0\varphi$ similarly. Define

$$
\psi_0=\exp(\rho_1\varphi)\quad\hbox{on }U_0,
\qquad
\psi_1=\exp(-\rho_0\varphi)\quad\hbox{on }U_1.
$$

On the overlap,

$$
\frac{\psi_1}{\psi_0}=e^{-(\rho_0+\rho_1)\varphi}=e^{-\varphi}=h^{-1},
$$

and therefore

$$
\boxed{\frac{\psi_1}{\psi_0}f=h^{-1}f=z^k.}
$$

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Changing the two local frames by the nowhere-zero functions $\psi_j$ replaces the transition function $f$ by

$$
\frac{\psi_1}{\psi_0}f=z^k.
$$

With the standard convention that the [tautological bundle](../../../fiber-bundle.md#tautological-bundle) $\mathcal O_{\mathbb{CP}^1}(-1)$ has transition function $z$, its $k$th tensor power $\mathcal O_{\mathbb{CP}^1}(-k)$ has transition function $z^k$. Thus

$$
L\cong\mathcal O_{\mathbb{CP}^1}(-k).
$$

This is the [smooth classification of complex line bundles on the complex projective line](../../../fiber-bundle.md#smooth-classification-of-complex-line-bundles-on-the-complex-projective-line) by their winding number.

## 3

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [principal connection](../../../fiber-bundle.md#connection-principal-bundle) on $P$ is a $G$-equivariant smooth splitting

$$
T_pP=H_p\oplus V_p,
$$

where $V_p$ is tangent to the $G$-orbit. Equivalently, it is a $\mathfrak g$-valued one-form $\mathcal A$ satisfying $\mathcal A(\xi_P)=\xi$ and $R_g^*\mathcal A=\operatorname{Ad}_{g^{-1}}\mathcal A$. Its [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection) is

$$
\boxed{\mathcal F=d\mathcal A+\frac12[\mathcal A\wedge\mathcal A].}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

On $S^n\times S^n$, consider $q(x,y)=\langle x,y\rangle$. At a point of $q^{-1}(0)$, its differential is

$$
dq_{(x,y)}(u,v)=\langle u,y\rangle+\langle x,v\rangle.
$$

The tangent vector $(y,x)$ lies in $T_xS^n\oplus T_yS^n$ and has $dq(y,x)=2$, so zero is a [regular value](../../../differential-geometry.md#regular-value). The [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) makes $P=q^{-1}(0)$ a smooth submanifold. Its tangent space is

$$
\boxed{T_{(x,y)}P=\left\{(u,v):
\langle u,x\rangle=0,
\ \langle v,y\rangle=0,
\ \langle u,y\rangle+\langle x,v\rangle=0
\right\}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The points $(x,y)$ are ordered orthonormal two-frames, so $P$ is the [Stiefel manifold](../../../fiber-bundle.md#stiefel-manifold) $V_2(\mathbb R^{n+1})$. Changing an orthonormal basis of the same plane gives the displayed free right $O(2)$-action. Since $O(2)$ is compact, the action is proper, and the quotient is the [Grassmannian](../../../differential-geometry.md#grassmannian) of unoriented two-planes. The [Free proper Lie-group action theorem](../../../fiber-bundle.md#free-proper-lie-group-action-theorem) makes

$$
P\longrightarrow P/O(2)
$$

a principal $O(2)$-bundle.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.
$$

The vertical space is spanned by the fundamental vector $(y,-x)$ corresponding to $J\in\mathfrak o(2)$. Define

$$
\mathcal A_{(x,y)}(u,v)=\langle u,y\rangle J=-\langle v,x\rangle J.
$$

It sends $(y,-x)$ to $J$, is $O(2)$-equivariant, and therefore is a [principal connection](../../../fiber-bundle.md#connection-principal-bundle). Its kernel consists exactly of those $(u,v)$ for which

$$
\langle u,x\rangle=\langle u,y\rangle
=\langle v,x\rangle=\langle v,y\rangle=0.
$$

These are precisely the velocities satisfying the stated horizontality condition. Every tangent vector has the unique decomposition

$$
(u,v)=\langle u,y\rangle(y,-x)
+\bigl((u,v)-\langle u,y\rangle(y,-x)\bigr),
$$

into vertical and horizontal parts, proving uniqueness. This is the [Canonical principal connection on the Stiefel bundle over a Grassmannian](../../../fiber-bundle.md#canonical-principal-connection-on-the-stiefel-bundle-over-a-grassmannian).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Write $\mathcal A=aJ$ with the scalar one-form

$$
a=\langle dx,y\rangle=-\langle x,dy\rangle.
$$

The Lie algebra $\mathfrak o(2)$ is abelian, so $[\mathcal A\wedge\mathcal A]=0$. Moreover

$$
da((u_1,v_1),(u_2,v_2))
=\langle u_2,v_1\rangle-\langle u_1,v_2\rangle.
$$

Consequently

$$
\mathcal F((u_1,v_1),(u_2,v_2))
=\bigl(\langle u_2,v_1\rangle-\langle u_1,v_2\rangle\bigr)
\begin{pmatrix}0&-1\\1&0\end{pmatrix},
$$

as required.

## 4

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

As a vector space, the [Lie algebra](../../../lie-algebra.md) of $G$ is $\mathfrak g=T_eG$. For $\xi\in\mathfrak g$, define

$$
l_\xi(g)=(dL_g)_e\xi,
$$

where $L_g$ is [Left translation on a Lie group](../../../lie-theory.md#left-and-right-translation-on-a-lie-group). This vector field is smooth and left-invariant because $(dL_h)_g l_\xi(g)=l_\xi(hg)$. The assignment $\xi\mapsto l_\xi$ is linear and injective by evaluation at $e$. Conversely, every left-invariant vector field $V$ satisfies $V(g)=(dL_g)_eV(e)$, so it equals $l_{V(e)}$. Hence the map is an isomorphism.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) is bilinear, alternating, satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity), and is natural under [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism). Therefore the bracket of two [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) is left-invariant. Define

$$
[\xi,\eta]=[l_\xi,l_\eta]_e.
$$

Then

$$
l_{[\xi,\eta]}=[l_\xi,l_\eta],
$$

and the inherited bilinearity, alternation, and Jacobi identity make $T_eG$ a [Lie algebra](../../../lie-algebra.md).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) $\gamma_\xi(t)=\exp(t\xi)$ is the integral curve through the identity of $l_\xi$. Its defining initial-value problem is

$$
\boxed{\dot\gamma_\xi(t)
=l_\xi(\gamma_\xi(t))
=(dL_{\gamma_\xi(t)})_e\xi,
\qquad
\gamma_\xi(0)=e.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection). Its [torsion form](../../../fiber-bundle.md#torsion-form) is

$$
T(u,v)=\nabla_uv-\nabla_vu-[u,v].
$$

Since $T=0$,

$$
\nabla_uv-\nabla_vu=[u,v].
$$

In coordinates this is the symmetry $\Gamma^i_{jk}=\Gamma^i_{kj}$ of the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is also a [metric connection](../../../fiber-bundle.md#metric-connection), so

$$
u\,g(v,w)=g(\nabla_uv,w)+g(v,\nabla_uw),
$$

and similarly for the two cyclic permutations. Add the identities with leading derivatives $u$ and $v$, subtract the one with leading derivative $w$, and use

$$
\nabla_vu=\nabla_uv-[u,v],
\quad
\nabla_uw=\nabla_wu+[u,w],
\quad
\nabla_vw=\nabla_wv+[v,w].
$$

Cancellation and symmetry of $g$ give

$$
u(g(v,w))+v(g(u,w))-w(g(u,v))
=2g(\nabla_uv,w)-g([u,v],w)+g(v,[u,w])+g(u,[v,w]).
$$

This is the [Koszul formula](../../../fiber-bundle.md#koszul-formula) written with the bracket terms on the right.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Take $u=v=l_\xi$ and $w=l_\eta$ in the identity from part (e). For a [left-invariant metric](../../../lie-theory.md#left-invariant-metric), all three scalar products are constant and $[l_\xi,l_\xi]=0$, so

$$
\langle\nabla_{l_\xi}l_\xi,l_\eta\rangle
=-\langle\xi,[\xi,\eta]\rangle.
$$

The curve $\gamma_\xi$ has velocity $l_\xi$, hence is a [geodesic](../../../riemannian-geometry.md#geodesic) exactly when $\nabla_{l_\xi}l_\xi=0$. Nondegeneracy of the inner product now gives

$$
\gamma_\xi\text{ is geodesic}
\quad\Longleftrightarrow\quad
\langle\xi,[\xi,\eta]\rangle=0
\quad\text{for every }\eta\in\mathfrak g.
$$

This is the [geodesic-vector criterion for a left-invariant metric](../../../lie-theory.md#geodesic-vector-criterion-for-a-left-invariant-metric).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
