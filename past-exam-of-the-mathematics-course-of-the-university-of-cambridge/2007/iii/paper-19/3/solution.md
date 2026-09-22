<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the metric on $M$ induced by its given Euclidean embedding. For two smooth maps define the [C1 metric on a smooth mapping space](../../../../../c1-metric-on-a-smooth-mapping-space.md) by

$$
d_1(f,g)=\sup_{x\in M}|f(x)-g(x)|+
\sup_{x\in M}\|Df_x-Dg_x\|_{\mathrm{op}},
$$

where the [differential](../../../../../differential-of-a-smooth-map.md) has domain $T_xM$ with the induced [inner product](../../../../../inner-product.md). Compactness makes both suprema finite. The norm properties give symmetry and the [triangle inequality](../../../../../triangle-inequality.md), and the first term makes distance zero imply equality of maps. Thus convergence in $d_1$ is [uniform convergence](../../../../../uniform-convergence.md) of both maps and [differentials](../../../../../differential-of-a-smooth-map.md).

Because $i$ is an [immersion](../../../../../immersion.md), $Di_x$ is injective at every point. The continuous function $|Di_xv|$ on the compact [unit tangent bundle](../../../../../unit-tangent-bundle.md) has a positive minimum $a$. Therefore

$$
|Di_xv|\ge a|v|\qquad(x\in M,\ v\in T_xM).
$$

For all sufficiently large $n$, $\sup_x\|Df_{n,x}-Di_x\|<a/2$, and then

$$
|Df_{n,x}v|\ge |Di_xv|-|(Df_{n,x}-Di_x)v|\ge\frac a2|v|.
$$

Consequently **every sufficiently late $f_n$ is an [immersion](../../../../../immersion.md)**. If $M$ has dimension zero it is a finite set, the [immersion](../../../../../immersion.md) assertion is automatic, and eventual injectivity follows directly from separation of its finitely many image points; we henceforth treat positive dimension.

For injectivity, choose finitely many coordinate maps $\phi_b$ on convex balls, with smaller coordinate neighborhoods covering $M$ and closures lying inside the larger balls. Write $I_b=i\circ\phi_b$ and $F_{n,b}=f_n\circ\phi_b$. On the finitely many relevant compact coordinate closures, the [differentials](../../../../../differential-of-a-smooth-map.md) of the $I_b$ have a common positive lower bound $s$, and convergence in $d_1$ gives

$$
|DF_{n,b}(u)v|\ge\frac s2|v|
$$

for all late $n$. The assumed uniform second-derivative bound gives a common bound $L$ for $D^2F_{n,b}$ on those larger coordinate neighborhoods. If the bound is expressed using an intrinsic [Hessian](../../../../../hessian-matrix.md), the coordinate chain rule also involves first derivatives and derivatives of the fixed charts; their bounds are uniform by C1 convergence and compactness. Thus $L$ can be larger than the printed constant $C$, but is independent of $n$.

For $u,v$ whose segment lies in one such coordinate ball, [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md) gives

$$
F_{n,b}(v)-F_{n,b}(u)=DF_{n,b}(u)(v-u)+R,
\qquad |R|\le\frac L2|v-u|^2.
$$

Choose $\delta>0$ with $L\delta\le s/2$. Then, whenever $0<|u-v|<\delta$,

$$
|F_{n,b}(v)-F_{n,b}(u)|\ge\frac s2|u-v|-\frac L2|u-v|^2
\ge\frac s4|u-v|>0.
$$

The [Lebesgue number lemma](../../../../../lebesgue-number-lemma.md) applied to the finite smaller-chart cover, together with [uniform continuity](../../../../../uniform-continuity.md) of its coordinate inverses on the relevant compact sets, gives $\rho>0$ such that every pair $x,y\in M$ with $0<|x-y|<\rho$ lies in one such chart with coordinate distance below $\delta$. The displayed estimate therefore excludes all sufficiently close pairs of equal images, uniformly in late $n$.

The remaining pairs form the compact set

$$
K_\rho=\{(x,y)\in M\times M:|x-y|\ge\rho\}.
$$

If it is nonempty, injectivity of the [smooth embedding](../../../../../smooth-embedding.md) $i$ gives a positive minimum $b$ of $|i(x)-i(y)|$ on it. [Uniform convergence](../../../../../uniform-convergence.md) makes $\sup_x|f_n(x)-i(x)|<b/3$ for all sufficiently large $n$, and hence on $K_\rho$,

$$
|f_n(x)-f_n(y)|\ge |i(x)-i(y)|-2\sup_z|f_n(z)-i(z)|>b/3.
$$

If $K_\rho$ is empty there is nothing left to check. Combining the near-pair and distant-pair bounds makes $f_n$ injective for every sufficiently late $n$. It is already an [immersion](../../../../../immersion.md), and a continuous injection from compact $M$ into a [Hausdorff space](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md) onto its image. By [compact injective immersion is an embedding](../../../../../compact-injective-immersion-is-an-embedding.md),

$$
\boxed{f_n:M\hookrightarrow\mathbb R^N\text{ is a smooth embedding for all sufficiently large }n.}
$$

This proves the requested [stability of compact smooth embeddings](../../../../../stability-of-compact-smooth-embeddings.md) using the stated second-derivative assumption. That assumption supplies a convenient Taylor constant; the stronger C1 openness result can replace it by the [uniform continuity](../../../../../uniform-continuity.md) of the limiting [differential](../../../../../differential-of-a-smooth-map.md) on finitely many small coordinate balls.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
