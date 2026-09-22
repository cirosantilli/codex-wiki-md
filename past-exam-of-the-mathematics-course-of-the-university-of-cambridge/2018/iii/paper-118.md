# Paper 118

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_118.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_118.pdf)

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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

If $M$ has complex dimension $n$, its complexified [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) splits into the $(1,0)$ and $(0,1)$ [cotangent bundles](../../../symplectic-geometry.md#cotangent-bundle). The space of global smooth [differential forms of type (p, q)](../../../complex-geometry.md#differential-form-of-type-p-q) is

$$
\boxed{\mathcal A^{p,q}(M)=\Gamma_{C^\infty}\!\left(M,\Lambda^p(T^{1,0}M)^*\otimes\Lambda^q(T^{0,1}M)^*\right).}
$$

In [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate), its elements have the form $\alpha=\sum_{I,J}a_{I,J}\,dz^I\wedge d\bar z^J$, where the coefficients are complex-valued [smooth functions](../../../analysis.md#smooth-function), $|I|=p$, and $|J|=q$.

The [exterior derivative](../../../differential-form.md#exterior-derivative) decomposes as $d=\partial+\bar\partial$. The [conjugate Dolbeault operator](../../../complex-geometry.md#conjugate-dolbeault-operator) $\partial$ and [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) $\bar\partial$ are its type components:

$$
\boxed{\partial\alpha=\sum_{I,J,k}\frac{\partial a_{I,J}}{\partial z_k}\,dz_k\wedge dz^I\wedge d\bar z^J,\qquad
\bar\partial\alpha=\sum_{I,J,k}\frac{\partial a_{I,J}}{\partial\bar z_k}\,d\bar z_k\wedge dz^I\wedge d\bar z^J.}
$$

They have bidegrees $(1,0)$ and $(0,1)$ respectively. Keeping the displayed wedge order avoids hiding a sign; moving $d\bar z_k$ past $dz^I$ introduces $(-1)^p$. Decomposing $d^2=0$ by type gives $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[Complex conjugation](../../../complex-analysis.md#complex-conjugation) interchanges the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) and [conjugate Dolbeault operator](../../../complex-geometry.md#conjugate-dolbeault-operator). Thus $\partial\alpha=0$ implies $\bar\partial\bar\alpha=0$, and $\bar\alpha$ has type $(q,p)$. Its antiholomorphic degree is $p\geq1$, so the allowed [Dolbeault-Poincaré lemma](../../../complex-geometry.md#dolbeault-poincare-lemma) on the [polydisc](../../../complex-geometry.md#polydisc) gives a form $\gamma\in\mathcal A^{q,p-1}$ satisfying $\bar\partial\gamma=\bar\alpha$.

Conjugate this identity and put $\beta=\bar\gamma$. This proves the [conjugate Dolbeault-Poincaré lemma](../../../complex-geometry.md#conjugate-dolbeault-poincare-lemma):

$$
\boxed{\beta\in\mathcal A^{p-1,q}(\mathcal P^n),\qquad\partial\beta=\alpha.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A pure-type $d$-closed form is both $\partial$-closed and $\bar\partial$-closed, because these two derivatives have different types. Let $k=p+q$. The smooth [Poincaré lemma](../../../differential-form.md#poincare-lemma) on the [polydisc](../../../complex-geometry.md#polydisc) gives $\eta\in\mathcal A^{k-1}_{\mathbb C}$ with $d\eta=\alpha$. We will modify $\eta$ by exact terms without changing $d\eta$.

Write $\eta=\sum_r\eta^{r,k-1-r}$. Starting with the smallest holomorphic degree, eliminate every component with $r<p-1$. Once the lower components are zero, the $(r,k-r)$ component of $d\eta$ says $\bar\partial\eta^{r,k-1-r}=0$, since $r<p$. Its antiholomorphic degree is positive, so the [Dolbeault-Poincaré lemma](../../../complex-geometry.md#dolbeault-poincare-lemma) supplies $\nu^{r,k-2-r}$ with $\bar\partial\nu=\eta^{r,k-1-r}$. Replace $\eta$ by $\eta-d\nu$: this removes the component at $r$ and changes only the next holomorphic degree.

Next, work downwards from the largest holomorphic degree and eliminate the components with $r>p$. Once the higher components are zero, the corresponding component of $d\eta$ gives $\partial\eta^{r,k-1-r}=0$. By part (b), write this as $\partial\nu^{r-1,k-1-r}$ and again subtract $d\nu$. This affects only the next lower holomorphic degree. The two finite procedures leave

$$
\eta=u+v,\qquad u\in\mathcal A^{p-1,q},\quad v\in\mathcal A^{p,q-1}.
$$

The components of $d\eta=\alpha$ outside type $(p,q)$ now give $\bar\partial u=0$ and $\partial v=0$, while its $(p,q)$ component gives $\alpha=\partial u+\bar\partial v$.

Since $q\geq1$, the [Dolbeault-Poincaré lemma](../../../complex-geometry.md#dolbeault-poincare-lemma) gives $u=\bar\partial a$ with $a$ of type $(p-1,q-1)$. Since $p\geq1$, part (b) gives $v=\partial b$ of the same type. The anticommutation identity therefore yields

$$
\alpha=\partial\bar\partial a+\bar\partial\partial b=\partial\bar\partial(a-b).
$$

This proves the [Bott-Chern Poincaré lemma](../../../complex-geometry.md#bott-chern-poincare-lemma) using precisely the permitted primitives:

$$
\boxed{H_{BC}^{p,q}(\mathcal P^n)=0\qquad(p,q\geq1).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The natural map between [Bott-Chern cohomology](../../../complex-geometry.md#bott-chern-cohomology) and [Dolbeault cohomology](../../../complex-geometry.md#dolbeault-cohomology) is

$$
\phi:[\alpha]_{BC}\longmapsto[\alpha]_{\bar\partial}.
$$

It is well-defined: a $d$-closed pure-type form is $\bar\partial$-closed, and $\partial\bar\partial\beta=-\bar\partial(\partial\beta)$ is $\bar\partial$-exact.

For surjectivity, choose the unique [harmonic differential form](../../../differential-form.md#harmonic-differential-form) $h$ representing a [Dolbeault cohomology](../../../complex-geometry.md#dolbeault-cohomology) class using [Dolbeault Hodge decomposition](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold). The [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity) $\Delta_d=2\Delta_{\bar\partial}$ makes $h$ a [harmonic differential form](../../../differential-form.md#harmonic-differential-form) for $d$, hence $d$-closed. Sending the Dolbeault class to $[h]_{BC}$ consequently gives a right inverse.

For injectivity, the [ddbar lemma](../../../complex-geometry.md#ddbar-lemma) says directly that a $d$-closed, $\bar\partial$-exact pure-type form is $\partial\bar\partial$-exact. One can also exhibit its primitive. Let $G_d$ be the [Green operator of the Hodge Laplacian](../../../differential-form.md#green-operator-of-the-hodge-laplacian), and put $G_{\bar\partial}=2G_d$. If $\alpha$ is $d$-closed and $\bar\partial$-exact, its harmonic projection vanishes and the [Kähler identities](../../../complex-geometry.md#kahler-identities) give

$$
\alpha=\bar\partial\bar\partial^*G_{\bar\partial}\alpha
=-i\partial\bar\partial\Lambda G_{\bar\partial}\alpha.
$$

Here $\partial G_{\bar\partial}\alpha=\bar\partial G_{\bar\partial}\alpha=0$ because the Green operator commutes with these differentials, and $\bar\partial^*=-i[\Lambda,\partial]$. Thus $\alpha$ represents zero in [Bott-Chern cohomology](../../../complex-geometry.md#bott-chern-cohomology). We have constructed the canonical isomorphism and its harmonic inverse:

$$
\boxed{\phi:H_{BC}^{p,q}(M)\xrightarrow{\sim}H_{\bar\partial}^{p,q}(M),\qquad
\phi^{-1}([\alpha]_{\bar\partial})=[h]_{BC}.}
$$

## 2

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose a [flasque resolution](../../../ringed-space.md#flasque-resolution) of the [sheaf of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups) $\mathcal F$,

$$
0\longrightarrow\mathcal F\longrightarrow\mathcal I^0\xrightarrow{d^0}\mathcal I^1\xrightarrow{d^1}\cdots.
$$

A [flasque sheaf](../../../ringed-space.md#flasque-sheaf) has surjective restriction maps; such resolutions exist for every [sheaf of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups). Apply the [global section functor](../../../ringed-space.md#global-section-functor) to obtain a [cochain complex](../../../algebra.md#cochain-complex). The [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) groups are

$$
\boxed{H^i(X,\mathcal F)=
\frac{\ker\bigl(\Gamma(X,\mathcal I^i)\to\Gamma(X,\mathcal I^{i+1})\bigr)}
{\operatorname{im}\bigl(\Gamma(X,\mathcal I^{i-1})\to\Gamma(X,\mathcal I^i)\bigr)}.}
$$

For $i=0$, the denominator is zero and $H^0(X,\mathcal F)=\Gamma(X,\mathcal F)$. Different resolutions give canonically isomorphic groups; the [resolution principle for sheaf cohomology](../../../ringed-space.md#resolution-principle-for-sheaf-cohomology) is what permits other acyclic resolutions to compute these same groups.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\mathcal C^\infty_{\mathbb C}$ be the additive sheaf of complex-valued [smooth functions](../../../analysis.md#smooth-function), and $\mathcal C^{\infty,*}_{\mathbb C}$ its multiplicative sheaf of nowhere-zero functions. The [smooth exponential sequence](../../../fiber-bundle.md#smooth-exponential-sequence) is

$$
0\longrightarrow\underline{\mathbb Z}\longrightarrow\mathcal C^\infty_{\mathbb C}
\xrightarrow{f\mapsto e^{2\pi if}}\mathcal C^{\infty,*}_{\mathbb C}\longrightarrow1.
$$

Its kernel is the integer-valued locally constant functions, namely the integer [constant sheaf](../../../algebraic-geometry.md#constant-sheaf). It is surjective on stalks because a nowhere-zero smooth function has a smooth logarithm on a sufficiently small neighbourhood.

The additive smooth-function sheaf is a [fine sheaf](../../../ringed-space.md#fine-sheaf), using a [partition of unity](../../../differential-geometry.md#partition-of-unity), and the [smooth manifold](../../../differential-geometry.md#smooth-manifold) is a [paracompact space](../../../topology.md#paracompact-space). Its positive-degree [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) vanishes. The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) consequently gives an isomorphism

$$
\delta:H^1(X,\mathcal C^{\infty,*}_{\mathbb C})\xrightarrow{\sim}H^2(X,\mathbb Z).
$$

To connect this with bundles, trivialize a smooth [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) over an open cover. Its transition functions $g_{ij}$ form a multiplicative [Čech cocycle](../../../ringed-space.md#cech-cocycle-condition), satisfying $g_{ij}g_{jk}=g_{ik}$. Changing trivializations changes it by a [Čech coboundary](../../../ringed-space.md#cech-coboundary). Conversely, any such cocycle glues trivial line bundles, and cohomologous cocycles give isomorphic bundles. Thus the isomorphism classes are $H^1(X,\mathcal C^{\infty,*}_{\mathbb C})$.

The connecting isomorphism is the [First Chern class](../../../complex-geometry.md#first-chern-class). Locally choose logarithms $g_{ij}=e^{2\pi if_{ij}}$; on triple intersections

$$
n_{ijk}=f_{ij}+f_{jk}-f_{ik}\in\mathbb Z
$$

represents that class. Combining the gluing classification with $\delta$ gives the requested bijection:

$$
\boxed{\{\text{smooth complex line bundles on }X\}/\cong\ \xrightarrow{\ c_1\ }\ H^2(X,\mathbb Z).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The restriction maps of this point sheaf satisfy the presheaf composition identities: every possible restriction is either the identity on $\mathbb C$ or the unique map to the zero group. We check the sheaf identity and gluing axioms for any open cover $U=\bigcup_iU_i$.

If $p\notin U$, every section group in the cover is zero, so a compatible family has the unique zero gluing. If $p\in U$, at least one $U_i$ contains $p$. For any two members containing $p$, their intersection also contains $p$, and compatibility forces their complex values to be equal, since the restriction maps there are identities. Call the common value $c$. Members not containing $p$ have only the zero section. The section $c\in\mathbb C_p(U)$ restricts to every member of the family, proving existence of a gluing; its restriction to any member containing $p$ determines $c$, proving uniqueness.

This also proves local identity for sections, and $\mathbb C_p(\varnothing)=0$ handles the empty open set. Hence

$$
\boxed{\mathbb C_p\text{ is a sheaf of abelian groups}.}
$$

It is the point-pushforward sheaf, usually called a [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf). Its restrictions are all surjective, so it is also a [flasque sheaf](../../../ringed-space.md#flasque-sheaf). No separation assumption on $X$ is needed for the preceding sheaf-axiom argument.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Evaluation is surjective as a sheaf morphism: near $p$, any prescribed value is supplied by a constant [holomorphic function](../../../complex-analysis.md#holomorphic-function). We therefore have a [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\longrightarrow\mathcal I_p\longrightarrow\mathcal O_X\xrightarrow{\operatorname{ev}_p}\mathbb C_p\longrightarrow0,
$$

where $\mathcal I_p$ is the [point ideal sheaf](../../../complex-geometry.md#ideal-sheaf-of-a-point-on-a-complex-manifold) and $\mathcal O_X$ the [sheaf of holomorphic functions](../../../complex-geometry.md#structure-sheaf-of-a-complex-manifold). By part (c), the [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) is flasque, so $H^0(X,\mathbb C_p)=\mathbb C$ and $H^i(X,\mathbb C_p)=0$ for $i>0$.

On the connected compact [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) makes every global [holomorphic function](../../../complex-analysis.md#holomorphic-function) constant. Consequently $H^0(X,\mathcal O_X)=\mathbb C$, and evaluation on [global sections](../../../ringed-space.md#global-section) is an isomorphism. Also $H^1(X,\mathcal O_X)\cong\mathbb C$: by [Serre duality for compact complex manifolds](../../../ringed-space.md#serre-duality-for-compact-complex-manifolds), its dual is $H^0(X,K_X)$, generated by the nowhere-zero form $dz$ descended from $\mathbb C$. Higher cohomology of $\mathcal O_X$ vanishes by the [Dolbeault theorem](../../../complex-geometry.md#dolbeault-theorem) in complex dimension one.

The [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) thus begins

$$
0\to H^0(X,\mathcal I_p)\to\mathbb C\xrightarrow{\sim}\mathbb C
\to H^1(X,\mathcal I_p)\to\mathbb C\to0.
$$

It follows that

$$
\boxed{H^i(X,\mathcal I_p)\cong
\begin{cases}0,&i=0,\\\mathbb C,&i=1,\\0,&i\geq2.\end{cases}}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [tautological bundle](../../../fiber-bundle.md#tautological-bundle) $\mathcal O(-1)$ over [Complex projective space](../../../algebraic-topology.md#complex-projective-space) has fibre over $[\ell]$ equal to the line $\ell\subset\mathbb C^{r+1}$. Define $\mathcal O(1)=\mathcal O(-1)^*$ and the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space), viewed analytically as a [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle), by

$$
\mathcal O(d)=
\begin{cases}\mathcal O(1)^{\otimes d},&d>0,\\
\mathcal O,&d=0,\\
\mathcal O(-1)^{\otimes(-d)},&d<0.
\end{cases}
$$

For $\mathbb{CP}^1$, use coordinates $z=Z_1/Z_0$ and $w=Z_0/Z_1=1/z$. The tautological frames $(1,z)$ and $(w,1)$ differ by $z^{-1}$, so frames $e_0,e_1$ for $\mathcal O(d)$ satisfy $e_1=z^d e_0$. A global [holomorphic section](../../../complex-geometry.md#holomorphic-section) is therefore described by entire functions $s_0(z),s_1(w)$ with

$$
s_1(w)=w^d s_0(1/w).
$$

Write $s_0(z)=\sum_{k\geq0}a_kz^k$. Holomorphicity of $s_1$ at zero permits only the powers $w^{d-k}$ with $d-k\geq0$. For $d\geq0$, this says $s_0$ is a [polynomial](../../../polynomial.md) of degree at most $d$; for $d<0$, every coefficient must vanish. Equivalently, when $d\geq0$ the sections are [homogeneous polynomials](../../../algebra.md#homogeneous-polynomial) of degree $d$ in $Z_0,Z_1$. Thus

$$
\boxed{\dim_{\mathbb C}H^0(\mathbb{CP}^1,\mathcal O(d))=
\begin{cases}d+1,&d\geq0,\\0,&d<0.\end{cases}}
$$

## 3

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the integral normalization of the [Chern connection](../../../complex-geometry.md#chern-connection) curvature. For a [holomorphic local frame](../../../complex-geometry.md#holomorphic-local-trivialization) $e$, put $h_e=h(e,e)>0$. The [fundamental form of a Hermitian holomorphic line bundle](../../../complex-geometry.md#normalized-curvature-form-of-a-hermitian-holomorphic-line-bundle) is

$$
\boxed{\omega_{(\mathcal L,h)}=\frac{i}{2\pi}F_h
=-\frac{i}{2\pi}\partial\bar\partial\log h_e.}
$$

This follows from the [local formula for the Chern connection on a line bundle](../../../complex-geometry.md#local-formula-for-the-chern-connection-on-a-line-bundle), $F_h=\bar\partial\partial\log h_e$. It is a closed [real (1, 1)-form](../../../complex-geometry.md#real-1-1-form) representing the [First Chern class](../../../complex-geometry.md#first-chern-class). If $h_e=e^{-\varphi}$, the formula becomes $(i/(2\pi))\partial\bar\partial\varphi$.

The [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) is positive when this is a [positive real (1, 1)-form](../../../complex-geometry.md#positive-real-1-1-form): for every nonzero $v\in T^{1,0}M$,

$$
\boxed{-i\omega_{(\mathcal L,h)}(v,\bar v)>0.}
$$

Equivalently, the matrix $(\partial^2\varphi/\partial z_j\partial\bar z_k)$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) in every frame. Such a metric makes $\mathcal L$ a [positive holomorphic line bundle](../../../complex-geometry.md#positive-holomorphic-line-bundle). Omitting the normalization factor $2\pi$ changes none of these positivity conditions.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply [Serre duality for compact complex manifolds](../../../ringed-space.md#serre-duality-for-compact-complex-manifolds) to $\mathcal L\otimes K_M$, where $K_M$ is the [canonical bundle](../../../complex-geometry.md#canonical-bundle):

$$
H^n(M,\mathcal L\otimes K_M)^*\cong H^0(M,\mathcal L^{-1}).
$$

We can show the group on the right vanishes directly from the embedding. Since $\mathcal L^{-1}=i^*\mathcal O(-1)$, the [tautological bundle](../../../fiber-bundle.md#tautological-bundle) inclusion gives an inclusion of [holomorphic vector bundles](../../../complex-geometry.md#holomorphic-vector-bundle)

$$
\mathcal L^{-1}\hookrightarrow M\times\mathbb C^{r+1}.
$$

A global [holomorphic section](../../../complex-geometry.md#holomorphic-section) of $\mathcal L^{-1}$ consequently determines $r+1$ global [holomorphic functions](../../../complex-analysis.md#holomorphic-function) on $M$. [Compactness](../../../topology.md#compact-space) and the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) make these functions constant on every [connected component](../../../geometry-and-topology.md#connected-component). On such a component the section is therefore a constant vector $v$ lying in the tautological line $i(x)$ for every $x$.

If $v\ne0$, all the points $i(x)$ equal $[v]$. This contradicts the fact that $i$ is an embedding of a component of positive dimension $n\geq1$. Hence $v=0$ on every component, and $H^0(M,\mathcal L^{-1})=0$. Duality proves

$$
\boxed{H^n(M,\mathcal L\otimes K_M)=0.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Dolbeault theorem](../../../complex-geometry.md#dolbeault-theorem) identifies $H^2(M,\mathcal O_M)$ with $H^{0,2}_{\bar\partial}(M)$. It vanishes by hypothesis, and [complex conjugation](../../../complex-analysis.md#complex-conjugation) in the [Hodge decomposition theorem for compact Kähler manifolds](../../../complex-geometry.md#hodge-decomposition-theorem-for-compact-kahler-manifolds) makes $H^{2,0}$ vanish too. Thus every real degree-two cohomology class has type $(1,1)$.

Let $\omega$ be a Kähler form. Choose a rational cohomology class $\eta$ sufficiently close to $[\omega]$. More concretely, using [harmonic differential forms](../../../differential-form.md#harmonic-differential-form) as representatives for a fixed [Kähler metric](../../../complex-geometry.md#kahler-metric), the harmonic form representing $\eta$ is close to $\omega$ in every smooth norm: [harmonic differential forms](../../../differential-form.md#harmonic-differential-form) constitute a [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space). It is a real closed $(1,1)$ form, and is positive if sufficiently close to $\omega$, by [compactness](../../../topology.md#compact-space). This is the openness of the [Kähler cone](../../../complex-geometry.md#kahler-cone). Multiplying by a positive integer gives an integral Kähler class $\kappa=N\eta$.

The [holomorphic exponential sequence](../../../complex-geometry.md#holomorphic-exponential-sequence) contains the cohomology segment

$$
H^1(M,\mathcal O_M^*)\xrightarrow{c_1}H^2(M,\mathbb Z)\longrightarrow H^2(M,\mathcal O_M)=0.
$$

Choose an integral lift of $\kappa$. Exactness gives a [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle) $\mathcal L$ having that [First Chern class](../../../complex-geometry.md#first-chern-class). We must ensure that it has a positive metric, rather than merely a positive representative of its class.

Choose any [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) $h_0$ and let $\theta_0$ be its [normalized curvature form of a Hermitian holomorphic line bundle](../../../complex-geometry.md#normalized-curvature-form-of-a-hermitian-holomorphic-line-bundle). If $\theta$ is the positive form representing $\kappa$, then $\theta-\theta_0$ is an exact real $(1,1)$ form. The [ddbar lemma](../../../complex-geometry.md#ddbar-lemma) gives a real smooth function $u$ with

$$
\theta-\theta_0=\frac{i}{2\pi}\partial\bar\partial u.
$$

Replace $h_0$ by $h=e^{-u}h_0$. Its normalized curvature is $\theta$, so $\mathcal L$ is a [positive holomorphic line bundle](../../../complex-geometry.md#positive-holomorphic-line-bundle). The [Kodaira embedding theorem](../../../complex-geometry.md#kodaira-embedding-theorem) now applies: sufficiently many sections of a sufficiently high [tensor power](../../../linear-algebra.md#tensor-power) define the desired embedding. Therefore

$$
\boxed{H^2(M,\mathcal O_M)=0\ \Longrightarrow\ M\text{ admits a holomorphic embedding into complex projective space}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For the [Calabi-Yau threefold](../../../complex-geometry.md#calabi-yau-threefold) in the stated convention, the [Hodge decomposition theorem for compact Kähler manifolds](../../../complex-geometry.md#hodge-decomposition-theorem-for-compact-kahler-manifolds) gives

$$
0=H^1(M,\mathbb C)=H^{1,0}_{\bar\partial}(M)\oplus H^{0,1}_{\bar\partial}(M).
$$

In particular, the [Dolbeault theorem](../../../complex-geometry.md#dolbeault-theorem) yields $H^1(M,\mathcal O_M)=0$. By [Serre duality for compact complex manifolds](../../../ringed-space.md#serre-duality-for-compact-complex-manifolds) in dimension three,

$$
H^2(M,\mathcal O_M)^*\cong H^1(M,K_M).
$$

The [canonical bundle](../../../complex-geometry.md#canonical-bundle) is trivial, so the group on the right equals $H^1(M,\mathcal O_M)=0$. Thus $H^2(M,\mathcal O_M)=0$, and part (c) gives

$$
\boxed{\text{Every Calabi-Yau threefold satisfying the given definition is projective}.}
$$

## 4

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\omega$ be the Kähler form associated with the metric. The [Lefschetz operator of a Kähler manifold](../../../complex-geometry.md#lefschetz-operator-of-a-kahler-manifold) and [adjoint Lefschetz operator](../../../complex-geometry.md#adjoint-lefschetz-operator) are

$$
\boxed{L\alpha=\omega\wedge\alpha,\qquad\Lambda=L^*.}
$$

Here the adjoint is taken with respect to the pointwise [Hermitian inner product](../../../linear-algebra.md#hermitian-form) on complexified forms, or equivalently the global $L^2$ inner product. It lowers degree by two and bidegree by $(1,1)$. In terms of the [Hodge star operator](../../../differential-form.md#hodge-star-operator), $\Lambda=*^{-1}L*$.

Since $d\omega=0$, $dL=Ld$, so $L$ takes [closed differential forms](../../../differential-form.md#closed-differential-form) to [closed differential forms](../../../differential-form.md#closed-differential-form) and [exact differential forms](../../../differential-form.md#exact-differential-form) to [exact differential forms](../../../differential-form.md#exact-differential-form). This already gives its action on [de Rham cohomology](../../../differential-form.md#de-rham-cohomology). For both operators together, use the [Kähler identities](../../../complex-geometry.md#kahler-identities): $L$ commutes with the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian), and taking adjoints shows that $\Lambda$ does too. Thus both preserve [harmonic differential forms](../../../differential-form.md#harmonic-differential-form).

When $M$ is compact, the [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) identifies $H^k(M,\mathbb C)$ with its space of harmonic $k$-forms. If $h_\alpha$ is the unique [harmonic differential form](../../../differential-form.md#harmonic-differential-form) representing $[\alpha]$, define

$$
\boxed{L[\alpha]=[Lh_\alpha],\qquad\Lambda[\alpha]=[\Lambda h_\alpha].}
$$

The resulting forms are harmonic and therefore closed, and uniqueness of $h_\alpha$ makes these definitions independent of the initial representative. The cohomological definition of $\Lambda$ uses [harmonic differential forms](../../../differential-form.md#harmonic-differential-form) as representatives: $\Lambda$ need not take an arbitrary closed form to a closed form.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Represent the middle-degree class by its unique [harmonic differential form](../../../differential-form.md#harmonic-differential-form) $h$. The [Lefschetz commutator](../../../complex-geometry.md#lefschetz-commutator) on degree $k$ is $[\Lambda,L]=(n-k)\operatorname{id}$, so at $k=n$ the operators commute. Since the [adjoint Lefschetz operator](../../../complex-geometry.md#adjoint-lefschetz-operator) is the adjoint of the [Lefschetz operator of a Kähler manifold](../../../complex-geometry.md#lefschetz-operator-of-a-kahler-manifold),

$$
\|Lh\|^2=\langle\Lambda Lh,h\rangle
=\langle L\Lambda h,h\rangle=\|\Lambda h\|^2.
$$

Both $Lh$ and $\Lambda h$ are harmonic. A harmonic form represents zero in [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) exactly when the form itself is zero. Consequently $L[\alpha]=0$ if and only if $Lh=0$, which by the norm identity is equivalent to $\Lambda h=0$, hence to $\Lambda[\alpha]=0$. Therefore

$$
\boxed{\alpha\in H^n(M,\mathbb C)\text{ is primitive}\ \Longleftrightarrow\ \Lambda\alpha=0.}
$$

This identifies the two middle-degree descriptions of a [primitive differential form on a Kähler manifold](../../../complex-geometry.md#primitive-differential-form-on-a-kahler-manifold) at the cohomology level.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The assertion is pointwise, so choose an oriented orthonormal real coframe $x_1,y_1,x_2,y_2$ compatible with the complex structure, with Kähler form $\omega=x_1\wedge y_1+x_2\wedge y_2$. Real $(1,1)$ forms have a four-dimensional space; imposing $\omega\wedge\alpha=0$ leaves the three-dimensional space spanned by

$$
\begin{aligned}
A&=x_1\wedge y_1-x_2\wedge y_2,\\
B&=x_1\wedge x_2+y_1\wedge y_2,\\
C&=x_1\wedge y_2-y_1\wedge x_2.
\end{aligned}
$$

These are precisely the real [primitive differential forms on a Kähler manifold](../../../complex-geometry.md#primitive-differential-form-on-a-kahler-manifold) of type $(1,1)$ in dimension two. Complexifying spans all complex primitive $(1,1)$ forms.

Using the complex orientation $x_1\wedge y_1\wedge x_2\wedge y_2$, the [Hodge star operator](../../../differential-form.md#hodge-star-operator) exchanges $x_1\wedge y_1$ with $x_2\wedge y_2$, sends $x_1\wedge x_2$ to $-y_1\wedge y_2$, and exchanges $x_1\wedge y_2$ with $y_1\wedge x_2$. Thus $*A=-A$, $*B=-B$, and $*C=-C$. By complex linearity,

$$
\boxed{*\alpha=-\alpha.}
$$

This is the fact that [primitive (1,1)-forms on a Kähler surface are anti-self-dual](../../../complex-geometry.md#primitive-1-1-forms-on-a-kahler-surface-are-anti-self-dual).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use the usual connected-manifold convention for this assertion. Suppose, for contradiction, that $H^2(M,\mathcal O_M)=0$. The [Dolbeault theorem](../../../complex-geometry.md#dolbeault-theorem) gives $H^{0,2}=0$, and the [Hodge decomposition theorem for compact Kähler manifolds](../../../complex-geometry.md#hodge-decomposition-theorem-for-compact-kahler-manifolds) and its conjugation symmetry give $H^{2,0}=0$. Hence every real class in $H^2(M,\mathbb R)$ has a real [harmonic differential form](../../../differential-form.md#harmonic-differential-form) of type $(1,1)$ as its representative.

The [intersection form](../../../homology.md#intersection-form) is $Q([u],[v])=\int_Mu\wedge v$. Its value on the Kähler class is positive: $Q([\omega],[\omega])=\int_M\omega^2>0$. Every real harmonic $(1,1)$ form splits uniquely as $c\omega+u_0$, with $u_0$ primitive and $c$ constant. Indeed, $\Lambda u$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function), hence constant by [connectedness](../../../geometry-and-topology.md#connected-space), and $\Lambda\omega=2$; subtracting $c\omega$ kills $\Lambda u$, and part (b) makes $u_0$ primitive.

Part (c) gives $*u_0=-u_0$, while $\omega\wedge u_0=0$. Thus

$$
Q([\omega],[u_0])=0,\qquad Q([u_0],[u_0])=-\|u_0\|_{L^2}^2<0\quad(u_0\ne0).
$$

This proves the [Hodge index theorem for compact Kähler surfaces](../../../complex-geometry.md#hodge-index-theorem-for-compact-kahler-surfaces) in this case: $Q$ has [signature](../../../linear-algebra.md#signature-of-a-quadratic-form) $(1,b_2-1)$.

On the alleged two-dimensional [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace) $V$, the [linear functional](../../../linear-algebra.md#linear-functional) $v\mapsto Q(v,[\omega])$ has a nonzero vector in its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). Its [harmonic differential form](../../../differential-form.md#harmonic-differential-form) representative is primitive, so the preceding negative-definiteness statement gives $Q(v,v)<0$, contradicting the vanishing of $Q$ on $V$. Therefore

$$
\boxed{\dim_{\mathbb R}V=2,\quad Q|_{V\otimes V}=0\ \Longrightarrow\ H^2(M,\mathcal O_M)\ne0.}
$$

[Connectedness](../../../geometry-and-topology.md#connected-space) is essential if one's definition of a manifold allows disconnected spaces. For $M=Y\sqcup Y$, with $Y=\mathbb{CP}^1\times\mathbb{CP}^1$, one has $H^2(M,\mathcal O_M)=0$. Take on each component the pullback of the degree-two class from its first factor. Each class has square zero, and their mutual pairing is zero because their supports lie on different components. Their span is then a two-dimensional [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace), disproving the unqualified disconnected version.

## 5

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) $\alpha$ of type $(p,0)$ satisfies $\bar\partial\alpha=0$. The adjoint $\bar\partial^*$ lowers antiholomorphic degree, so $\bar\partial^*\alpha=0$ as well. Therefore $\Delta_{\bar\partial}\alpha=0$.

The [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity) gives $\Delta_d\alpha=2\Delta_{\bar\partial}\alpha=0$. [Compactness](../../../topology.md#compact-space) lets us use the $L^2$ identity for the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian):

$$
0=\langle\Delta_d\alpha,\alpha\rangle
=\|d\alpha\|^2+\|d^*\alpha\|^2.
$$

Both terms are nonnegative, so

$$
\boxed{d\alpha=0.}
$$

This proves that [holomorphic forms on a compact Kähler manifold are closed](../../../complex-geometry.md#holomorphic-forms-on-a-compact-kahler-manifold-are-closed). The original PDF uses $\Omega_M^p$ and $\mathcal A_{M,\mathbb C}^{p+1}$; the extra symbols in the local TeX superscripts are transcription errors.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [holomorphic de Rham complex](../../../complex-geometry.md#holomorphic-de-rham-complex) is exact locally, which is the criterion for an [exact sequence of sheaves](../../../algebraic-geometry.md#exact-sequence-of-sheaves). Work in a small star-shaped [holomorphic coordinate](../../../complex-geometry.md#holomorphic-coordinate) neighbourhood in $\mathbb C^2$, centred at zero. A [holomorphic function](../../../complex-analysis.md#holomorphic-function) has $\partial f=0$ exactly when it is constant on this neighbourhood, giving exactness at $\mathcal O_M$ and the injection of the [constant sheaf](../../../algebraic-geometry.md#constant-sheaf).

For exactness at $\Omega_M^1$, let $\alpha=a_1(z)\,dz_1+a_2(z)\,dz_2$ be holomorphic and $\partial$-closed. Then $\partial a_1/\partial z_2=\partial a_2/\partial z_1$. Define the [holomorphic function](../../../complex-analysis.md#holomorphic-function)

$$
F(z)=\int_0^1\bigl(z_1a_1(tz)+z_2a_2(tz)\bigr)\,dt.
$$

Differentiation under the integral and the closedness identity give

$$
\frac{\partial F}{\partial z_j}
=\int_0^1\left(a_j(tz)+t\sum_i z_i\frac{\partial a_j}{\partial z_i}(tz)\right)dt
=[t\,a_j(tz)]_{t=0}^{t=1}=a_j(z).
$$

Thus $\partial F=\alpha$.

For exactness at $\Omega_M^2$, any [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) of degree two is $\beta=b(z)\,dz_1\wedge dz_2$ and is automatically $\partial$-closed by dimension. Define

$$
\gamma(z)=\int_0^1 t\,b(tz)(z_1\,dz_2-z_2\,dz_1)\,dt.
$$

Its derivative is

$$
\partial\gamma
=\int_0^1\left(2t\,b(tz)+t^2\sum_i z_i\frac{\partial b}{\partial z_i}(tz)\right)dt\,dz_1\wedge dz_2
=[t^2b(tz)]_0^1\,dz_1\wedge dz_2=\beta.
$$

These local primitives prove the [holomorphic Poincaré lemma](../../../complex-geometry.md#holomorphic-poincare-lemma) in the degrees needed here. Exactness on every stalk gives

$$
\boxed{0\longrightarrow\underline{\mathbb C}\longrightarrow\mathcal O_M
\xrightarrow{\partial}\Omega_M^1\xrightarrow{\partial}\Omega_M^2\longrightarrow0.}
$$

This is sheaf exactness; the local primitives need not glue to global ones.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For degree zero, [compactness](../../../topology.md#compact-space) and the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) make [holomorphic functions](../../../complex-analysis.md#holomorphic-function) constant on each [connected component](../../../geometry-and-topology.md#connected-component). For degree two, a [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) is $\bar\partial$-closed and its $\partial$ derivative has type $(3,0)$, which vanishes on a complex surface. Degrees above two have no nonzero holomorphic forms. It remains to treat a [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) $\alpha$ of degree one.

Set $\beta=d\alpha=\partial\alpha$. Its coefficients are holomorphic, so $\beta$ is a [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) of degree two, hence closed by the degree-two observation. Its conjugate is closed too. The [Stokes theorem](../../../calculus.md#stokes-theorem) gives

$$
\int_M\beta\wedge\bar\beta
=\int_Md(\alpha\wedge\bar\beta)=0.
$$

The integrand is nonnegative in the complex orientation. In local coordinates, if $\beta=b(z)\,dz_1\wedge dz_2$ with $z_j=x_j+iy_j$, then

$$
\beta\wedge\bar\beta
=4|b(z)|^2\,dx_1\wedge dy_1\wedge dx_2\wedge dy_2.
$$

It is strictly positive wherever $\beta$ is nonzero. Its zero integral therefore forces $\beta=0$ everywhere. Thus [holomorphic forms on a compact complex surface are closed](../../../complex-geometry.md#holomorphic-forms-on-a-compact-complex-surface-are-closed), even when the surface is not Kähler:

$$
\boxed{d\alpha=0\quad\text{for every global holomorphic }p\text{-form}.}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Let $\mathcal Z_M^1$ be the [sheaf of closed holomorphic one-forms](../../../complex-geometry.md#sheaf-of-closed-holomorphic-one-forms), namely $\ker(\partial:\Omega_M^1\to\Omega_M^2)$. The local exactness proved in part (b) gives the [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\longrightarrow\underline{\mathbb C}\longrightarrow\mathcal O_M\xrightarrow{\partial}\mathcal Z_M^1\longrightarrow0.
$$

Its [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) begins

$$
H^0(M,\mathbb C)\longrightarrow H^0(M,\mathcal O_M)
\longrightarrow H^0(M,\mathcal Z_M^1)
\xrightarrow{\delta}H^1(M,\mathbb C)\longrightarrow H^1(M,\mathcal O_M).
$$

The first arrow is an isomorphism: on a compact [complex manifold](../../../complex-geometry.md#complex-manifold), a global [holomorphic function](../../../complex-analysis.md#holomorphic-function) is constant on each [connected component](../../../geometry-and-topology.md#connected-component), just as a global section of the [constant sheaf](../../../algebraic-geometry.md#constant-sheaf) is. Thus $\delta$ is injective. By part (c), every global [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) of degree one is closed, so $H^0(M,\mathcal Z_M^1)=H^0(M,\Omega_M^1)$.

Concretely, for a [holomorphic differential form](../../../complex-geometry.md#holomorphic-differential-form) of degree one choose local holomorphic primitives $f_i$. The connecting class $\delta(\alpha)$ is represented by the locally constant [Čech cocycle](../../../ringed-space.md#cech-cocycle-condition) $f_j-f_i$ on overlaps. The following arrow is induced by the inclusion of the [constant sheaf](../../../algebraic-geometry.md#constant-sheaf) into the [sheaf of holomorphic functions](../../../complex-geometry.md#structure-sheaf-of-a-complex-manifold). Exactness is inherited from the long exact sequence, giving

$$
\boxed{0\longrightarrow H^0(M,\Omega_M^1)\xrightarrow{\delta}H^1(M,\mathbb C)
\longrightarrow H^1(M,\mathcal O_M).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
