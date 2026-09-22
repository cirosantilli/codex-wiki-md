# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_203.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $\mathbb H=\{z:\operatorname{Im}z>0\}$. A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded, relatively closed set $A\subseteq\mathbb H$ for which $D_A=\mathbb H\setminus A$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). “Compact” refers to its compact [closure](../../../topology.md#closure-topology) in $\overline{\mathbb H}$; [boundary](../../../topology.md#boundary-of-a-set) points on $\mathbb R$ can be adjoined without changing the remaining [domain](../../../topology.md#domain-mathematical-analysis).

The [Riemann mapping theorem](../../../complex-analysis.md#riemann-mapping-theorem) and normalization at infinity give a unique [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) $g_A:D_A\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity). By the [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) outside a large disc, it has the [Laurent series](../../../analysis.md#laurent-series)

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}),\qquad a\in\mathbb R.
$$

The [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is the coefficient

$$
\boxed{\operatorname{hcap}(A)=a.}
$$

The empty [compact H-hull](../../../stochastic-process.md#compact-h-hull) has $g_A(z)=z$ and [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) zero. Nonnegativity follows from the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) proved next.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $u(z)=\operatorname{Im}(z-g_A(z))$ on $D_A$. This is a [harmonic function](../../../partial-differential-equation.md#harmonic-function), tends to zero at infinity, and is bounded. To justify the [boundary](../../../topology.md#boundary-of-a-set) behavior without requiring a [locally connected space](../../../topology.md#locally-connected-space) as its [boundary](../../../topology.md#boundary-of-a-set), let $f_A=g_A^{-1}$. Its expansion at infinity implies that bounded $z$ cannot have $|g_A(z)|\to\infty$. If $z_n$ approaches a finite point of $\partial D_A$ and $g_A(z_n)$ had a subsequential limit inside $\mathbb H$, [continuity](../../../calculus.md#continuous-function) of $f_A$ would force that point to lie inside $D_A$, a contradiction. Thus [boundary degeneration under a mapping-out function](../../../stochastic-process.md#boundary-degeneration-under-a-mapping-out-function) gives $\operatorname{Im}g_A(z_n)\to0$. Consequently $u$ extends continuously to the finite [boundary](../../../topology.md#boundary-of-a-set) with value $\operatorname{Im}z$.

Let $B$ be [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $z\in D_A$, and $\tau$ its [Brownian exit time](../../../brownian-motion.md#brownian-exit-time) from $D_A$. This time is finite almost surely: it is at most the first time the imaginary coordinate, a one-dimensional [Brownian motion](../../../brownian-motion.md), hits zero. By the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), $u(B_{t\wedge\tau})$ is a bounded [martingale](../../../martingale.md). The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) and [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore give

$$
u(z)=\mathbb E_z[u(B_\tau)]=\mathbb E_z[\operatorname{Im}B_\tau].
$$

Boundedness is important here: directly stopping the unbounded imaginary-coordinate [martingale](../../../martingale.md) would require an unjustified [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) assertion.

At $z=iy$, the [Laurent series](../../../analysis.md#laurent-series) gives $u(iy)=a/y+O(y^{-2})$. Hence

$$
\boxed{\operatorname{hcap}(A)=\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau]\geq0.}
$$

The sign follows because the exit point lies on $\partial D_A\subseteq\overline{\mathbb H}$. This proves the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $x\in\mathbb R$, the [conformal map](../../../geometry-and-topology.md#conformal-map)

$$
h(z)=x+g_A(z-x)
$$

maps $\mathbb H\setminus(A+x)$ onto $\mathbb H$ and has [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity). Its [Laurent series](../../../analysis.md#laurent-series) is $h(z)=z+a/z+O(z^{-2})$. Uniqueness of the [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) therefore gives

$$
\boxed{\operatorname{hcap}(A+x)=\operatorname{hcap}(A).}
$$

This is the translation part of [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity).

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

For $r>0$, the [conformal map](../../../geometry-and-topology.md#conformal-map) $h(z)=r g_A(z/r)$ maps $\mathbb H\setminus rA$ onto $\mathbb H$ and has [Laurent series](../../../analysis.md#laurent-series) $h(z)=z+r^2a/z+O(z^{-2})$. The uniqueness in [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) gives

$$
\boxed{\operatorname{hcap}(rA)=r^2\operatorname{hcap}(A).}
$$

At $r=0$ the scaled [closure](../../../topology.md#closure-topology) is contained in $\mathbb R$, so the [interior](../../../topology.md#interior-topology) [compact H-hull](../../../stochastic-process.md#compact-h-hull) is empty and both sides are zero. This is the scaling part of [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity).

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Suppose $A\subseteq B$. Map out $A$ and let $C$ be the relatively closed image hull corresponding to $g_A(B\setminus A)$, with bounded complementary components filled if needed. Then $g_A$ maps $\mathbb H\setminus B$ onto $\mathbb H\setminus C$. Uniqueness of the [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) gives $g_B=g_C\circ g_A$. Comparing their [Laurent series](../../../analysis.md#laurent-series) yields the [half-plane-capacity composition rule](../../../stochastic-process.md#half-plane-capacity-composition-rule)

$$
\operatorname{hcap}(B)=\operatorname{hcap}(A)+\operatorname{hcap}(C).
$$

The [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) makes the last term nonnegative, proving [monotonicity of half-plane capacity](../../../stochastic-process.md#monotonicity-of-half-plane-capacity):

$$
\boxed{\operatorname{hcap}(A)\leq\operatorname{hcap}(B).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For the vertical slit, choose the branch of $\sqrt{z^2+1}$ asymptotic to $z$ at infinity. It is the [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) for $(0,i]$, and

$$
\sqrt{z^2+1}=z+\frac1{2z}+O(z^{-3}).
$$

Thus [half-plane capacity of a vertical slit](../../../stochastic-process.md#half-plane-capacity-of-a-vertical-slit) gives

$$
\boxed{\operatorname{hcap}([0,i])=\frac12.}
$$

The endpoint $0$ is merely part of the [boundary](../../../topology.md#boundary-of-a-set) [closure](../../../topology.md#closure-topology) convention.

For the filled upper half-disc $K=\{z\in\mathbb H:|z|\leq1\}$, the [conformal map](../../../geometry-and-topology.md#conformal-map) $g_K(z)=z+1/z$ maps the exterior half-disc onto $\mathbb H$. Indeed, it sends the semicircle to $[-2,2]$, the remaining real [boundary](../../../topology.md#boundary-of-a-set) to the complementary intervals, and its inverse is the branch of $(w+\sqrt{w^2-4})/2$ asymptotic to $w$. Hence [half-plane capacity of a half-disc](../../../stochastic-process.md#half-plane-capacity-of-a-half-disc) gives

$$
\boxed{\operatorname{hcap}(K)=1.}
$$

If $\mathbb D$ denotes the open [unit disc](../../../topology.md#unit-disc), the printed $\mathbb H\cap\mathbb D$ is not relatively closed and is literally not a [compact H-hull](../../../stochastic-process.md#compact-h-hull). The intended value is the one for its filled relative [closure](../../../topology.md#closure-topology) $K$. With a closed-disc convention the displayed notation already represents that hull.

For a nonempty [compact H-hull](../../../stochastic-process.md#compact-h-hull) $A$, its [closure](../../../topology.md#closure-topology) meets $\mathbb R$: otherwise a nonempty [compact set](../../../topology.md#compact-space) strictly inside $\mathbb H$ would be separated from the lower half-plane in the complement, contradicting the [simply connected domain](../../../complex-analysis.md#simply-connected-domain) condition for $\mathbb H\setminus A$. Choose $x\in\overline A\cap\mathbb R$ and put $d=\operatorname{diam}(A)$. Taking limits in the definition of [diameter](../../../topological-analysis.md#diameter) shows $|z-x|\leq d$ for every $z\in A$. Thus $A$ lies in the filled half-disc of radius $d$ centered at $x$. Its [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is $d^2$ by [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity). Using [monotonicity of half-plane capacity](../../../stochastic-process.md#monotonicity-of-half-plane-capacity),

$$
\boxed{\operatorname{hcap}(A)\leq\operatorname{diam}(A)^2.}
$$

For the empty [compact H-hull](../../../stochastic-process.md#compact-h-hull), use [diameter](../../../topological-analysis.md#diameter) zero. This proves the unit-constant version of [half-plane capacity is bounded by squared diameter](../../../stochastic-process.md#half-plane-capacity-is-bounded-by-squared-diameter); no claim of optimality of the constant is needed.

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A family $(K_t)_{t\geq0}$ of [compact H-hulls](../../../stochastic-process.md#compact-h-hull) is non-decreasing when

$$
\boxed{K_s\subseteq K_t\quad\text{whenever }0\leq s\leq t.}
$$

This permits equal hulls at different times. A [Loewner chain](../../../stochastic-process.md#loewner-chain) with strictly increasing [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) has strict inclusion for $s<t$. Usually its initial [compact H-hull](../../../stochastic-process.md#compact-h-hull) is $K_0=\varnothing$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Write $g_s=g_{K_s}$ and let $K_{s,t}$ be the relatively closed hull obtained by mapping the increment $K_t\setminus K_s$ through $g_s$. For a bounded [compact H-hull](../../../stochastic-process.md#compact-h-hull) $L$, define

$$
\operatorname{rad}(L)=\inf_{x\in\mathbb R}\sup_{z\in L}|z-x|,\qquad \operatorname{rad}(\varnothing)=0.
$$

The [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) is

$$
\boxed{\lim_{h\downarrow0}\sup_{0\leq t\leq T}\operatorname{rad}(K_{t,t+h})=0\quad\text{for every finite }T.}
$$

One can equivalently use [diameter](../../../topological-analysis.md#diameter): for a nonempty [compact H-hull](../../../stochastic-process.md#compact-h-hull), $\operatorname{diam}(L)\leq2\operatorname{rad}(L)\leq2\operatorname{diam}(L)$, using a point of its [closure](../../../topology.md#closure-topology) on $\mathbb R$ for the second inequality. The condition concerns the mapped increment, not the original difference $K_{t+h}\setminus K_t$, which can be large when a narrow opening closes. It makes growth occur near one continuous [Loewner driving function](../../../stochastic-process.md#loewner-driving-function) rather than by a sudden addition at separated [boundary](../../../topology.md#boundary-of-a-set) points.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

With the normalization used in the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation), [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) means

$$
\boxed{\operatorname{hcap}(K_t)=2t,\qquad g_t(z)=z+\frac{2t}{z}+O(z^{-2}).}
$$

Thus $K_0$ is empty and the [half-plane-capacity composition rule](../../../stochastic-process.md#half-plane-capacity-composition-rule) gives $\operatorname{hcap}(K_{s,t})=2(t-s)$. The factor two produces $\partial_tg_t(z)=2/(g_t(z)-U_t)$. A convention using [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) $t$ instead changes that coefficient to one and rescales time; the convention must be kept consistent.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**The implication is false**. Take the thin rectangles

$$
A_\varepsilon=\{x+iy:-1\leq x\leq1,\ 0<y\leq\varepsilon\},\qquad 0<\varepsilon\leq1.
$$

Each is a [compact H-hull](../../../stochastic-process.md#compact-h-hull), and $\operatorname{diam}(A_\varepsilon)=\sqrt{4+\varepsilon^2}\to2$. We verify that its [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) nevertheless tends to zero.

Let $K=\{z\in\mathbb H:|z|\leq2\}$, which contains all these rectangles. At the [Brownian exit time](../../../brownian-motion.md#brownian-exit-time) $\tau$ from $\mathbb H\setminus A_\varepsilon$, the exit height is at most $\varepsilon$, and a positive exit height requires hitting $K$ before $\mathbb R$. Therefore

$$
\mathbb E_{iy}[\operatorname{Im}B_\tau]\leq\varepsilon\,\mathbb P_{iy}(B\text{ hits }K\text{ before }\mathbb R).
$$

For $y>2$, [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) and $g_K(z)=z+4/z$ identify the probability on the right with the [harmonic measure](../../../brownian-motion.md#harmonic-measure) of $[-4,4]$ from $i(y-4/y)$ in $\mathbb H$. Integrating the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) gives

$$
\mathbb P_{iy}(B\text{ hits }K\text{ before }\mathbb R)=\frac2\pi\arctan\frac4{y-4/y},\qquad \lim_{y\to\infty}y\,\mathbb P_{iy}(B\text{ hits }K\text{ before }\mathbb R)=\frac8\pi.
$$

The [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) now proves the explicit estimate

$$
\boxed{0\leq\operatorname{hcap}(A_\varepsilon)\leq\frac8\pi\varepsilon\longrightarrow0,\qquad \operatorname{diam}(A_\varepsilon)\longrightarrow2.}
$$

Choose $\varepsilon=1/n$ to obtain the required sequence. This is an instance of [half-plane capacity of a low rectangle](../../../stochastic-process.md#half-plane-capacity-of-a-low-rectangle): shrinking height can make [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) small while horizontal extent stays fixed.

<a id="2/b/image-half-plane-capacities-of-a-slit-half-disc-and-thin-rectangle"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203-capacity-examples.png)

**[Figure 1](#2/b/image-half-plane-capacities-of-a-slit-half-disc-and-thin-rectangle). Half-plane capacities of a slit, half-disc and thin rectangle**. Two explicit [half-plane capacities](../../../stochastic-process.md#half-plane-capacity) and a thin [compact H-hull](../../../stochastic-process.md#compact-h-hull) with fixed width and vanishing [half-plane capacity](../../../stochastic-process.md#half-plane-capacity).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For real [smooth functions](../../../analysis.md#smooth-function) of [compact support](../../../function.md#compact-support) in a planar [domain](../../../topology.md#domain-mathematical-analysis) $D$, use the [Dirichlet inner product](../../../sobolev-space.md#dirichlet-inner-product)

$$
\boxed{(u,v)_{\nabla,D}=\frac1{2\pi}\int_D\nabla u\cdot\nabla v\,dA.}
$$

Changing the positive normalization factor does not change [orthogonality](../../../linear-algebra.md#orthogonal-vectors). For complex functions, insert [complex conjugation](../../../complex-analysis.md#complex-conjugation) in the second factor to obtain the corresponding [Hermitian form](../../../linear-algebra.md#hermitian-form).

Let $f:D\to\widetilde D$ be a [conformal bijection](../../../complex-analysis.md#biholomorphism), and let $\widetilde u,\widetilde v$ be [smooth functions](../../../analysis.md#smooth-function) of [compact support](../../../function.md#compact-support) on $\widetilde D$. Its real [Jacobian matrix](../../../calculus.md#jacobian-matrix) is $Df=|f'|R$, where $R$ is a rotation. By the [chain rule](../../../calculus.md#chain-rule),

$$
\nabla(\widetilde u\circ f)\cdot\nabla(\widetilde v\circ f)=|f'|^2(\nabla\widetilde u\cdot\nabla\widetilde v)\circ f.
$$

The [change of variables formula](../../../calculus.md#change-of-variables-formula) has [Jacobian determinant](../../../calculus.md#jacobian-determinant) $|f'|^2$, so this factor cancels:

$$
\boxed{(\widetilde u\circ f,\widetilde v\circ f)_{\nabla,D}=(\widetilde u,\widetilde v)_{\nabla,\widetilde D}.}
$$

This proves [conformal invariance of the planar Dirichlet inner product](../../../sobolev-space.md#conformal-invariance-of-the-planar-dirichlet-inner-product). By completion it is also an [isometry](../../../riemannian-geometry.md#isometry) between the corresponding [Dirichlet energy spaces](../../../sobolev-space.md#dirichlet-energy-space). It asserts invariance of the energy form, not of the inhomogeneous [Sobolev norm](../../../sobolev-space.md#sobolev-norm), whose $L^2$ term has a different transformation rule.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Using the usual [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) convention,

$$
H_0^1(D)=\overline{C_c^\infty(D)}^{\,H^1(D)},\qquad \|u\|_{H^1(D)}^2=\int_D(|u|^2+|\nabla u|^2)\,dA,
$$

where [weak derivatives](../../../distribution-theory.md#weak-derivative) define $H^1(D)$ and $C_c^\infty(D)$ is the [space of test functions](../../../distribution-theory.md#space-of-test-functions). In the [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) convention, the same notation often denotes the [Dirichlet energy space](../../../sobolev-space.md#dirichlet-energy-space), the completion in the [gradient](../../../calculus.md#gradient) [norm](../../../functional-analysis.md#norm) alone. On bounded [domains](../../../topology.md#domain-mathematical-analysis) the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) makes the two definitions equivalent; on unbounded [domains](../../../topology.md#domain-mathematical-analysis) one must distinguish them. The following gradient-pairing argument applies in either setting whenever the energy completion is realized as weak functions.

Identify $H_{\mathrm{supp}}=H_0^1(U)$ with a [vector subspace](../../../vector-space.md#vector-subspace) of $H_0^1(D)$ by [zero extension of H01](../../../sobolev-space.md#zero-extension-of-h01). Approximating by [test functions](../../../distribution-theory.md#test-function) in $U$ shows that this is an [isometric embedding](../../../riemannian-geometry.md#isometric-embedding) in the inhomogeneous [Sobolev norm](../../../sobolev-space.md#sobolev-norm) and also in the [Dirichlet inner product](../../../sobolev-space.md#dirichlet-inner-product) [norm](../../../functional-analysis.md#norm). In particular, arbitrary irregularity of $\partial U$ causes no additional [boundary](../../../topology.md#boundary-of-a-set) term.

Define

$$
H_{\mathrm{harm}}=\{h\in H_0^1(D):\Delta h=0\text{ in distributions on }U\}.
$$

These are [weakly harmonic Sobolev functions](../../../partial-differential-equation.md#weakly-harmonic-sobolev-function). For $\phi\in C_c^\infty(U)$, [integration by parts](../../../calculus.md#integration-by-parts) in the weak sense gives $\int_U\nabla h\cdot\nabla\phi\,dA=0$. If $u\in H_{\mathrm{supp}}$, choose $\phi_n\in C_c^\infty(U)$ converging to $u$ in $H^1(U)$, or in energy for the homogeneous convention. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
(h,u)_{\nabla,D}=\lim_{n\to\infty}(h,\phi_n)_{\nabla,D}=0.
$$

Hence the [orthogonality of supported and harmonic Dirichlet functions](../../../sobolev-space.md#orthogonality-of-supported-and-harmonic-dirichlet-functions) is

$$
\boxed{H_{\mathrm{supp}}\perp H_{\mathrm{harm}}.}
$$

Both are linear [vector subspaces](../../../vector-space.md#vector-subspace). In the inhomogeneous convention they are closed: the first is the isometric image of a complete space, and the second is the intersection of the kernels of the [linear functionals](../../../linear-algebra.md#linear-functional) $h\mapsto(h,\phi)_\nabla$. No spanning assertion is needed. The PDF contains this [orthogonality](../../../linear-algebra.md#orthogonal-vectors) statement; the TeX has badly corrupted it into an assertion about openness.

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Koebe quarter theorem](../../../complex-analysis.md#koebe-quarter-theorem) says that if $F:\mathbb D\to\mathbb C$ is a [univalent function](../../../complex-analysis.md#univalent-function) with $F(0)=0$ and $F'(0)=1$, then

$$
\boxed{\{w:|w|<1/4\}\subseteq F(\mathbb D).}
$$

Equivalently, an arbitrary [univalent function](../../../complex-analysis.md#univalent-function) $f$ on the [unit disc](../../../topology.md#unit-disc) has $B(f(0),|f'(0)|/4)\subseteq f(\mathbb D)$. The constant cannot be increased: the [Koebe function](../../../complex-analysis.md#koebe-function) $F(w)=w/(1-w)^2$ omits the ray $(-\infty,-1/4]$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume the [domains](../../../topology.md#domain-mathematical-analysis) are proper, so $d$ and $\widetilde d$ are finite and positive, and interpret the [conformal transformation](../../../geometry-and-topology.md#conformal-map) as a bijection. Apply the [Koebe quarter theorem](../../../complex-analysis.md#koebe-quarter-theorem) to

$$
F(w)=\frac{f(z+dw)-f(z)}{d f'(z)},\qquad |w|<1.
$$

The [open ball](../../../topology.md#open-ball) $B(z,d)$ lies in $D$, so $F$ is a normalized [univalent function](../../../complex-analysis.md#univalent-function). Its image inclusion shows that $B(\widetilde z,d|f'(z)|/4)\subseteq\widetilde D$. Therefore $d|f'(z)|/4\leq\widetilde d$, or $|f'(z)|\leq4\widetilde d/d$.

Apply the same argument to the inverse [conformal map](../../../geometry-and-topology.md#conformal-map), whose [derivative](../../../calculus.md#derivative) at $\widetilde z$ is $1/f'(z)$. It gives $\widetilde d/(4|f'(z)|)\leq d$. Thus the [boundary-distance derivative bound for a conformal bijection](../../../complex-analysis.md#boundary-distance-derivative-bound-for-a-conformal-bijection) is

$$
\boxed{\frac{\widetilde d}{4d}\leq|f'(z)|\leq\frac{4\widetilde d}{d}.}
$$

The full [domains](../../../topology.md#domain-mathematical-analysis) need not be [simply connected domains](../../../complex-analysis.md#simply-connected-domain): only the two [interior](../../../topology.md#interior-topology) discs are used. If the whole plane is allowed as a [domain](../../../topology.md#domain-mathematical-analysis), a [conformal bijection](../../../complex-analysis.md#biholomorphism) onto another plane [domain](../../../topology.md#domain-mathematical-analysis) is affine and both [domains](../../../topology.md#domain-mathematical-analysis) are the whole plane. For example, $D=\widetilde D=\mathbb C$ and $f(z)=z$ make both [boundary](../../../topology.md#boundary-of-a-set) distances infinite and the printed ratios $\infty/\infty$ undefined. This is a necessary proper-domain convention. Bijectivity also matters: the injective [conformal map](../../../geometry-and-topology.md#conformal-map) $f(w)=w/8$ from the [unit disc](../../../topology.md#unit-disc) into itself has $d=\widetilde d=1$ at zero but $|f'(0)|=1/8<1/4$. Thus an interpretation allowing a map into, rather than onto, the second [domain](../../../topology.md#domain-mathematical-analysis) makes the lower bound false.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) $\partial_tg_t=2/(g_t-U_t)$ with $U_t=\sqrt\kappa B_t$. For a fixed $z\in\mathbb H$, let $T_z$ be its [Loewner swallowing time](../../../stochastic-process.md#interior-point-swallowing-time-for-a-loewner-chain), and write $Z_t=X_t+iY_t=g_t(z)-U_t$ and $J_t=|g_t'(z)|$ before that time. The [Loewner conformal radius](../../../geometry-and-topology.md#conformal-radius-under-a-chordal-loewner-flow) is $\Upsilon_t=Y_t/J_t$, half of the [conformal radius](../../../geometry-and-topology.md#conformal-radius) of $D_t=\mathbb H\setminus K_t$ at $z$. The [Koebe quarter theorem](../../../complex-analysis.md#koebe-quarter-theorem) bounds the [conformal radius](../../../geometry-and-topology.md#conformal-radius) above by four times the distance to the [boundary](../../../topology.md#boundary-of-a-set). For the reverse comparison, if $\phi:\mathbb D\to D_t$ maps zero to $z$, apply the [Schwarz lemma](../../../analysis.md#schwarz-lemma) to $\phi^{-1}(z+dw)$ on the [unit disc](../../../topology.md#unit-disc), where $d=\operatorname{dist}(z,\partial D_t)$; it gives $d\leq|\phi'(0)|$. Thus

$$
\frac12\operatorname{dist}(z,\partial D_t)\leq\Upsilon_t\leq2\operatorname{dist}(z,\partial D_t).
$$

We use the basic trace theorems that, for $\kappa>8$, the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) is continuous and [Transience of chordal SLE](../../../stochastic-process.md#transience-of-chordal-sle) gives $|\gamma(t)|\to\infty$. These facts make its image relatively closed in $\mathbb H$; they do not assume the space-filling conclusion. The [continuity](../../../calculus.md#continuous-function) and transience statements are available in [Rohde and Schramm's basic trace theorems](https://annals.math.princeton.edu/wp-content/uploads/annals-v161-n2-p07.pdf).

Take $\rho=\kappa-8>0$ in the supplied [SLE interior-point martingale](../../../stochastic-process.md#sle-interior-point-martingale). The [derivative](../../../calculus.md#derivative) exponent vanishes, leaving

$$
M_t=\Upsilon_t^{a}S_t^{-b},\qquad a=\frac{\kappa-8}{8}>0,\quad b=\frac{\kappa-8}{\kappa}>0,\quad S_t=\frac{Y_t}{|Z_t|}.
$$

A [nonnegative local martingale](../../../martingale.md#nonnegative-local-martingale) is a [supermartingale](../../../martingale.md#supermartingale). Applying the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) after localization at its first hit of a level $R$ gives the [maximal inequality for a nonnegative supermartingale](../../../martingale.md#maximal-inequality-for-a-nonnegative-supermartingale)

$$
\mathbb P\!\left(\sup_{t<T_z}M_t\geq R\right)\leq\frac{M_0}{R}.
$$

Thus $C=\sup_{t<T_z}M_t<\infty$ almost surely.

Suppose the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) avoids some [open ball](../../../topology.md#open-ball) $B(z,r)$ whose [closure](../../../topology.md#closure-topology) is inside $\mathbb H$. Before $T_z$, the whole [open ball](../../../topology.md#open-ball) is in $D_t$: a [connected](../../../geometry-and-topology.md#connected-space) [open ball](../../../topology.md#open-ball) disjoint from the trace cannot be partly in the unbounded [connected component](../../../geometry-and-topology.md#connected-component). Hence $\Upsilon_t\geq r/2$. The bound on $M$ forces $S_t\geq c>0$ throughout this interval, for a positive random constant $c$.

The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) and its [derivative](../../../calculus.md#derivative) yield

$$
\frac{d}{dt}Y_t^2=-4S_t^2,\qquad \frac{d}{dt}\log\Upsilon_t=-\frac{4Y_t^2}{|Z_t|^4},\qquad \frac{d\log\Upsilon_t}{d\log Y_t}=2S_t^2.
$$

The first identity forces $T_z<\infty$, since otherwise $Y_t^2\leq Y_0^2-4c^2t$ becomes negative. At a finite maximal lifetime, $Y_t\to0$; otherwise the continuous [Loewner driving function](../../../stochastic-process.md#loewner-driving-function) and the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) continue past that time. Integrating the last identity, using $S_t\geq c$, gives

$$
\Upsilon_t\leq\Upsilon_0\left(\frac{Y_t}{Y_0}\right)^{2c^2}\longrightarrow0,
$$

contradicting $\Upsilon_t\geq r/2$. Thus every fixed rational ball inside $\mathbb H$ is hit almost surely. A countable intersection makes the trace a [dense subset](../../../topology.md#dense-set) almost surely, and its relatively closed image, established by [continuity](../../../calculus.md#continuous-function) and transience, then contains all of $\mathbb H$:

$$
\boxed{\mathbb H\subseteq\gamma[0,\infty)\quad\text{almost surely for }\kappa>8.}
$$

This proves [space-filling SLE above parameter eight](../../../stochastic-process.md#space-filling-sle-above-parameter-eight). It rules out unvisited open regions, rather than inferring visits merely from membership in the filled [compact H-hulls](../../../stochastic-process.md#compact-h-hull). The choice $\rho=\kappa-8$ does not address the critical value eight.

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [chordal restriction property](../../../stochastic-process.md#chordal-restriction-property) concerns the unparameterized trace law. Let $A$ be a [compact H-hull](../../../stochastic-process.md#compact-h-hull) with $0\notin\overline A$, and put $\psi_A(z)=g_A(z)-g_A(0)$. This [conformal map](../../../geometry-and-topology.md#conformal-map) takes $\mathbb H\setminus A$ onto $\mathbb H$, fixes $0$ and infinity, and has [derivative](../../../calculus.md#derivative) one at infinity. On the event that the curve avoids $A$, its image is a curve from $0$ to infinity in $\mathbb H$. Restriction requires positive avoidance probability for every admissible $A$, and the conditional identity

$$
\boxed{\mathcal L\bigl(\psi_A(\gamma)\mid\gamma\cap A=\varnothing\bigr)=\mathcal L(\gamma),}
$$

up to increasing changes of the curve parameter. Equivalently, conditioning an [SLE](../../../stochastic-process.md#schramm-loewner-evolution) in a marked [simply connected domain](../../../complex-analysis.md#simply-connected-domain) to stay in an admissible [simply connected domain](../../../complex-analysis.md#simply-connected-domain) gives the same [SLE](../../../stochastic-process.md#schramm-loewner-evolution) law in that subdomain. The property does not assert that the original [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) survives an arbitrary [conformal map](../../../geometry-and-topology.md#conformal-map).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $\psi_A=g_A-g_A(0)$, and take another admissible [compact H-hull](../../../stochastic-process.md#compact-h-hull) $B$ in the image [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). Form the hull $C=A\cup\psi_A^{-1}(B)$, including its relative [closure](../../../topology.md#closure-topology) and filling bounded complementary components if needed. Its [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is

$$
g_C=g_B\circ\psi_A+g_A(0).
$$

Indeed, this composition maps the correct remaining [domain](../../../topology.md#domain-mathematical-analysis) onto $\mathbb H$, and its constant term at infinity is zero. Since $\psi_A(0)=0$, the [chain rule](../../../calculus.md#chain-rule) gives

$$
g_C'(0)=g_B'(0)g_A'(0).
$$

Both [derivatives](../../../calculus.md#derivative) are positive by local [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) and [boundary](../../../topology.md#boundary-of-a-set) orientation. Therefore the assumed avoidance formula gives

$$
\mathbb P(\psi_A(\gamma)\cap B=\varnothing\mid\gamma\cap A=\varnothing)=\frac{g_C'(0)^\alpha}{g_A'(0)^\alpha}=g_B'(0)^\alpha=\mathbb P(\gamma\cap B=\varnothing).
$$

The conditioning event has positive probability because $g_A'(0)>0$.

It remains to justify that these equalities determine the law. For a proper [simple curve](../../../topology.md#simple-curve) from $0$ to infinity, its complement has two sides, each [connected](../../../geometry-and-topology.md#connected-space) to an interval of the real [boundary](../../../topology.md#boundary-of-a-set). Any point off the curve lies in a thin polygonal tube attached to that [boundary](../../../topology.md#boundary-of-a-set) which avoids both the curve and zero; its [closure](../../../topology.md#closure-topology), with an end cap, is an admissible [compact H-hull](../../../stochastic-process.md#compact-h-hull). A countable collection of tubes with rational geometry therefore reconstructs the complement as the union of the tubes avoided by the curve.

The joint distribution of their avoidance indicators is also determined. Avoiding finitely many tubes is equivalent to avoiding the filled union when that union is admissible. If the union separates $0$ from infinity, avoidance is impossible and the joint probability is zero. Otherwise a [simple curve](../../../topology.md#simple-curve) cannot enter the bounded complementary pockets without crossing the union, so filling does not change the avoidance event. Finite joint avoidance probabilities consequently come from the same single-hull formulas; [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) supplies every finite indicator pattern. These patterns determine the random complement and hence the unparameterized simple trace.

Thus [avoidance probabilities determine a simple chordal curve law](../../../stochastic-process.md#avoidance-probabilities-determine-a-simple-chordal-curve-law), and the conditional image law above equals the original law. This proves the [derivative avoidance criterion for chordal restriction](../../../stochastic-process.md#derivative-avoidance-criterion-for-chordal-restriction), giving **the chordal restriction property**. Simplicity is essential to this reconstruction argument; it should not be replaced by a claim that arbitrary random closed sets are determined by these hull-avoidance tests.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [boundary](../../../topology.md#boundary-of-a-set) assertion is interpreted at positive finite times: a chordal [SLE](../../../stochastic-process.md#schramm-loewner-evolution) already starts on the [domain boundary](../../../topology.md#boundary-of-a-domain), and its marked target is another [boundary](../../../topology.md#boundary-of-a-set) point. The precise conclusion in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) is $\gamma(0,\infty)\subseteq\mathbb H$ almost surely.

For $0<\kappa\leq4$ and a fixed real $x>0$, the centered [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) $V_t=g_t(x)-U_t$ solves

$$
dV_t=\frac2{V_t}\,dt-\sqrt\kappa\,dB_t.
$$

Thus $R_t=V_t/\sqrt\kappa$ is a [Bessel process](../../../brownian-motion.md#bessel-process) driven by $-B$ of dimension

$$
\boxed{\delta=1+\frac4\kappa\geq2.}
$$

The [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process) says that, started positively, it never hits zero when $\delta\geq2$. For $x<0$, reflect the equation and apply the same result. Therefore every fixed nonzero [boundary](../../../topology.md#boundary-of-a-set) point has infinite swallowing time. A countable intersection gives this simultaneously for all nonzero rational [boundary](../../../topology.md#boundary-of-a-set) points.

To extend this countable conclusion to every real $x>0$, choose rational $q$ with $0<q<x$. The difference of two centered boundary solutions satisfies

$$
\frac{d}{dt}(V_t(x)-V_t(q))=-\frac{2(V_t(x)-V_t(q))}{V_t(x)V_t(q)},
$$

so it remains positive while both flows exist. On any finite time interval, $V_t(q)$ is bounded away from zero, hence so is $V_t(x)$. Moreover $V_t(x)=x-U_t+\int_0^t2/V_s(x)\,ds$ remains bounded there, so the differential equation continues for the whole interval. Its uniform separation from the [Loewner driving function](../../../stochastic-process.md#loewner-driving-function) also allows each flow map to continue as a [holomorphic function](../../../complex-analysis.md#holomorphic-function) on a complex [neighborhood](../../../topology.md#neighbourhood-mathematics) of $x$. Thus $x$ is outside $K_t$ and cannot be visited by the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain). Reflection gives the negative real axis. This uses countably many [Bessel processes](../../../brownian-motion.md#bessel-process) followed by deterministic flow comparison, rather than an uncountable union of probability-zero events.

To exclude a return to the starting point, use the [boundary extension of the inverse map for a continuous Loewner trace](../../../stochastic-process.md#boundary-extension-of-the-inverse-map-for-a-continuous-loewner-trace): $g_s^{-1}$ is continuous on the closed [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) and maps $U_s$ to $\gamma(s)$. This follows from the continuous trace theorem and the [Caratheodory boundary extension theorem](../../../complex-analysis.md#caratheodory-boundary-extension-theorem); it does not assume simplicity. At each deterministic rational time $s$, the [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) makes the mapped future a fresh [SLE](../../../stochastic-process.md#schramm-loewner-evolution), so its trace lies in $\mathbb H\cup\{0\}$ by the preceding argument. Mapping back with $g_s^{-1}$ therefore shows

$$
\gamma[s,\infty)\cap(K_s\cup\mathbb R)\subseteq\{\gamma(s)\}.
$$

If a point $q=\gamma(r)$ were revisited at $t>r$, choose rational $s\in(r,t)$ with $\gamma(s)\ne q$. Such an $s$ exists because [continuity](../../../calculus.md#continuous-function) and strictly increasing [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) forbid a constant trace on an interval. But $q\in K_s\cup\mathbb R$, contradicting the displayed inclusion. This excludes all self-contacts, including returns to zero, and proves the [simple curve](../../../topology.md#simple-curve) property needed when discussing later swallowing times.

For $\kappa=0$, the deterministic [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) is $\gamma(t)=2i\sqrt t$, so the conclusion follows directly. Hence the [boundary-intersection threshold for SLE](../../../stochastic-process.md#boundary-intersection-threshold-for-sle) gives

$$
\boxed{\gamma(t)\in\mathbb H\text{ for every }t>0\text{ almost surely, for }0\leq\kappa\leq4.}
$$

Mapping to another marked [simply connected domain](../../../complex-analysis.md#simply-connected-domain) carries positive-time points into its [interior](../../../topology.md#interior-topology). The literal statement including the starting point is false, since $\gamma(0)$ is prescribed to be on the [domain boundary](../../../topology.md#boundary-of-a-domain).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Before the [Loewner swallowing time](../../../stochastic-process.md#interior-point-swallowing-time-for-a-loewner-chain) $T_z$, put $Z_t=g_t(z)-U_t=X_t+iY_t$ and $\theta_t=\arg Z_t\in(0,\pi)$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applied to the [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) gives

$$
d\log Z_t=\frac{2-\kappa/2}{Z_t^2}\,dt-\frac{\sqrt\kappa}{Z_t}\,dB_t.
$$

Taking imaginary parts yields the [SLE angle process](../../../stochastic-process.md#sle-angle-process)

$$
d\theta_t=(\kappa-4)\frac{X_tY_t}{|Z_t|^4}\,dt+\sqrt\kappa\frac{Y_t}{|Z_t|^2}\,dB_t.
$$

For $\kappa=4$ the drift vanishes, so

$$
\boxed{\theta_t=\arg z+2\int_0^t\frac{Y_s}{|Z_s|^2}\,dB_s}
$$

is a continuous [local martingale](../../../martingale.md#local-martingale). Since $0<\theta_t<\pi$, every localized stopped version is a bounded true [martingale](../../../martingale.md). After resolving the lifetime issue below, the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) applied to [conditional expectations](../../../measure-theory.md#conditional-expectation) removes localization and gives a true bounded [martingale](../../../martingale.md).

For completeness, there is no finite lifetime ambiguity for a fixed [interior](../../../topology.md#interior-topology) $z$ in this parameter range. The preceding [Bessel process](../../../brownian-motion.md#bessel-process) and [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) argument gives a simple trace staying in the [interior](../../../topology.md#interior-topology), so no point is swallowed in a disconnected pocket. If $T_z$ were finite, the trace would have to reach $z$, forcing the [Loewner conformal radius](../../../geometry-and-topology.md#conformal-radius-under-a-chordal-loewner-flow) to tend to zero by the [Koebe quarter theorem](../../../complex-analysis.md#koebe-quarter-theorem). But

$$
\log\frac{\Upsilon_t}{\Upsilon_0}=-4\int_0^t\frac{Y_s^2}{|Z_s|^4}\,ds=-[\theta]_t.
$$

The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) says that a bounded continuous [local martingale](../../../martingale.md#local-martingale) cannot have infinite [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) before a finite terminal time: that would require a [Brownian motion](../../../brownian-motion.md) to stay in a bounded interval for all clock times. Therefore $\Upsilon_t$ cannot tend to zero at a finite $T_z$, a contradiction. Thus $T_z=\infty$ almost surely for each fixed $z$. This proves the [SLE4 angle martingale](../../../stochastic-process.md#sle4-angle-martingale) assertion: **the angle is a bounded continuous [martingale](../../../martingale.md)**. In particular $\mathbb E[\theta_t]=\arg z$. The upper-half-plane branch of the argument is used throughout.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
