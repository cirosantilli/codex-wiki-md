# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_203.pdf)

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

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take the convention that the coordinates of [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) are independent standard real [Brownian motions](../../../brownian-motion.md), so its [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) is $\tfrac12\Delta$. Define the forward [conformal Brownian clock](../../../brownian-motion.md#conformal-brownian-clock)

$$
A(s)=\int_0^s|\phi'(B_r)|^2\,dr,\qquad
\widetilde T=A(T-),\qquad \tau=A^{-1}.
$$

Since a [conformal bijection](../../../complex-analysis.md#biholomorphism) has nonzero derivative, $A$ is a strictly increasing continuous map from $[0,T)$ onto $[0,\widetilde T)$. The time used inside the original path is its inverse:

$$
\boxed{\tau:[0,\widetilde T)\longrightarrow[0,T),\qquad
\widetilde B_t=\phi(B_{\tau(t)}).}
$$

Thus the interval direction for $\tau$ is the inverse-clock direction.

Write $\phi=u+iv$. The [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) and the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) make $u(B_s),v(B_s)$ continuous [local martingales](../../../martingale.md#local-martingale), with

$$
d[u(B)]_s=d[v(B)]_s=|\phi'(B_s)|^2ds,
\qquad d[u(B),v(B)]_s=0.
$$

Indeed both components are [harmonic functions](../../../partial-differential-equation.md#harmonic-function), and their gradients are orthogonal with the same squared norm. After the [time change of a continuous process](../../../stochastic-process.md#time-change-of-a-continuous-process) by $\tau$, their [quadratic variations](../../../stochastic-calculus.md#quadratic-variation) are $t$ and their [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) is zero. The [Lévy characterization of multidimensional Brownian motion](../../../brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion) therefore identifies $\widetilde B$ as [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $z'$, up to its lifetime.

It remains to identify that lifetime as the exit time, rather than merely produce a local Brownian path. Boundedness of $D$ gives $T<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). For every compact subset $C\subset D'$, its inverse image under $\phi$ is compactly contained in $D$. As $s\uparrow T$, continuity gives $B_s\to B_T\notin D$, so $\phi(B_s)$ eventually leaves $C$. Consequently the transformed path leaves every compact subset of $D'$ at its lifetime. If $\widetilde T<\infty$, its Brownian extension has a finite limit, and that limit is outside $D'$; if $\widetilde T=\infty$, the path never exits. In both cases its maximal lifetime is precisely the exit time from $D'$.

**The killed paths, together with their lifetimes, have the same law**:

$$
\boxed{\bigl(\widetilde T,(\widetilde B_t)_{t<\widetilde T}\bigr)
\overset{d}=\bigl(T',(B'_t)_{t<T'}\bigr).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A finite original exit time alone does not imply that the integral defining the [conformal Brownian clock](../../../brownian-motion.md#conformal-brownian-clock) is finite. To establish this, let $\psi=\phi^{-1}$. On the event $\{\widetilde T=\infty\}$, the Brownian path of part (a) lives forever in $D'$, while its inverse clock satisfies

$$
\tau(t)=\int_0^t|\psi'(\widetilde B_r)|^2\,dr<T.
$$

Choose a closed disc $C$ compactly contained in $D'$. Its radius may be decreased so that $|\psi'|^2\geq c>0$ on $C$. [Recurrence of planar Brownian motion](../../../brownian-motion.md#recurrence-of-planar-brownian-motion), together with the [Strong Markov property](../../../markov-process.md#strong-markov-property), gives infinite total [Brownian occupation time](../../../brownian-motion.md#brownian-occupation-time) in $C$: return repeatedly to a smaller concentric disc, and use the fixed positive probability of remaining in $C$ for a fixed positive duration. The successive trials imply infinitely many such durations. This is the same mechanism as the [divergence of a positive planar Brownian occupation integral](../../../brownian-motion.md#divergence-of-a-positive-planar-brownian-occupation-integral).

Hence, on any infinite-lifetime Brownian path,

$$
\int_0^\infty|\psi'(\widetilde B_r)|^2\,dr
\geq c\int_0^\infty\mathbf1_C(\widetilde B_r)\,dr=\infty.
$$

This contradicts $\tau(t)<T<\infty$. Thus $\widetilde T$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and equality in law from part (a) gives **[finite exit from a conformal image of a bounded planar domain](../../../brownian-motion.md#finite-exit-from-a-conformal-image-of-a-bounded-planar-domain)**:

$$
\boxed{\mathbb P_{z'}(T'<\infty)=1.}
$$

This asserts almost-sure finiteness, not finiteness of the expected exit time.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**No such [conformal bijection](../../../complex-analysis.md#biholomorphism) exists.** A prescribed point is a [polar point for planar Brownian motion](../../../brownian-motion.md#polar-point-for-planar-brownian-motion): a [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started away from zero hits zero with probability zero. For example, inside an annulus the probability of reaching radius $\varepsilon$ before radius $R$ is

$$
\frac{\log R-\log|z'|}{\log R-\log\varepsilon},
$$

by the [harmonic function](../../../partial-differential-equation.md#harmonic-function) $\log|w|$ and the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale). For fixed $R>|z'|$ this tends to zero as $\varepsilon\downarrow0$. Any finite-time visit to zero would occur before leaving some sufficiently large disc; the countable union over integer $R$ still has probability zero.

The exit time from $\mathbb C\setminus\{0\}$ is therefore infinite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), contradicting part (b) if this were the image of a bounded domain. Equivalently, a hypothetical inverse $\psi:\mathbb C\setminus\{0\}\to D$ would be bounded and holomorphic. The [Riemann removable singularity theorem](../../../isolated-singularity.md#riemann-removable-singularity-theorem) extends it over zero, and the [Liouville theorem](../../../complex-analysis.md#liouville-theorem) makes it constant, contradicting bijectivity.

$$
\boxed{D\text{ bounded}\quad\Longrightarrow\quad
D\text{ is not conformally equivalent to }\mathbb C\setminus\{0\}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use the [Green function of killed planar Brownian motion](../../../analysis.md#green-function-of-killed-planar-brownian-motion), normalized as the density of expected occupation with respect to area:

$$
\mathbb E_z\int_0^T f(B_t)\,dt
=\int_D G_D(z,w)f(w)\,dA(w)
$$

for nonnegative measurable $f$. Equivalently, $G_D(z,w)=\int_0^\infty p_D(t,z,w)\,dt$, where $p_D$ is the [killed Brownian transition density](../../../brownian-motion.md#killed-brownian-transition-density). With generator $\tfrac12\Delta$, the distributional normalization is $-\tfrac12\Delta_wG_D(z,w)=\delta_z(w)$, and the singularity is $-\pi^{-1}\log|w-z|$ plus a locally [harmonic function](../../../partial-differential-equation.md#harmonic-function). This fixes the normalization of the [Dirichlet Green function](../../../analysis.md#dirichlet-green-function) explicitly.

By [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) and its [conformal Brownian clock](../../../brownian-motion.md#conformal-brownian-clock),

$$
\mathbb E_{z'}\int_0^{T'} f(B'_s)\,ds
=\mathbb E_z\int_0^T f(\phi(B_t))|\phi'(B_t)|^2\,dt
=\int_D G_D(z,w)f(\phi(w))|\phi'(w)|^2\,dA(w).
$$

The [Jacobian determinant](../../../calculus.md#jacobian-determinant) of a [conformal map](../../../geometry-and-topology.md#conformal-map) is $|\phi'(w)|^2$. Changing the area variable to $w'=\phi(w)$ gives

$$
\int_{D'}G_D(z,\phi^{-1}(w'))f(w')\,dA(w').
$$

Uniqueness of the occupation density proves the desired equality almost everywhere. Both functions are continuous and [harmonic](../../../partial-differential-equation.md#harmonic-function) away from their pole, so it holds at every $w\ne z$. **The Green function is conformally invariant**:

$$
\boxed{G_{D'}(\phi(z),\phi(w))=G_D(z,w).}
$$

If the [Dirichlet Green function](../../../analysis.md#dirichlet-green-function) is instead normalized for $-\Delta$, both kernels are divided by two and the invariance statement is unchanged.

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the unique [conformal bijection](../../../complex-analysis.md#biholomorphism) from $H=\mathbb H\setminus K$ onto the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) with [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity):

$$
\boxed{g_K:H\to\mathbb H,\qquad
g_K(z)=z+\frac{a_K}{z}+O(|z|^{-2})\quad(z\to\infty).}
$$

The nonnegative coefficient $a_K$ is the [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) of $K$. The leading coefficient one and constant term zero remove the affine ambiguity of a half-plane map. In the [compact H-hull](../../../stochastic-process.md#compact-h-hull) convention, $K$ is bounded and relatively closed in $\mathbb H$, and its complement is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain); boundary attachment points can be included in its closure.

We will use these standard properties explicitly: $g_K$ and its inverse extend holomorphically by [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) across real intervals outside the hull's real attachment region; their real boundary restrictions are strictly increasing; and their normalized [Laurent series](../../../analysis.md#laurent-series) hold in a full reflected neighbourhood of infinity. In particular, when $K$ lies in the unit disc, these extensions exist across $(-\infty,-1)$ and $(1,\infty)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Set $g_K(iy)=u_y+iv_y$. The [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) gives

$$
u_y=O(y^{-2}),\qquad v_y=y-\frac{a_K}{y}+O(y^{-2}),
\qquad \frac{v_y}{y}\to1.
$$

The real interval under consideration lies outside the hull, so the reflected boundary map sends it monotonically to $(g_K(x),g_K(b))$. [Conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) transports its [harmonic measure](../../../brownian-motion.md#harmonic-measure) to the half-plane. By the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane),

$$
\mathbb P_{iy}(B_T\in(x,b))
=\frac1\pi\int_{g_K(x)}^{g_K(b)}
\frac{v_y}{(r-u_y)^2+v_y^2}\,dr.
$$

The endpoints are fixed and finite. On this interval,

$$
\frac{y v_y}{(r-u_y)^2+v_y^2}\longrightarrow1
$$

uniformly, using $v_y/y\to1$ and $u_y\to0$. Integrating gives **the interval-length limit**:

$$
\boxed{\lim_{y\to\infty}\pi y\,\mathbb P_{iy}(B_T\in(x,b))
=g_K(b)-g_K(x).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Compare the hull with the empty hull and the filled unit half-disc $J=\{z\in\mathbb H:|z|\leq1\}$. Their [mapping-out functions of compact H-hulls](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) are $g_\varnothing(z)=z$ and $g_J(z)=z+1/z$, the latter also giving the [half-plane capacity of a half-disc](../../../stochastic-process.md#half-plane-capacity-of-a-half-disc).

Use one [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $iy$, with $y>1$. For $x>1$, exiting $\mathbb H\setminus J$ through $(x,\infty)$ entails avoiding $K$, while exiting $\mathbb H\setminus K$ through this interval entails reaching it before exit from the whole half-plane. Thus the tail [harmonic measures](../../../brownian-motion.md#harmonic-measure) satisfy

$$
p_J(y,x)\leq p_K(y,x)\leq p_\varnothing(y,x).
$$

For any of these fixed hulls $L$, the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) gives the exact tail formula

$$
p_L(y,x)=\frac12-\frac1\pi
\arctan\!\frac{g_L(x)-\operatorname{Re}g_L(iy)}{\operatorname{Im}g_L(iy)}
=\frac12-\frac{g_L(x)}{\pi y}+o(y^{-1}).
$$

Subtract from $1/2$, multiply by $\pi y$, and take the limit. The inequalities reverse, yielding **the real boundary bounds**:

$$
\boxed{x\leq g_K(x)\leq x+\frac1x\qquad(x>1).}
$$

Applying this result to the reflected hull $-\overline K$ also gives

$$
x+\frac1x\leq g_K(x)\leq x\qquad(x<-1).
$$

The comparison is of Brownian exit events, so it does not assume that arbitrary conformal maps are pointwise ordered by domain inclusion.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write $g=g_K$ and $f=g^{-1}$. We use the [real boundary bounds for a unit-disc H-hull](../../../stochastic-process.md#real-boundary-bounds-for-a-unit-disc-h-hull) from part (c), including their reflected version. Set

$$
\alpha=\lim_{x\uparrow-1}g(x),\qquad
\beta=\lim_{x\downarrow1}g(x).
$$

Strict monotonicity and those bounds give $-2\leq\alpha\leq-1$ and $1\leq\beta\leq2$. The inverse $f$ extends across $\mathbb R\setminus[\alpha,\beta]$ and maps these intervals onto $(-\infty,-1)$ and $(1,\infty)$.

Consider the [holomorphic function](../../../complex-analysis.md#holomorphic-function) $F(w)=w-f(w)$ on $\mathbb H$. If $w$ approaches a real $u$ outside $[\alpha,\beta]$, its inverse tends to a real $x$ with $|x|>1$. Part (c) gives

$$
|u-f(u)|=|g(x)-x|\leq\frac1{|x|}\leq1.
$$

If $u\in[\alpha,\beta]$, every cluster point of $f(w)$ as $w\to u$ lies in the closed unit disc. To justify this without a boundary regularity assumption, first note that $f(w)$ cannot tend to infinity for bounded $w$, since $g(z)=z+O(1/z)$ there. An interior cluster point in $H$ would be mapped to the real number $u$, impossible for $g:H\to\mathbb H$. A real cluster point $x$ with $|x|>1$ would, by the reflected extension and strict monotonicity, have $g(x)$ outside $[\alpha,\beta]$, also impossible. All remaining finite boundary points lie in $K$ or in $[-1,1]$, hence in the unit disc.

It follows for every such $u$ that

$$
\limsup_{\substack{w\to u\\w\in\mathbb H}}|F(w)|
\leq |u|+1\leq3.
$$

Finally $f(w)=w+O(1/w)$ at infinity, so $F(w)\to0$ there. Apply the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) on large upper half-discs, using the boundary limsup just obtained, to conclude $|F(w)|\leq3$ everywhere in $\mathbb H$. Taking $w=g(z)$ proves **the [sharp displacement bound for a compact H-hull](../../../stochastic-process.md#sharp-displacement-bound-for-a-compact-h-hull), including irregular hulls**:

$$
\boxed{|g_K(z)-z|\leq3\qquad(z\in H).}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**A nearly closed semicircular slit makes the constant sharp.** Put

$$
m(z)=\frac{z+1}{1-z},\qquad
K_L=m^{-1}(\{iy:0<y\leq L\}),\qquad L>0.
$$

This is the unit-circle arc attached at $-1$ and ending just short of $1$. Its complement is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). There remains a narrow passage near $1$ connecting the interior bay to infinity. Thus $K_L$ is a [compact H-hull](../../../stochastic-process.md#compact-h-hull) inside the closed unit disc.

For an explicit check, let $S=\sqrt{1+L^2}$ and let $q_L(z)=\sqrt{m(z)^2+L^2}$ denote the [mapping-out function of a vertical slit](../../../stochastic-process.md#mapping-out-function-of-a-vertical-slit) applied to $m(z)$, with the branch asymptotic to its argument in the slit half-plane. Its normalized map is

$$
g_{K_L}(z)=1+\frac{L^2}{S^2}-\frac{2}{S\,[q_L(z)+S]}.
$$

The final [Möbius transformation](../../../group-theory.md#mobius-transformation) takes the image of the original infinity to infinity and gives [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity). For a fixed $z$ in the open unit half-disc, $\operatorname{Re}m(z)>0$, so $q_L(z)\sim L$ and $g_{K_L}(z)\to2$ as $L\to\infty$. Now take $z_\delta=-1+\delta+i\delta$, with $0<\delta<1$. First let $L\to\infty$, then let $\delta\downarrow0$. The [nearly closed semicircular slit](../../../stochastic-process.md#nearly-closed-semicircular-slit) gives

$$
\boxed{\lim_{\delta\downarrow0}\lim_{L\to\infty}
|g_{K_L}(z_\delta)-z_\delta|=3.}
$$

Every constant smaller than three therefore fails for some member of this family and some interior point. The bound need not be attained at an interior point of a single fixed hull.

<a id="2/e/image-a-nearly-closed-semicircular-slit-and-a-marked-point-inside-its-bay"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-203-nearly-closed-hull.png)

**[Figure 1](#2/e/image-a-nearly-closed-semicircular-slit-and-a-marked-point-inside-its-bay). A nearly closed semicircular slit and a marked point inside its bay**.

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization), let $W$ be standard real [Brownian motion](../../../brownian-motion.md) and put $\xi_t=\sqrt\kappa\,W_t$. Solve the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation)

$$
\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},\qquad g_0(z)=z.
$$

The points for which this flow ceases to exist form the growing [compact H-hulls](../../../stochastic-process.md#compact-h-hull) $K_t$, with [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) $2t$. The process is an [SLE](../../../stochastic-process.md#schramm-loewner-evolution) trace when its initial segments generate these hulls and

$$
\boxed{\gamma_t=\lim_{y\downarrow0}g_t^{-1}(\xi_t+iy),
\qquad \xi_t=\sqrt\kappa\,W_t.}
$$

The limit is the continuous [trace of a Loewner chain](../../../stochastic-process.md#trace-of-a-loewner-chain) started at zero. If the curve disconnects a region from infinity, that region is included in $K_t$; the hull is not generally just the visited curve. For $\kappa=0$ the driver is identically zero and the trace is the deterministic vertical slit $\gamma_t=2i\sqrt t$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the following deterministic boundary fact from the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation). For a continuous [trace of a Loewner chain](../../../stochastic-process.md#trace-of-a-loewner-chain) started at zero and generating its hulls, the real flow at $b>0$ has a [boundary swallowing time](../../../stochastic-process.md#boundary-point-swallowing-time-for-a-loewner-chain) $T_b$. Until that time it is the reflected boundary value of $g_t$, and

$$
X_t=g_t(b)-\xi_t>0.
$$

A finite $T_b$ is its first collision with the driver, $X_t\to0$ as $t\uparrow T_b$. Topologically, the boundary point $b$ is then visited or separated from infinity precisely when the trace has reached some point in $[b,\infty)$. A boundary crosscut can swallow an interval, so this is not a claim that the trace visits the particular point $b$.

Consequently the [SLE boundary swallowing criterion](../../../stochastic-process.md#sle-boundary-swallowing-criterion) is

$$
\boxed{\{\gamma\text{ hits }[b,\infty)\}=\{T_b<\infty\}.}
$$

For the [SLE](../../../stochastic-process.md#schramm-loewner-evolution) driver this real flow obeys

$$
dX_t=\frac2{X_t}\,dt-\sqrt\kappa\,dW_t,\qquad X_0=b,
$$

up to its first hit of zero. This is the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $\kappa>0$, divide the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) by $\sqrt\kappa$ and replace $W$ by $-W$. The resulting [Bessel process](../../../brownian-motion.md#bessel-process) has dimension

$$
\delta=1+\frac4\kappa,
$$

since its drift is $\tfrac{\delta-1}{2R_t}=2/(\kappa R_t)$. The [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process) suggests the threshold $\delta=2$, or $\kappa=4$. Here is a direct verification including accessibility in finite time.

The [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) of $X$ is $\mathcal L=\tfrac\kappa2\partial_x^2+(2/x)\partial_x$. An increasing [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) is

$$
s(x)=\begin{cases}
\dfrac{x^{1-4/\kappa}}{1-4/\kappa},&\kappa\ne4,\\
\log x,&\kappa=4.
\end{cases}
$$

It satisfies $\mathcal Ls=0$. For $0<\varepsilon<b<R$, the [boundary hitting probability from a diffusion scale function](../../../stochastic-calculus.md#boundary-hitting-probability-from-a-diffusion-scale-function), or [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) applied to $s(X)$, gives

$$
\mathbb P_b(T_\varepsilon<T_R)
=\frac{s(R)-s(b)}{s(R)-s(\varepsilon)}.
$$

For $0<\kappa<4$, $s(\varepsilon)\to-\infty$, so this probability tends to zero as $\varepsilon\downarrow0$. A finite zero hit has a bounded path before the hit and hence precedes $T_R$ for some integer $R$; taking a countable union proves that zero is never hit.

For $\kappa>4$, write $a=1-4/\kappa>0$. Taking the inner boundary to zero gives $1-(b/R)^a$. This limit really concerns a finite zero hit: the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
d(X_t^2)=(\kappa+4)dt-2\sqrt\kappa X_t\,dW_t.
$$

Stopped on $[\varepsilon,R]$, it implies

$$
\mathbb E_b(T_\varepsilon\wedge T_R)
\leq\frac{R^2-b^2}{\kappa+4},
$$

uniformly in $\varepsilon$. The increasing limit of these exit times is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence); the stopped squared process has a continuous extension, so its limiting lower endpoint is zero. Thus

$$
\mathbb P_b(T_0<T_R)=1-(b/R)^a.
$$

Let $R\to\infty$ to obtain $\mathbb P_b(T_0<\infty)=1$. When $\kappa=0$, the explicit solution is $X_t=\sqrt{b^2+4t}$, which stays positive.

Combining this with the [SLE boundary swallowing criterion](../../../stochastic-process.md#sle-boundary-swallowing-criterion) gives **the critical parameter and the two regimes**:

$$
\boxed{\kappa_c=4,\qquad
\mathbb P(\gamma\text{ hits }[b,\infty))=
\begin{cases}0,&0\leq\kappa<4,\\1,&\kappa>4.\end{cases}}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $\kappa<4$, each event $\{\gamma\text{ hits }[1/n,\infty)\}$ has probability zero by part (c). Every positive real point lies in one of these intervals. The countable union therefore has probability zero, proving **simultaneous avoidance of the entire positive real axis**:

$$
\boxed{\gamma([0,\infty))\cap(0,\infty)=\varnothing\quad\text{almost surely}.}
$$

For $\kappa>4$, every event $\{\gamma\text{ hits }[n,\infty)\}$ has probability one. Their countable intersection still has probability one. On that event the set of positive real points visited contains a point at least $n$ for every integer $n$, so **the visited positive boundary set is unbounded**:

$$
\boxed{\sup\bigl(\gamma([0,\infty))\cap(0,\infty)\bigr)=\infty
\quad\text{almost surely}.}
$$

This uses countably many [SLE boundary swallowing criteria](../../../stochastic-process.md#sle-boundary-swallowing-criterion); no intersection over an uncountable family of probability-one events is needed.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

At $\kappa=4$, the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) has dimension two. Its [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) is $s(x)=\log x$, giving

$$
\mathbb P_b(T_\varepsilon<T_R)
=\frac{\log(R/b)}{\log(R/\varepsilon)}\longrightarrow0
\qquad(\varepsilon\downarrow0).
$$

The same bounded-path and countable-union argument as in part (c) excludes a finite zero hit. Hence **the critical case belongs to the boundary-avoiding regime**:

$$
\boxed{\mathbb P(\gamma\text{ hits }[b,\infty))=0
\qquad(b>0,\ \kappa=4).}
$$

The countable argument of part (d) gives no visits to any positive real point [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). By [Reflection invariance of Brownian motion](../../../brownian-motion.md#reflection-invariance-of-brownian-motion), reflected [SLE](../../../stochastic-process.md#schramm-loewner-evolution) has the same law, so no negative real point is visited either. Thus the set of real points visited is exactly $\{0\}$. Recurrence of a two-dimensional [Bessel process](../../../brownian-motion.md#bessel-process) near zero does not mean that it hits zero.

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [conformal automorphism of the upper half-plane](../../../complex-analysis.md#conformal-automorphism-of-the-upper-half-plane) is a real [Möbius transformation](../../../group-theory.md#mobius-transformation)

$$
\phi(z)=\frac{az+b}{cz+d},\qquad a,b,c,d\in\mathbb R,
\quad ad-bc>0,
$$

with coefficients determined up to a common nonzero factor. The boundary interval $(\infty,1)$ is the oriented real boundary arc from infinity to $1$, namely the finite real interval $(-\infty,1)$. The map must take the left endpoint $-1$ to infinity and the right endpoint infinity to $1$, while fixing zero. These three boundary values determine the [Möbius transformation](../../../group-theory.md#mobius-transformation) uniquely:

$$
\boxed{\phi(z)=\frac{z}{1+z}.}
$$

Its determinant is positive, $\operatorname{Im}\phi(z)=\operatorname{Im}z/|1+z|^2>0$, and on $(-1,\infty)$ its derivative is $(1+x)^{-2}>0$. Its endpoint limits are $-\infty$ at $-1+$ and $1$ at $+\infty$, so it has exactly the required boundary extension.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The scale is precisely the inverse [conformal map](../../../geometry-and-topology.md#conformal-map):

$$
\sigma(w)=\frac{w}{1-w}=\phi^{-1}(w),\qquad
\sigma(0)=0,\quad\sigma(1)=\infty.
$$

By definition, a [chordal SLE in a specified scale](../../../stochastic-process.md#chordal-sle-in-a-specified-scale) in $(\mathbb H,0,1)$ is a curve whose image under $\sigma$ is the half-plane-capacity-parameterized [SLE](../../../stochastic-process.md#schramm-loewner-evolution) from zero to infinity. Here

$$
\boxed{\sigma(\widetilde\gamma_t)
=\sigma(\phi(\gamma_t))=\gamma_t,}
$$

and the right-hand side is the given $\operatorname{SLE}_6$. Equivalently, this is [Conformal invariance of SLE](../../../stochastic-process.md#conformal-invariance-of-sle), with the target point transported from infinity to $1$. Thus **$\widetilde\gamma$ is $\operatorname{SLE}_6$ in $(\mathbb H,0,1)$ in scale $\sigma$**, using the original parameter $t$. This scaled parameter is distinguished from the ordinary [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) of its image hulls used next.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $\widetilde\xi_t=\phi_t(\xi_t)$ and $p_t=\phi_t'(\xi_t)$. The given [conformal change of half-plane capacity](../../../stochastic-process.md#conformal-change-of-half-plane-capacity) makes the image mapping-out equation

$$
\partial_t\widetilde g_t(w)
=\frac{2p_t^2}{\widetilde g_t(w)-\widetilde\xi_t}.
$$

Indeed its capacity speed is $2p_t^2$, and the stated [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) identifies the indicated single driver. For $t<T$, differentiate the conjugacy identity

$$
\widetilde g_t\circ\phi=\phi_t\circ g_t
$$

at a fixed original point. The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) then gives the **[conformal conjugacy derivative for the chordal Loewner equation](../../../stochastic-process.md#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)**

$$
\boxed{\dot\phi_t(z)
=\frac{2\phi_t'(\xi_t)^2}{\phi_t(z)-\phi_t(\xi_t)}
-\frac{2\phi_t'(z)}{z-\xi_t}.}
$$

The change of variable $z=g_t(w)$ covers the whole upper half-plane. The [conformal automorphism of the upper half-plane](../../../complex-analysis.md#conformal-automorphism-of-the-upper-half-plane) $\phi_t$ is a real [Möbius transformation](../../../group-theory.md#mobius-transformation). Its pole is the image of the still-unswallowed boundary point $-1$, so it is holomorphic in a neighbourhood of $\xi_t$ before $T$.

To evaluate the apparent singularity, write $h=z-\xi_t$, $p=\phi_t'(\xi_t)>0$ and $q=\phi_t''(\xi_t)$. The [Taylor series](../../../calculus.md#taylor-series) is

$$
\phi_t(\xi_t+h)-\phi_t(\xi_t)=ph+\tfrac12qh^2+O(h^3),
\qquad\phi_t'(\xi_t+h)=p+qh+O(h^2).
$$

Thus the first term in the derivative is $2p/h-q+O(h)$, while the second is $2p/h+2q+O(h)$. Their poles cancel and their constant terms differ by $-3q$. Therefore

$$
\boxed{\dot\phi_t(\xi_t)=-3\phi_t''(\xi_t).}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For the [SLE](../../../stochastic-process.md#schramm-loewner-evolution) driver $d\xi_t=\sqrt6\,dW_t$, apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\widetilde\xi_t=\phi_t(\xi_t)$. At a fixed spatial point, $\phi_t$ has [finite variation](../../../real-analysis.md#total-variation-of-a-function) locally in time by the derivative formula in part (c); there is no extra spatial martingale term. Consequently

$$
d\widetilde\xi_t
=\left(\dot\phi_t(\xi_t)+3\phi_t''(\xi_t)\right)dt
+\sqrt6\,\phi_t'(\xi_t)\,dW_t
=\sqrt6\,p_t\,dW_t.
$$

This exact cancellation is the [target-change locality of SLE6](../../../stochastic-process.md#target-change-locality-of-sle6). For a general parameter the [transformed SLE driving function](../../../stochastic-process.md#transformed-sle-driving-function) would have drift $(\kappa/2-3)\phi_t''(\xi_t)$.

Define the increasing clock and its inverse by

$$
a(t)=\int_0^tp_r^2\,dr=\frac12\operatorname{hcap}(\widetilde K_t),
\qquad t(s)=a^{-1}(s).
$$

The derivative $p_t$ is real and strictly positive before $T$, so this is a valid continuous [time change of a continuous process](../../../stochastic-process.md#time-change-of-a-continuous-process). The driver is a continuous [local martingale](../../../martingale.md#local-martingale) with [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $[\widetilde\xi]_t=6a(t)$ and initial value zero. The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) gives a standard [Brownian motion](../../../brownian-motion.md) $\widehat W$ such that

$$
\widetilde\xi_{t(s)}=\sqrt6\,\widehat W_s,
\qquad 0\leq s<a(T-).
$$

If the terminal clock is finite, the Brownian motion may be extended beyond that stopping time; only its stopped part is used here. Reparameterizing the image maps gives

$$
\partial_s\widetilde g_{t(s)}(z)
=\frac2{\widetilde g_{t(s)}(z)-\sqrt6\,\widehat W_s},
\qquad\operatorname{hcap}(\widetilde K_{t(s)})=2s.
$$

These are exactly the defining [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) and [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) for $\operatorname{SLE}_6$. The trace is $\widetilde\gamma_{t(s)}$. Hence **the image curve is also ordinary chordal $\operatorname{SLE}_6$ after this time change, up to the specified stopping time**:

$$
\boxed{\bigl(\widetilde\gamma_{t(s)}\bigr)_{0\leq s<a(T-)}
\text{ is stopped }\operatorname{SLE}_6\text{ in }(\mathbb H,0,\infty).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
