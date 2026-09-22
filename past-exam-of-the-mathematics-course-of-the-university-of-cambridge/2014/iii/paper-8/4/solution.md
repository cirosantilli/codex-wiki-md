<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the standard setting of a [compact metrizable convex set](../../../../../compact-metrizable-convex-set.md) $K$ in a Hausdorff locally convex real topological vector space, with its metrizable topology. Write $A(K)$ for the continuous affine real [functions](../../../../../function-split.md) on $K$. The [affine upper envelope](../../../../../affine-upper-envelope.md) of a bounded real [function](../../../../../function-split.md) is

$$
\boxed{\overline f(x)=\inf\{a(x):a\in A(K),\ a\ge f\text{ on }K\}.}
$$

Constants make this infimum finite, and $f\le\overline f$. An infimum of affine continuous majorants is concave and [upper semicontinuous](../../../../../upper-semicontinuity.md), hence Borel. For continuous $f$ it is the upper concave envelope appropriate to barycentric [measures](../../../../../measure.md); it is not the pointwise maximum of $f$ and a selected [affine function](../../../../../affine-function.md).

For a fixed probability $\mu$, define $p(g)=\int_K\overline g\,d\mu$ on real $C(K)$. Affine majorants show

$$
\overline{g+h}\le\overline g+\overline h,\qquad
\overline{\lambda g}=\lambda\overline g\ (\lambda\ge0),\qquad
\overline{g+a}=\overline g+a\ (a\in A(K)).
$$

Thus $p$ is sublinear and $p(a)=\int a\,d\mu$ for affine $a$. On the span of $f$, the linear functional taking $f$ to $p(f)$ is dominated by $p$: the negative-scalar condition follows from $-p(f)\le p(-f)$. For $f=0$ start from the zero subspace. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) extends it to a linear functional $L$ on $C(K)$ with $L\le p$ and $L(f)=p(f)$.

If $g\ge0$, then $p(-g)\le0$, so $L(g)\ge0$. Also $p(1)=1$ and $p(-1)=-1$, forcing $L(1)=1$. Positivity gives $|L(g)|\le\|g\|_\infty$, and the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) produces a Borel probability $\nu$ with $L(g)=\int g\,d\nu$. Therefore

$$
\boxed{\int f\,d\nu=\int\overline f\,d\mu,\qquad
\int g\,d\nu\le\int\overline g\,d\mu\quad(g\in C(K)).}
$$

For affine $a$, testing both $a$ and $-a$ gives $\int a\,d\nu=\int a\,d\mu$: the two [measures](../../../../../measure.md) have the same [barycenter](../../../../../barycenter.md). This proves the requested [supporting measure lemma for affine upper envelopes](../../../../../supporting-measure-lemma-for-affine-upper-envelopes.md).

**Choquet's theorem:** every $x\in K$ has a [Borel probability measure](../../../../../borel-probability-measure.md) $\lambda$ concentrated on the [extreme points](../../../../../extreme-point.md) of $K$ whose [barycenter](../../../../../barycenter.md) is $x$; equivalently,

$$
\boxed{\lambda(\operatorname{Ex}K)=1,\qquad
a(x)=\int_K a\,d\lambda\quad(a\in A(K)).}
$$

Concentration is a [measure](../../../../../measure.md)-one assertion, not a claim that the topological support must be a closed subset of $\operatorname{Ex}K$.

To prove it, let $\mathcal M_x$ be the [measures](../../../../../measure.md) satisfying all the displayed affine equalities. It is nonempty because it contains $\delta_x$, and it is weakly closed in the compact space $P(K)$, hence compact. Let $h\in C(K)$ be strictly convex, as permitted. Choose $\lambda\in\mathcal M_x$ maximizing $\int h\,d\lambda$. Apply the supporting [measure](../../../../../measure.md) lemma with $\mu=\lambda$ and $f=h$. It gives $\nu$ with the same affine integrals, so $\nu\in\mathcal M_x$, and

$$
\int h\,d\lambda\ge\int h\,d\nu
=\int\overline h\,d\lambda\ge\int h\,d\lambda.
$$

Thus $\overline h-h\ge0$ has integral zero. If $z$ is not extreme, write $z=ty+(1-t)w$ with $0<t<1$ and distinct $y,w\in K$. Strict convexity and every affine majorant give

$$
h(z)<th(y)+(1-t)h(w)\le\overline h(z).
$$

Therefore the nonnegative gap is strictly positive at every nonextreme point. It is Borel, and $\operatorname{Ex}K$ is Borel by the allowed [G-delta set](../../../../../g-delta-set.md) assertion. Its zero integral forces $\lambda(K\setminus\operatorname{Ex}K)=0$, proving [Choquet's theorem by strict convexity](../../../../../choquet-s-theorem-by-strict-convexity.md). No uniqueness is asserted for the representing [measure](../../../../../measure.md).

For the real $L^\infty$ example, give its closed unit ball $K$ the [weak-star topology](../../../../../weak-star-topology.md) $\sigma(L^\infty,L^1)$, not the norm topology. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes it compact, and separability of $L^1[0,1]$ makes this ball metrizable. Its extreme points are exactly the classes $h$ satisfying $|h|=1$ almost everywhere. Indeed, if $|h|\le1-\varepsilon$ on a positive-[measure](../../../../../measure.md) set, adding and subtracting $\varepsilon$ times its indicator decomposes $h$ nontrivially inside the ball. Conversely, if $|h|=1$ almost everywhere and $h=(u+v)/2$ with $|u|,|v|\le1$, pointwise equality at the endpoints of $[-1,1]$ forces $u=v=h$ almost everywhere. This is the [extreme-point criterion for the L-infinity unit ball](../../../../../extreme-point-criterion-for-the-l-infinity-unit-ball.md).

For the hinted case $f=1_A-1_B$, put $C=[0,1]\setminus(A\cup B)$ and $h_\pm=1_A-1_B\pm1_C$. Then $h_\pm$ are extreme and

$$
\boxed{\nu=\tfrac12\delta_{h_+}+\tfrac12\delta_{h_-}}
$$

has [barycenter](../../../../../barycenter.md) $f$. If $C$ is null, the two point masses coincide.

For a general real $f$, choose a measurable representative in $[-1,1]$ and set, for $0\le t\le1$,

$$
H_t(s)=2\,1_{\{t\le(1+f(s))/2\}}-1,\qquad
\boxed{\nu=(t\mapsto H_t)_*\operatorname{Leb}_{[0,1]}.}
$$

Every $H_t$ is extreme. The map into the weak-star compact ball is Borel: for each $u\in L^1$, the [function](../../../../../function-split.md) $t\mapsto\int u(s)H_t(s)\,ds$ is measurable by joint measurability and integration; a countable dense family of such tests generates the ball's topology and Borel sigma-algebra. The [measure](../../../../../measure.md) is independent of changes to $f$ on a null set. For each $s$,

$$
\int_0^1 H_t(s)\,dt=2\frac{1+f(s)}2-1=f(s).
$$

The integrand paired with $u$ is dominated by $|u|$, so [Fubini's theorem](../../../../../fubini-s-theorem.md) yields

$$
\int_K\left(\int_0^1u(s)h(s)\,ds\right)d\nu(h)
=\int_0^1u(s)f(s)\,ds.
$$

These continuous linear tests define the weak-star [barycenter](../../../../../barycenter.md), hence that [barycenter](../../../../../barycenter.md) is $f$. Together with $\nu(\operatorname{Ex}K)=1$, this is the required [threshold Choquet representation in L-infinity](../../../../../threshold-choquet-representation-in-l-infinity.md).

If $L^\infty$ is instead taken over complex scalars, its extreme points satisfy the same unit-modulus condition. Write $f(s)=r(s)\zeta(s)$, with $r=|f|$ and $|\zeta|=1$, choosing $\zeta=1$ where $f=0$. Replace the threshold family by $\zeta(s)(2\,1_{\{t\le(1+r(s))/2\}}-1)$. Its members have unit modulus and its average is $f$, so the same pushforward and Fubini argument gives a representing [measure](../../../../../measure.md) in the real locally convex interpretation of the complex ball.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
