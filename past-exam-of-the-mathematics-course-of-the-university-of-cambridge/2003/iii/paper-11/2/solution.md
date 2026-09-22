<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

There is an essential qualification to the printed hypothesis. If [compactly generated group](../../../../../compactly-generated-group.md) means merely generated algebraically by a [compact subset](../../../../../compact-space.md), the claim is false. In the additive group $\mathbb Q$ with its usual [topology](../../../../../topology-split.md),

$$
K=\{0\}\cup\{1/n!:n\ge1\}
$$

is compact, being a convergent sequence together with its limit, and generates every rational number since any integer denominator divides some factorial. The group is metrizable. However, an invariant [Radon measure](../../../../../radon-measure.md) has a common mass $c$ on each singleton. If $c>0$, the [compact set](../../../../../compact-space.md) $K$ has infinite measure, contradicting finiteness on [compact sets](../../../../../compact-space.md). If $c=0$, countable additivity makes the entire countable group have measure zero. Thus it has no nonzero [Haar measure](../../../../../haar-measure.md). This proves that [compact generation does not imply local compactness](../../../../../compact-generation-does-not-imply-local-compactness.md) and disproves the literal unrestricted statement.

The intended existence statement is valid when local [compactness](../../../../../compact-space.md) is included, either explicitly or in the convention that the group has a compact generating [neighbourhood](../../../../../neighbourhood-mathematics.md). Here is a construction for a locally compact, compactly generated, metrizable Hausdorff group. No invariant measure is assumed during its construction.

Enlarge a compact generating set to a symmetric compact [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) $S$. Then $G=\bigcup_nS^n$, and each $S^n$ is compact. Moreover $S^n$ lies in the interior of $S^{n+1}$, since multiplication by the open [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) contained in $S$ supplies an open [neighbourhood](../../../../../neighbourhood-mathematics.md) of every point of $S^n$. This gives a compact exhaustion. Every compact [metric](../../../../../metric.md) space has a countable [dense subset](../../../../../dense-set.md): take finite $1/k$-nets and unite them. Their union over this exhaustion is dense in $G$, so the [metric](../../../../../metric.md) space is separable and has a countable open basis.

We use nonnegative [compactly supported](../../../../../compact-support.md) [continuous functions](../../../../../continuous-function.md) and cutoffs equal to one on specified [compact sets](../../../../../compact-space.md). Their existence is covered by the source's permission concerning auxiliary functions. Fix a nonzero such function $h$. For nonzero $u\ge0$ define the weighted covering quantity

$$
(f:u)=\inf\left\{\sum_{j=1}^m c_j:f\le\sum_{j=1}^m c_jT_{x_j}u,\ c_j\ge0\right\},\qquad
T_xu(y)=u(x^{-1}y),\qquad I_u(f)=\frac{(f:u)}{(h:u)}.
$$

The quantities are finite: an [open set](../../../../../open-set.md) where $u$ is bounded below has translates covering the [compact support](../../../../../compact-support.md) of $f$, so finitely many sufficiently large weighted translates dominate it. The denominator is positive, since evaluation at a point where $h>0$ gives $(h:u)\ge h(y)/\|u\|_\infty>0$.

Each $I_u$ is nonnegative, homogeneous, monotone, left invariant and subadditive; these follow respectively by rescaling, comparing or combining covers, and translating their centers. Also $I_u(h)=1$. Composing a cover of $f$ by translates of $h$ with a cover of $h$ by translates of $u$ gives

$$
(f:u)\le(f:h)(h:u),\qquad 0\le I_u(f)\le(f:h).
$$

This is a bound independent of $u$. On functions supported in a fixed [compact set](../../../../../compact-space.md) $C$, choose a cutoff $k\ge1$ on $C$. Monotonicity and subadditivity imply

$$
|I_u(f)-I_u(g)|\le\|f-g\|_\infty I_u(k)\le\|f-g\|_\infty(k:h).
$$

Thus the covering functionals are uniformly Lipschitz on each fixed support.

Choose a nonzero $u_n\ge0$ with support in an [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) shrinking to $e$. The nonnegative functions supported in each compact member of the exhaustion form a separable [metric](../../../../../metric.md) cone in the [supremum norm](../../../../../supremum-norm.md), as a subspace of [continuous functions](../../../../../continuous-function.md) on that compact [metric](../../../../../metric.md) space. Select a countable dense family from each cone and include $h$. The uniform scalar bounds permit a diagonal subsequence along which $I_{u_n}$ converges on their countable union. The displayed Lipschitz estimate extends convergence to every nonnegative member of $C_c(G)$. Denote the limit by $I$. It inherits positivity, homogeneity, monotonicity, subadditivity, invariance and $I(h)=1$.

The crucial remaining step is additivity. Fix $f_1,f_2\ge0$ with combined support $C$, and fix a compact [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) $V_0$. Choose a cutoff $k$ equal to one on $CV_0^{-1}V_0$. For $\delta>0$, put

$$
F=f_1+f_2+\delta k,\qquad r_i=f_i/F,
$$

setting the ratio to zero off the denominator's nonzero set. These ratios are continuous: $k=1$ on a [neighbourhood](../../../../../neighbourhood-mathematics.md) of the supports, and off those supports the numerator vanishes. Their sum is at most one. [Compactness](../../../../../compact-space.md) and continuity give, for each $\eta>0$, an [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) $V$ small enough that each $r_i$ oscillates by at most $\eta$ on any translate of $V$ meeting $C$. To justify this uniform choice, such translates lie inside the fixed [compact set](../../../../../compact-space.md) $CV_0^{-1}V_0$ when $V\subset V_0$; continuity of $(y,v)\mapsto r_i(yv)$ and a finite cover of that [compact set](../../../../../compact-space.md) give a single small right-increment [neighbourhood](../../../../../neighbourhood-mathematics.md), then choose $V^{-1}V$ inside it.

If $u$ has support in $V$ and $F\le\sum_j c_jT_{x_j}u$, discard translates not meeting $C$ when covering $f_i$. Let $a_{ij}$ be the supremum of $r_i$ on the remaining translate's support. Then $f_i\le\sum_j a_{ij}c_jT_{x_j}u$, and comparing both suprema with the ratios at one common point gives $a_{1j}+a_{2j}\le1+2\eta$. Taking covering infima yields

$$
I_u(f_1)+I_u(f_2)\le(1+2\eta)I_u(F)
\le(1+2\eta)[I_u(f_1+f_2)+\delta I_u(k)].
$$

Along the subsequence this holds eventually, since its supports shrink. Pass to $I$, then let $\eta\downarrow0$ and $\delta\downarrow0$; the uniform bound on $I_u(k)$ gives $I(f_1)+I(f_2)\le I(f_1+f_2)$. Subadditivity gives the reverse inequality. Thus $I$ is additive.

Extend $I$ linearly to real functions using positive and negative parts, and then complex-linearly to $C_c(G)$. The compact-support bounds above make it a positive, locally bounded functional. The [Riesz representation on compactly supported continuous functions](../../../../../riesz-representation-on-compactly-supported-continuous-functions.md) gives a [Radon measure](../../../../../radon-measure.md) $\mu$ with $I(f)=\int f\,d\mu$. Translation invariance of $I$ and uniqueness in that representation give $\mu(xE)=\mu(E)$ for Borel $E$. It is nonzero because $I(h)=1$, and finite on [compact sets](../../../../../compact-space.md) because a cutoff dominating their indicators has finite integral. Finally every nonempty [open set](../../../../../open-set.md) has positive measure: otherwise its translates cover the [compact support](../../../../../compact-support.md) of $h$, a finite subcover would give that support measure zero, contradicting $I(h)=1$. Hence **$\mu$ is a [Haar measure](../../../../../haar-measure.md) under the stated local-compactness qualification**. This is [Haar measure from normalized covering functionals](../../../../../haar-measure-from-normalized-covering-functionals.md), with the limiting additivity proved explicitly.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
