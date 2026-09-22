# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper15.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
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
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) $X$ through $p$ is a [smooth curve](../../../differential-geometry.md#smooth-curve) $c:I\to M$, on an interval containing zero, satisfying $c(0)=p$ and $\dot c(t)=X_{c(t)}$. The [local flow](../../../differential-geometry.md#local-flow) is the smoothly varying family of these [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field):

$$
\phi:D\longrightarrow M,\qquad \phi_t(p)=c_p(t),\qquad
\phi_0(p)=p,\quad \partial_t\phi_t(p)=X_{\phi_t(p)}.
$$

Here $D$ is an open neighborhood of $\{0\}\times M$; for the maximal [local flow](../../../differential-geometry.md#local-flow), its fibre over $p$ is the maximal existence interval of $c_p$. Local existence, uniqueness and smooth dependence for a smooth [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) give this family. Uniqueness also gives $\phi_{t+s}(p)=\phi_t(\phi_s(p))$ whenever the relevant curves and compositions are defined, and $\phi_{-t}=\phi_t^{-1}$ on their common domains.

Reparametrizing the [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) gives

$$
\frac{d}{dt}\phi_{2t}(p)=2X_{\phi_{2t}(p)}.
$$

Thus **the flow of $2X$ is $\boxed{\widetilde\phi_t=\phi_{2t}}$**, with domain $\{(t,p):(2t,p)\in D\}$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Commutation of the two [local flows](../../../differential-geometry.md#local-flow) means $\phi_t\psi_s=\psi_s\phi_t$ for all sufficiently small independent parameters $s,t$, on their common local domains. Differentiate this identity in $s$ at zero. The [chain rule](../../../calculus.md#chain-rule) gives

$$
d\phi_t|_p(Y_p)=Y_{\phi_t(p)}.
$$

In a [coordinate chart](../../../differential-geometry.md#manifold-chart), differentiating again in $t$ at zero gives $DX_pY_p=DY_pX_p$. But the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) has coordinate expression

$$
[X,Y]_p=DY_pX_p-DX_pY_p,
$$

so commuting [local flows](../../../differential-geometry.md#local-flow) imply $[X,Y]=0$.

For the converse, suppose the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) vanishes. Write $u(t)=\phi_t(p)$ in a [coordinate chart](../../../differential-geometry.md#manifold-chart), and put $J(t)=d\phi_t|_p$. Differentiating the [local flow](../../../differential-geometry.md#local-flow) equation with respect to the initial point gives the variational [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation)

$$
\dot J(t)=DX_{u(t)}J(t),\qquad J(0)=I.
$$

Consequently $W(t)=Y_{u(t)}-J(t)Y_p$ satisfies

$$
\dot W(t)=DY_{u(t)}X_{u(t)}-DX_{u(t)}J(t)Y_p
=DX_{u(t)}W(t),\qquad W(0)=0,
$$

where the zero [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) was used in the second equality. Uniqueness for this linear [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) gives $W=0$. This is a local argument and can be continued through successive [coordinate charts](../../../differential-geometry.md#manifold-chart), proving $d\phi_t(Y)=Y\circ\phi_t$ wherever the [local flow](../../../differential-geometry.md#local-flow) is defined.

For fixed $t$, the curve $s\mapsto\phi_t(\psi_s(p))$ therefore has derivative $Y$ at its current point and starts at $\phi_t(p)$. Uniqueness of the [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) $Y$ identifies it with $s\mapsto\psi_s(\phi_t(p))$. Hence **$\boxed{\phi_t\psi_s=\psi_s\phi_t\ \Longleftrightarrow\ [X,Y]=0}$ locally**. No [complete vector field](../../../differential-geometry.md#complete-vector-field) hypothesis is needed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Using the coordinate formula for the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields), the two components are

$$
[X,Y]^x=X(0)-Y(y)=-\frac{x^2}{2},\qquad
[X,Y]^y=X(x^2/2)-Y(0)=xy.
$$

Thus $\boxed{[X,Y]=-(x^2/2)\partial_x+xy\partial_y}$, which is not the zero [vector field](../../../calculus.md#vector-field).

The [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) $X$ solve $\dot x=y$, $\dot y=0$, whereas those of $Y$ solve $\dot x=0$, $\dot y=x^2/2$. Their [local flows](../../../differential-geometry.md#local-flow) are

$$
\boxed{\phi_t(x,y)=(x+ty,y),\qquad \psi_s(x,y)=(x,y+sx^2/2).}
$$

Both formulas exist for all real parameters, so both are [complete vector fields](../../../differential-geometry.md#complete-vector-field). Direct composition gives

$$
\phi_t\psi_s(x,y)=(x+ty+tsx^2/2,\ y+sx^2/2),\qquad
\psi_s\phi_t(x,y)=(x+ty,\ y+s(x+ty)^2/2).
$$

At $(1,0)$ their first coordinates differ by $ts/2$. Hence these [local flows](../../../differential-geometry.md#local-flow) do not commute when $s,t$ are nonzero.

For the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields), start at $(2,0)$. An [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) $[X,Y]$ is

$$
(x(t),y(t))=\left(\frac{2}{1+t},0\right),\qquad -1<t<\infty.
$$

It solves $\dot x=-x^2/2$, $\dot y=xy$, but $x(t)$ diverges as $t\downarrow-1$. It cannot extend through that finite time as a curve in $\mathbb R^2$. **Complete vector fields are therefore not closed under the Lie bracket.**

For the sum $X+Y$, its [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) obey $\dot x=y$, $\dot y=x^2/2$. Substitution of $x=(1+\alpha t)^{-2}$ and $y=\beta(1+\alpha t)^{-3}$ requires

$$
\beta=-2\alpha,\qquad -3\alpha\beta=\frac12,
\qquad \alpha^2=\frac1{12}.
$$

Choosing $\alpha=-1/(2\sqrt3)$ gives the [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field)

$$
\gamma(t)=\left(\left(1-\frac{t}{2\sqrt3}\right)^{-2},
\frac1{\sqrt3}\left(1-\frac{t}{2\sqrt3}\right)^{-3}\right),\qquad t<2\sqrt3.
$$

It starts at $(1,1/\sqrt3)$ and escapes to infinity at the finite time $2\sqrt3$. **Complete vector fields are not closed under addition either.** Both failures use the same pair of [complete vector fields](../../../differential-geometry.md#complete-vector-field).

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A smooth rank-$r$ [vector bundle](../../../fiber-bundle.md#vector-bundle) over a [smooth manifold](../../../differential-geometry.md#smooth-manifold) $M$ consists of a smooth total space $E$, a smooth projection $\pi:E\to M$, and an $r$-dimensional real [vector space](../../../vector-space.md) structure on each fibre $E_p=\pi^{-1}(p)$. Each point has a neighborhood $U$ with a [vector bundle trivialization](../../../fiber-bundle.md#vector-bundle-trivialization)

$$
\tau_U:\pi^{-1}(U)\xrightarrow{\sim}U\times\mathbb R^r
$$

that is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), commutes with projection to $U$, and is a [linear isomorphism](../../../vector-space.md#linear-isomorphism) on every fibre. The overlap maps have the form $(p,v)\mapsto(p,h(p)v)$ with $h:U\cap V\to GL_r(\mathbb R)$ smooth. For a complex [vector bundle](../../../fiber-bundle.md#vector-bundle), replace $\mathbb R$ by $\mathbb C$ and require complex-linear fibre maps.

A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) is an $\mathbb R$-linear map

$$
\nabla:\Gamma(E)\longrightarrow\Omega^1(M;E),\qquad
\nabla(fs)=df\otimes s+f\nabla s,
$$

where $\Gamma(E)$ is the [module of smooth sections](../../../fiber-bundle.md#module-of-smooth-sections), $\Omega^1(M;E)$ consists of [vector-bundle-valued differential forms](../../../differential-form.md#vector-bundle-valued-differential-form) of degree one, and $f$ is a [smooth function](../../../analysis.md#smooth-function). Equivalently, evaluating on a [vector field](../../../calculus.md#vector-field) $X$ gives operators $\nabla_X$ with $\nabla_{fX}s=f\nabla_Xs$ and $\nabla_X(fs)=X(f)s+f\nabla_Xs$. A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) is local: its value at a point depends on the germ of the [section of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle), so the same definition applies to local sections.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Realize the [pullback vector bundle](../../../fiber-bundle.md#pullback-vector-bundle) as

$$
\phi^*E=\{(p,v)\in M'\times E:\phi(p)=\pi(v)\},\qquad
\pi'(p,v)=p.
$$

Its fibre over $p$ is canonically $E_{\phi(p)}$, with the same [vector space](../../../vector-space.md) operations. If a [vector bundle trivialization](../../../fiber-bundle.md#vector-bundle-trivialization) over $U\subset M$ is $\tau_U(v)=(\pi(v),\widehat v)$, give the [pullback vector bundle](../../../fiber-bundle.md#pullback-vector-bundle) the local trivialization

$$
T_U:(\pi')^{-1}(\phi^{-1}U)\longrightarrow\phi^{-1}U\times\mathbb R^r,
\qquad T_U(p,v)=(p,\widehat v).
$$

Declare these maps to be local homeomorphisms and use [coordinate charts](../../../differential-geometry.md#manifold-chart) on $M'$ to obtain a [smooth atlas](../../../differential-geometry.md#smooth-atlas) on the total space. On overlaps the [smooth transition maps](../../../differential-geometry.md#smooth-transition-map) are $(p,w)\mapsto(p,h(\phi(p))w)$, hence smooth and fibrewise linear. They satisfy the same cocycle identities as the original transition maps. This gives a well-defined smooth [vector bundle](../../../fiber-bundle.md#vector-bundle), with smooth projection and rank $r$. It also gives the [subspace topology](../../../topology.md#subspace-topology) inherited from $M'\times E$: inside each product $\phi^{-1}(U)\times\pi^{-1}(U)$ the defining condition is the graph of $\phi$ in the base coordinates. Thus the total space is Hausdorff and second countable, as required for a [smooth manifold](../../../differential-geometry.md#smooth-manifold).

For a smooth [section of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle) $s$ over $U$, its pulled-back section is more precisely $p\mapsto(p,s(\phi(p)))$. If $s$ has component column $u:U\to\mathbb R^r$ in the original [vector bundle trivialization](../../../fiber-bundle.md#vector-bundle-trivialization), its component column in $T_U$ is $u\circ\phi$, which is smooth. **The pullback is a smooth rank-$r$ vector bundle, and every local section pulls back smoothly.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The expression $d\phi(X)$ is in general a [vector field along a map](../../../fiber-bundle.md#vector-field-along-a-map), rather than a [vector field](../../../calculus.md#vector-field) on $M$. Its intended meaning in the required formula is pointwise evaluation of the [vector-bundle-valued differential form](../../../differential-form.md#vector-bundle-valued-differential-form) $\nabla s$:

$$
\bigl(\nabla'_{X}(\phi^*s)\bigr)_p
=(\nabla s)_{\phi(p)}(d\phi_pX_p),
$$

using the canonical identification $(\phi^*E)_p=E_{\phi(p)}$. This interpretation works for every [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds), including a constant map or a map with self-intersections.

Choose a [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle) over $U$, written as a row $e=(e_1,\ldots,e_r)$. Define its [connection one-form](../../../fiber-bundle.md#connection-one-form) $\Omega$ by

$$
\nabla(eu)=e(du+\Omega u)
$$

for component columns $u$. The pulled-back frame $e^\phi=(\phi^*e_1,\ldots,\phi^*e_r)$ is a [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle) over $\phi^{-1}U$. For any component column $v$ of [smooth functions](../../../analysis.md#smooth-function) on that open set, define

$$
\boxed{\nabla'(e^\phi v)=e^\phi\bigl(dv+(\phi^*\Omega)v\bigr).}
$$

Here the matrix entries of $\phi^*\Omega$ are ordinary [pullbacks of a differential form](../../../differential-form.md#pullback-of-a-differential-form). The displayed operator is linear and satisfies the [Leibniz rule](../../../calculus.md#leibniz-rule), hence is locally a [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle).

To prove these local operators glue, change the original [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle) to $\widetilde e=eh$. Expanding $\nabla(eh u)$ gives the [change of frame of a vector-bundle connection](../../../fiber-bundle.md#change-of-frame-of-a-vector-bundle-connection)

$$
\widetilde\Omega=h^{-1}\Omega h+h^{-1}dh.
$$

The [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) and the [chain rule](../../../calculus.md#chain-rule) give

$$
\phi^*\widetilde\Omega
=(h\circ\phi)^{-1}(\phi^*\Omega)(h\circ\phi)
+(h\circ\phi)^{-1}d(h\circ\phi).
$$

This is precisely the required transformation law for the pulled-back frame $\widetilde e^\phi=e^\phi(h\circ\phi)$. Thus the definitions agree and give a global [pullback connection](../../../fiber-bundle.md#pullback-connection).

For $s=eu$, substitute $v=u\circ\phi$ in the defining formula and use $d(u\circ\phi)(X)=du(d\phi(X))$. This proves the required identity. Conversely that identity fixes $\nabla'_X(\phi^*e_a)$; the [Leibniz rule](../../../calculus.md#leibniz-rule) then fixes the derivative of every $\sum_a v^a\phi^*e_a$, proving uniqueness. If the identity is initially imposed only on global [sections of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle), multiply each local frame section by a [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) equal to one near the point in question and supported in $U$, and extend by zero. These global sections agree with the frame locally, so the same uniqueness argument applies. **The pullback connection exists and is unique.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [curvature form of a connection](../../../fiber-bundle.md#curvature-form) is the endomorphism-valued [differential two-form](../../../differential-form.md#2-form) defined by

$$
R^\nabla(X,Y)s=\nabla_X\nabla_Ys-\nabla_Y\nabla_Xs-\nabla_{[X,Y]}s.
$$

It is alternating in $X,Y$. To see its [tensoriality](../../../fiber-bundle.md#tensoriality), replacing $X$ by $fX$ produces an extra $-Y(f)\nabla_Xs$ from the second term and an extra $+Y(f)\nabla_Xs$ from $[fX,Y]=f[X,Y]-Y(f)X$, so these cancel. Alternation gives linearity over [smooth functions](../../../analysis.md#smooth-function) in $Y$ too. Replacing $s$ by $fs$ produces the additional coefficient $(X(Yf)-Y(Xf)-[X,Y]f)s=0$; all terms involving one derivative of $s$ also cancel. Thus $R^\nabla$ belongs to $\Omega^2(M;\operatorname{End}E)$.

In the coefficient-column convention of part (b), expanding the definition gives

$$
R^\nabla(X,Y)(eu)=e\Bigl(
X(\Omega(Y))-Y(\Omega(X))-\Omega([X,Y])
+\Omega(X)\Omega(Y)-\Omega(Y)\Omega(X)\Bigr)u.
$$

The first three terms are $d\Omega(X,Y)$, and the last two are $(\Omega\wedge\Omega)(X,Y)$. This proves the [Cartan curvature matrix equation](../../../fiber-bundle.md#cartan-curvature-matrix-equation) $F=d\Omega+\Omega\wedge\Omega$, with matrix multiplication combined with the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms).

The [pullback connection](../../../fiber-bundle.md#pullback-connection) has matrix $\Omega'=\phi^*\Omega$. Since the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) commutes with the [exterior derivative](../../../differential-form.md#exterior-derivative) and the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms), its [curvature form of a connection](../../../fiber-bundle.md#curvature-form) has matrix

$$
F'=d(\phi^*\Omega)+(\phi^*\Omega)\wedge(\phi^*\Omega)
=\phi^*(d\Omega+\Omega\wedge\Omega)=\phi^*F.
$$

Changes of [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle) conjugate both sides by the same pulled-back transition matrix, so this identity is intrinsic. In fibre notation the answer is

$$
\boxed{R^{\nabla'}_p(u,v)=R^\nabla_{\phi(p)}(d\phi_pu,d\phi_pv),
\qquad u,v\in T_pM'.}
$$

Both sides act on the same fibre $E_{\phi(p)}$. No claim that $d\phi$ preserves [Lie brackets of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) for an arbitrary map is needed.

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An [oriented atlas](../../../differential-geometry.md#oriented-atlas) is a [smooth atlas](../../../differential-geometry.md#smooth-atlas) whose [smooth transition maps](../../../differential-geometry.md#smooth-transition-map) have positive [Jacobian determinants](../../../calculus.md#jacobian-determinant) at every point of their domains. Such an atlas supplies an [orientation of a vector space](../../../linear-algebra.md#orientation-of-a-vector-space) on every [tangent space](../../../differential-geometry.md#tangent-space), and these choices agree on overlaps.

Let $\omega$ be a nowhere-vanishing smooth top-degree [differential form](../../../differential-form.md). In a [coordinate chart](../../../differential-geometry.md#manifold-chart) write

$$
\omega=f(x)\,dx^1\wedge\cdots\wedge dx^n.
$$

The coefficient $f$ is smooth and nowhere zero. Restrict the [coordinate chart](../../../differential-geometry.md#manifold-chart) to connected neighborhoods; the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) makes the sign of $f$ constant on each. If $f$ is negative, replacing $x^1$ by $-x^1$ changes the sign of the coordinate [volume form](../../../differential-form.md#volume-form). Thus for $n\geq1$ we can choose a covering of [coordinate charts](../../../differential-geometry.md#manifold-chart) in each of which the coefficient is positive.

On an overlap of two such [coordinate charts](../../../differential-geometry.md#manifold-chart), the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms) transforms by

$$
dx^1\wedge\cdots\wedge dx^n
=\det\left(\frac{\partial x}{\partial y}\right)
dy^1\wedge\cdots\wedge dy^n.
$$

Consequently $f_y=f_x\det(\partial x/\partial y)$. Both coefficients are positive, so the [Jacobian determinant](../../../calculus.md#jacobian-determinant) is positive, as is that of the inverse transition. **A nowhere-vanishing top form therefore determines an oriented atlas.** The zero-dimensional case has only zero-dimensional transitions, whose determinant is one, and is automatically orientable. Connectedness of $M$ is not needed for the positive-dimensional construction; only the local sign choice matters.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use [coordinate charts](../../../differential-geometry.md#manifold-chart) from the chosen [oriented atlas](../../../differential-geometry.md#oriented-atlas). In each, the matrix $G_x=(g_{ij})$ of the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is smooth and [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form), so $\det G_x>0$ and its positive square root is smooth. Define the local [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) by

$$
\omega_{g,x}=\sqrt{\det G_x}\,dx^1\wedge\cdots\wedge dx^n.
$$

If $y$ is another positive [coordinate chart](../../../differential-geometry.md#manifold-chart) and $J=\partial x/\partial y$, the transformation rule for the [metric tensor](../../../general-relativity.md#metric-tensor) is $G_y=J^TG_xJ$. Taking [determinants](../../../linear-algebra.md#determinant) gives

$$
\det G_y=(\det J)^2\det G_x,
\qquad \sqrt{\det G_y}=|\det J|\sqrt{\det G_x}.
$$

The [oriented atlas](../../../differential-geometry.md#oriented-atlas) has $\det J>0$, so the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms) transformation from part (a) gives

$$
\sqrt{\det G_y}\,dy^1\wedge\cdots\wedge dy^n
=\sqrt{\det G_x}\,dx^1\wedge\cdots\wedge dx^n.
$$

The local expressions therefore glue to a global smooth top-degree [differential form](../../../differential-form.md). Its local coefficient never vanishes, so it is a [volume form](../../../differential-form.md#volume-form). **The global answer is $\boxed{\omega_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n}$ in positive charts.** In an arbitrary negatively oriented chart the corresponding expression needs a minus sign; the orientation is essential to the form, although a positive metric volume density exists without it.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**The integral identity requires compactness of $M$, compact support of $X$, or suitable conditions eliminating flux at infinity.** The printed question does not state such a hypothesis. We prove the [Riemannian divergence theorem](../../../calculus.md#riemannian-divergence-theorem) for a [compact manifold](../../../differential-geometry.md#compact-manifold), and more generally for a [compactly supported](../../../function.md#compact-support) smooth [vector field](../../../calculus.md#vector-field) on an oriented [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) with boundary.

Write $j:\partial M\hookrightarrow M$ for the inclusion. Give $\partial M$ the [outward-normal-first boundary orientation](../../../differential-geometry.md#outward-normal-first-boundary-orientation), and let $N$ be the outward unit [normal vector](../../../differential-geometry.md#normal-vector). The [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) of the induced [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is

$$
\omega_{\widetilde g}=j^*(\iota_N\omega_g).
$$

Indeed, if $(e_1,\ldots,e_{n-1})$ is a positively oriented [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) tangent to the boundary, $(N,e_1,\ldots,e_{n-1})$ is a positively oriented [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) in $M$. Both sides therefore evaluate to one on the boundary basis.

At a boundary point decompose $X=g(X,N)N+X^\top$, where $X^\top$ is tangent to $\partial M$. Evaluating on $n-1$ tangent vectors, the term with $X^\top$ vanishes: all $n$ arguments of the alternating [volume form](../../../differential-form.md#volume-form) then lie in the $(n-1)$-dimensional boundary [tangent space](../../../differential-geometry.md#tangent-space). Thus the [interior product of a differential form](../../../differential-form.md#interior-product) satisfies

$$
j^*(\iota_X\omega_g)=g(X,N)\,\omega_{\widetilde g}.
$$

The general [Stokes theorem](../../../calculus.md#stokes-theorem) for an oriented [manifold with boundary](../../../differential-geometry.md#manifold-with-boundary) states $\int_M d\eta=\int_{\partial M}j^*\eta$ for any smooth [differential form](../../../differential-form.md) $\eta$ of degree $n-1$ with [compact support](../../../function.md#compact-support); compactness of $M$ makes the support condition automatic. Applying it to $\eta=\iota_X\omega_g$ and using the defining equation for the [divergence of a Riemannian vector field](../../../calculus.md#divergence-of-a-riemannian-vector-field) proves

$$
\boxed{\int_M (\operatorname{div}X)\,\omega_g
=\int_{\partial M}g(X,N)\,\omega_{\widetilde g}.}
$$

For a concrete failure without the extra hypothesis, take $M=[0,\infty)$ with [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $dx^2$ and $X=(\arctan x)\partial_x$. The [divergence of a Riemannian vector field](../../../calculus.md#divergence-of-a-riemannian-vector-field) is $\operatorname{div}X=(1+x^2)^{-1}$, so

$$
\int_M\operatorname{div}X\,dx=\frac\pi2,
\qquad \int_{\partial M}g(X,N)\,\omega_{\widetilde g}=0,
$$

because $X$ vanishes at the only boundary point. Both integrals are finite. The missing $\pi/2$ is the limiting flux at infinity, so mere integrability of the divergence cannot repair the unrestricted assertion.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A subset $Z$ of an $m$-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold) $M$ is an $r$-dimensional [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) if, for each $p\in Z$, some [coordinate chart](../../../differential-geometry.md#manifold-chart) $x:U\to V\subset\mathbb R^m$ containing $p$ satisfies

$$
x(U\cap Z)=V\cap(\mathbb R^r\times\{0\}^{m-r}).
$$

The induced topology on $Z$ is the [subspace topology](../../../topology.md#subspace-topology), and the first $r$ coordinates restricted to $Z$ give its [smooth atlas](../../../differential-geometry.md#smooth-atlas). To see their [smooth transition maps](../../../differential-geometry.md#smooth-transition-map) agree, restrict the ambient smooth transitions to the coordinate planes; their inverses restrict in the same way. The inclusion then has injective [differential of a smooth map](../../../differential-geometry.md#differential-of-a-smooth-map) and is a homeomorphism onto its image. Conversely this is the local coordinate description of a smooth [smooth embedding](../../../differential-geometry.md#smooth-embedding). An [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) need not be a closed subset of $M$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $m=\dim M$ and $n=\dim N$. The hypothesis says that $q$ is a [regular value](../../../differential-geometry.md#regular-value) of $F$. Since its preimage is nonempty and the [differential of a smooth map](../../../differential-geometry.md#differential-of-a-smooth-map) is surjective there, $m\geq n$.

We use the following finite-dimensional [inverse function theorem](../../../calculus.md#inverse-function-theorem): if a smooth map $H:O\to\mathbb R^m$, with $O\subset\mathbb R^m$ open, has invertible derivative at $a$, there are open neighborhoods of $a$ and $H(a)$ on which $H$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), with smooth inverse.

Fix $p\in F^{-1}(q)$. Choose [coordinate charts](../../../differential-geometry.md#manifold-chart) centered at $p$ and $q$, and shrink the source neighborhood so that its image under $F$ lies in the target chart. Its coordinate expression is $f=(f^1,\ldots,f^n)$ with $f(0)=0$ and derivative of rank $n$. Choose $n$ domain coordinates giving an invertible $n\times n$ minor, and relabel them as $x^1,\ldots,x^n$. Define

$$
H(x)=\bigl(f^1(x),\ldots,f^n(x),x^{n+1},\ldots,x^m\bigr).
$$

Its derivative at zero has block form

$$
DH_0=\begin{pmatrix}B&C\\0&I_{m-n}\end{pmatrix},\qquad \det B\ne0,
$$

so it is invertible. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $u=H(x)$ a new [coordinate chart](../../../differential-geometry.md#manifold-chart) near $p$. In this chart $F=q$ is exactly $u^1=\cdots=u^n=0$, because the target chart sends $q$ to zero. These are [slice charts for an embedded submanifold](../../../differential-geometry.md#slice-chart-for-an-embedded-submanifold); reordering coordinates if desired puts the free coordinates first. Giving the level set the [subspace topology](../../../topology.md#subspace-topology), these restricted charts are smoothly compatible, as in part (a). This proves the [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) rather than merely invoking it.

**The level set is an embedded submanifold of dimension $\boxed{m-n}$**. The same coordinates show $T_pZ=\ker dF_p$: tangent vectors to the slice have zero first $n$ components, which are exactly the components of $dF_p$. The empty-dimensional case $m=n$ gives a discrete zero-dimensional [embedded submanifold](../../../differential-geometry.md#embedded-submanifold).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $m=\dim M$, $n=\dim N$ and $k=\operatorname{codim}_N S$. Fix $p\in f^{-1}(S)$ and choose the allowed [slice chart for an embedded submanifold](../../../differential-geometry.md#slice-chart-for-an-embedded-submanifold) on a neighborhood $U$ of $f(p)$, so that $S\cap U$ is given by $x^1=\cdots=x^k=0$. On $f^{-1}(U)$ define the [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds)

$$
G=(x^1,\ldots,x^k)\circ f:f^{-1}(U)\longrightarrow\mathbb R^k.
$$

The derivative $L=d(x^1,\ldots,x^k)$ at a point of $S\cap U$ is surjective and has kernel $T S$, by the slice description. The printed sum-of-spaces condition gives

$$
L\bigl(df_r(T_rM)\bigr)=\mathbb R^k\qquad
\text{for every }r\in f^{-1}(S\cap U).
$$

Indeed any target tangent vector is a sum of an image vector and a tangent vector to $S$, and $L$ kills the latter. By the [chain rule](../../../calculus.md#chain-rule), $dG_r=L\circ df_r$ is therefore surjective. This condition is precisely [transversality of a map to a submanifold](../../../differential-geometry.md#transversality-of-a-map-to-a-submanifold); the original sum need not be direct.

We have $G^{-1}(0)=f^{-1}(S)\cap f^{-1}(U)$. Part (b), applied to $G$, gives [slice charts for an embedded submanifold](../../../differential-geometry.md#slice-chart-for-an-embedded-submanifold) of codimension $k$ around every point of this zero set. Since the construction is available around every $p\in f^{-1}(S)$, the charts give its global structure as an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) with the [subspace topology](../../../topology.md#subspace-topology). **Its dimension is $\boxed{m-k=m-n+\dim S}$**. Moreover,

$$
\boxed{T_p(f^{-1}(S))=\{v\in T_pM:df_p(v)\in T_{f(p)}S\}.}
$$

This follows either from the slice coordinates or from $T_pG^{-1}(0)=\ker dG_p$ and $\ker L=T_{f(p)}S$. No injectivity of $df$, closedness of $S$, or direct-sum hypothesis is required.

## 5

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

An [affine connection](../../../fiber-bundle.md#affine-connection) $\nabla$ is a [metric connection](../../../fiber-bundle.md#metric-connection) for the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $g$ when

$$
\boxed{X\bigl(g(Y,Z)\bigr)=g(\nabla_XY,Z)+g(Y,\nabla_XZ)
\quad\text{for all vector fields }X,Y,Z.}
$$

Equivalently the induced [covariant derivative](../../../general-relativity.md#covariant-derivative) of the [metric tensor](../../../general-relativity.md#metric-tensor) satisfies $\nabla g=0$. This is [metric compatibility](../../../fiber-bundle.md#metric-compatibility); it imposes no condition on the [torsion tensor](../../../fiber-bundle.md#torsion-tensor). A [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) has the additional property of being a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection).

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

A [vector field along a map](../../../fiber-bundle.md#vector-field-along-a-map) $\gamma$ assigns $V(t)\in T_{\gamma(t)}M$ smoothly to each parameter value. Equivalently, it is a [section of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle) $\gamma^*TM$. The [pullback connection](../../../fiber-bundle.md#pullback-connection) defines its [covariant derivative along a curve](../../../fiber-bundle.md#covariant-derivative-along-a-curve), $D_tV$. To make the definition explicit, use [connection coefficients](../../../fiber-bundle.md#connection-components) with the convention

$$
\nabla_{\partial_i}\partial_j=\Gamma^k{}_{ij}\partial_k.
$$

For $V=V^k(t)\partial_k|_{\gamma(t)}$ the derivative is

$$
D_tV=\left(\frac{dV^k}{dt}
+\Gamma^k{}_{ij}(\gamma(t))\dot\gamma^i(t)V^j(t)\right)\partial_k.
$$

The [change of frame of a vector-bundle connection](../../../fiber-bundle.md#change-of-frame-of-a-vector-bundle-connection) ensures this expression is independent of the [coordinate chart](../../../differential-geometry.md#manifold-chart). It remains meaningful when $\dot\gamma=0$ and does not require extending $V$ to one ambient [vector field](../../../calculus.md#vector-field).

**The field is parallel exactly when $\boxed{D_tV=0}$**. A [geodesic](../../../riemannian-geometry.md#geodesic) for $\nabla$, with its specified affine parameter, is a [smooth curve](../../../differential-geometry.md#smooth-curve) whose own tangent is parallel:

$$
\boxed{D_t\dot\gamma=0,
\qquad \ddot\gamma^k+\Gamma^k{}_{ij}(\gamma)\dot\gamma^i\dot\gamma^j=0.}
$$

This definition applies to any [affine connection](../../../fiber-bundle.md#affine-connection), whether or not it is a [metric connection](../../../fiber-bundle.md#metric-connection). A non-affine change of parameter generally gives a [pregeodesic](../../../riemannian-geometry.md#pregeodesic) instead of this parametrized [geodesic](../../../riemannian-geometry.md#geodesic).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

We use the following existence and uniqueness statement for [parallel transport](../../../fiber-bundle.md#parallel-transport): for a smooth [affine connection](../../../fiber-bundle.md#affine-connection), a smooth curve $\gamma:[0,1]\to M$, an initial time $t_0$ and a vector $v\in T_{\gamma(t_0)}M$, there is a unique smooth [vector field along a map](../../../fiber-bundle.md#vector-field-along-a-map) $V$ on the whole curve satisfying $D_tV=0$ and $V(t_0)=v$. In a [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle) this is the linear [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) $\dot V=-\Gamma(\dot\gamma)V$. Its smooth coefficient matrix is bounded on every compact time subinterval in a trivializing neighborhood, and the linear existence theorem gives a solution throughout that subinterval. A finite subdivision of $[0,1]$ into such neighborhoods and uniqueness patch the solutions. No completeness hypothesis on $M$ is needed.

For arbitrary fields $U,V$ along a curve, the definition of the induced [covariant derivative](../../../general-relativity.md#covariant-derivative) of the [metric tensor](../../../general-relativity.md#metric-tensor) gives

$$
\frac d{dt}g(U,V)
=(\nabla_{\dot\gamma}g)(U,V)+g(D_tU,V)+g(U,D_tV).
$$

This can also be checked by differentiating $g_{ij}(\gamma(t))U^i(t)V^j(t)$ and substituting the formula in part (a). If $\nabla$ is a [metric connection](../../../fiber-bundle.md#metric-connection) and $V$ is parallel, it follows that $d(g(V,V))/dt=0$. Positivity of the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) makes $|V|=\sqrt{g(V,V)}$ constant. Thus [parallel transport](../../../fiber-bundle.md#parallel-transport) preserves lengths.

Conversely assume every parallel field along every smooth curve has constant length. Fix $p\in M$ and arbitrary $x,v\in T_pM$. Choose a curve through $p$ with velocity $x$ at an interior time $t_0$. Explicitly, in a [coordinate chart](../../../differential-geometry.md#manifold-chart) $z$ centered at $p$, take $\gamma(t)=z^{-1}(h(t)\,dz_p(x))$, where $h(t_0)=0$, $h'(t_0)=1$, and $h$ has sufficiently small amplitude and support near $t_0$. A [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) produces such $h$, so the curve is defined on all of $[0,1]$ and remains inside the chart. By the stated [parallel transport](../../../fiber-bundle.md#parallel-transport) theorem there is a parallel field with $V(t_0)=v$. Evaluating the derivative of its squared length gives

$$
0=\left.\frac d{dt}g(V,V)\right|_{t_0}=(\nabla_xg)_p(v,v).
$$

For fixed $x$, the [bilinear form](../../../linear-algebra.md#bilinear-form) $B_x(v,w)=(\nabla_xg)_p(v,w)$ is symmetric. Its diagonal values vanish, so [polarization identity](../../../linear-algebra.md#polarization-identity) gives

$$
2B_x(v,w)=B_x(v+w,v+w)-B_x(v,v)-B_x(w,w)=0.
$$

Since $p,x,v,w$ were arbitrary, $\nabla g=0$. **A connection is metric-compatible if and only if all parallel fields have constant length.** Polarization also shows that its [parallel transport](../../../fiber-bundle.md#parallel-transport) preserves all [inner products](../../../linear-algebra.md#inner-product), not just lengths.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

First verify the [difference of affine connections is a tensor](../../../fiber-bundle.md#difference-of-affine-connections-is-a-tensor). Linearity over [smooth functions](../../../analysis.md#smooth-function) in $X$ follows from the [affine connection](../../../fiber-bundle.md#affine-connection) axioms. In $Y$, the two derivative terms cancel:

$$
A(X,fY)=\nabla_X(fY)-\nabla'_X(fY)=fA(X,Y).
$$

Thus $A$ is a smooth $(1,2)$-[tensor field](../../../fiber-bundle.md#tensor-field), and $A_p(u,v)$ depends only on the tangent vectors $u,v$ at $p$. For any [smooth curve](../../../differential-geometry.md#smooth-curve), its two covariant accelerations satisfy

$$
D_t\dot\gamma-D'_t\dot\gamma=A(\dot\gamma,\dot\gamma).
$$

If $A(X,Y)=-A(Y,X)$, its diagonal values vanish. The two [geodesic equations](../../../riemannian-geometry.md#geodesic-equation) are therefore identical, and the connections have the same parametrized [geodesics](../../../riemannian-geometry.md#geodesic).

For necessity, the required local [geodesic](../../../riemannian-geometry.md#geodesic) existence theorem is this: for every smooth [affine connection](../../../fiber-bundle.md#affine-connection), $p\in M$ and $v\in T_pM$, a unique [geodesic](../../../riemannian-geometry.md#geodesic) exists on some interval about zero with $\gamma(0)=p$ and $\dot\gamma(0)=v$. Indeed the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) is the smooth first-order [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) on position and velocity

$$
\dot x^k=v^k,\qquad \dot v^k=-\Gamma^k{}_{ij}(x)v^iv^j,
$$

so local existence and uniqueness apply. If the two connections have the same parametrized [geodesics](../../../riemannian-geometry.md#geodesic), apply the acceleration identity to this [geodesic](../../../riemannian-geometry.md#geodesic) at zero to obtain $A_p(v,v)=0$ for every $p,v$. Expanding $A_p(u+v,u+v)=0$ gives $A_p(u,v)+A_p(v,u)=0$. Therefore

$$
\boxed{\text{same parametrized geodesics}\quad\Longleftrightarrow\quad
A(X,Y)=-A(Y,X).}
$$

This is the criterion that [parametrized geodesics determine the symmetric part of an affine connection](../../../fiber-bundle.md#parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection). It concerns equality with the same affine parameters. Agreement merely of unparametrized images is weaker: adding $\alpha(X)Y+\alpha(Y)X$ to a connection, for a smooth one-form $\alpha$, changes acceleration by a multiple of the velocity, which can be absorbed by reparametrization. Such a difference need not be antisymmetric.

Finally, since $\nabla'_XY=\nabla_XY-A(X,Y)$, expand the derivative of the [metric tensor](../../../general-relativity.md#metric-tensor):

$$
(\nabla'_Xg)(Y,Z)
=X(g(Y,Z))-g(\nabla'_XY,Z)-g(Y,\nabla'_XZ)
=(\nabla_Xg)(Y,Z)+g(A(X,Y),Z)+g(Y,A(X,Z)).
$$

Under the assumed [metric compatibility](../../../fiber-bundle.md#metric-compatibility) of $\nabla$, the first term is zero. Consequently

$$
\boxed{\nabla' g=0\quad\Longleftrightarrow\quad
g(A(X,Y),Z)=-g(Y,A(X,Z))\quad\text{for all }X,Y,Z.}
$$

Equivalently, for each fixed $X$, the endomorphism $A(X,\cdot)$ is skew-adjoint for the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). This metric criterion does not require the two connections to have the same [geodesics](../../../riemannian-geometry.md#geodesic).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
