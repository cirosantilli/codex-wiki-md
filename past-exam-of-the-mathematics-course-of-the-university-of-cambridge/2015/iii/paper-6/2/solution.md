<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [weak topology](../../../../../weak-topology-split.md) on a [normed vector space](../../../../../normed-vector-space.md) $X$ is $\sigma(X,X^*)$, the coarsest [topology](../../../../../topology-split.md) making every [bounded linear functional](../../../../../continuous-linear-functional.md) continuous. A neighbourhood base at $x$ is given by finitely many inequalities $|f_j(y-x)|<\varepsilon$, with $f_j\in X^*$. In the complex case, separation uses [real parts](../../../../../real-part.md) of [bounded linear functionals](../../../../../continuous-linear-functional.md).

[Mazur theorem](../../../../../mazur-theorem.md) states that the [weak closure](../../../../../weak-closure.md) of a [convex set](../../../../../convex-set.md) equals its closure in the [norm topology](../../../../../norm-topology.md). The [weak topology](../../../../../weak-topology-split.md) is coarser than the [norm topology](../../../../../norm-topology.md), so the norm closure is contained in the [weak closure](../../../../../weak-closure.md). Conversely, if $x$ is outside the norm closure of a [convex set](../../../../../convex-set.md) $C$, the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) gives $f\in X^*$ and $a\in\mathbb R$ with $\operatorname{Re}f(x)>a\geq\sup_{c\in C}\operatorname{Re}f(c)$. The corresponding [weak topology](../../../../../weak-topology-split.md) neighbourhood of $x$ misses $C$, so $x$ is outside its [weak closure](../../../../../weak-closure.md). This proves [Mazur theorem](../../../../../mazur-theorem.md), including the empty-set case. In particular, if $x_n$ converges weakly to $x$, then $x$ is in the [weak closure](../../../../../weak-closure.md) of every tail and therefore in the norm closure of its [convex hull](../../../../../convex-hull.md). Choosing a finite [convex combination](../../../../../convex-combination.md) of the $n$th tail within $1/n$ of $x$ proves the usual [Mazur lemma](../../../../../mazur-s-lemma.md) formulation as well.

The [weak-star topology](../../../../../weak-star-topology.md) on the [continuous dual space](../../../../../continuous-dual-space-split.md) $X^*$ is $\sigma(X^*,X)$: convergence means pointwise convergence on $X$, and a neighbourhood base prescribes finitely many evaluation inequalities. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) states that the [closed unit ball](../../../../../closed-unit-ball.md) of $X^*$ is compact in this [weak-star topology](../../../../../weak-star-topology.md), even if $X$ is incomplete. Embed this [closed unit ball](../../../../../closed-unit-ball.md) into

$$
P=\prod_{x\in X}\{z\in\mathbb K:|z|\leq\|x\|\},\qquad f\longmapsto(f(x))_{x\in X},
$$

where $\mathbb K=\mathbb R$ or $\mathbb C$. Each factor is compact, so $P$ is compact by the [Tychonoff theorem](../../../../../tychonoff-s-theorem.md). Inside $P$, the equations $a_{x+y}=a_x+a_y$ and $a_{\lambda x}=\lambda a_x$ define a [closed set](../../../../../closed-set.md). Every such point defines a [linear functional](../../../../../linear-functional.md) satisfying $|a_x|\leq\|x\|$, hence belongs to the [closed unit ball](../../../../../closed-unit-ball.md) of $X^*$. Thus this image is closed in $P$. The [product topology](../../../../../product-topology.md) on it is exactly the [weak-star topology](../../../../../weak-star-topology.md), proving [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). Evaluations also separate its points, so the [weak-star topology](../../../../../weak-star-topology.md) is Hausdorff.

For the [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md) $J_X:X\to X^{**}$, we have $(J_Xx)(f)=f(x)$. Restricting all evaluations at $f\in X^*$ therefore gives exactly $\sigma(X,X^*)$. Thus **the induced [subspace topology](../../../../../subspace-topology.md) is the [weak topology](../../../../../weak-topology-split.md) on $X$**.

Now identify $X$ with $J_XX$. Let $C$ be a bounded [convex set](../../../../../convex-set.md), write $D$ for its norm closure in $X$, and let $K$ be its [weak-star topology](../../../../../weak-star-topology.md) closure in $X^{**}$. Boundedness places $K$ in a multiple of the [closed unit ball](../../../../../closed-unit-ball.md) of $X^{**}$, so $K$ is compact by [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). The preceding [subspace topology](../../../../../subspace-topology.md) identification and [Mazur theorem](../../../../../mazur-theorem.md) give

$$
K\cap X=\overline C^{\,w}=D.
$$

If $D$ is a [weakly compact set](../../../../../weakly-compact-set.md), its image in the Hausdorff [weak-star topology](../../../../../weak-star-topology.md) is compact and therefore closed. It contains $C$, so $K\subseteq D\subseteq X$. Conversely, if $K\subseteq X$, the displayed identity gives $K=D$, and its compactness is precisely weak compactness in $X$. Hence **$\boxed{D\text{ is weakly compact}\iff K\subseteq X}$**. This argument also covers $C=\varnothing$.

For a [bounded linear operator](../../../../../continuous-linear-operator.md) $T:X\to Y$, its [Banach-space adjoint](../../../../../transpose-of-a-bounded-linear-operator.md) is $T^*:Y^*\to X^*$, defined by $(T^*y^*)(x)=y^*(Tx)$. Evaluation at any fixed $x$ is thus evaluation at $Tx$ after applying $T^*$. Each is continuous in the relevant [weak-star topology](../../../../../weak-star-topology.md), proving that **$T^*$ is weak-star continuous**. Applying the same result to $T^*$ shows that $T^{**}:X^{**}\to Y^{**}$ is weak-star continuous. Direct evaluation gives

$$
T^{**}J_X=J_YT.
$$

Use $B_X$ for the [closed unit ball](../../../../../closed-unit-ball.md); using the open ball gives the same norm closure of $T(B_X)$. [Goldstine theorem](../../../../../goldstine-theorem.md) says that $J_XB_X$ is weak-star dense in $B_{X^{**}}$. Put $K=T^{**}(B_{X^{**}})$. It is compact and closed in the [weak-star topology](../../../../../weak-star-topology.md) by [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) and the established continuity. It contains $J_YT(B_X)$. Conversely, [Goldstine theorem](../../../../../goldstine-theorem.md) gives, for every $x^{**}\in B_{X^{**}}$, a [net](../../../../../net-mathematics.md) $(J_Xx_\alpha)$ from $J_XB_X$ converging weak-star to $x^{**}$; its image converges weak-star to $T^{**}x^{**}$. Consequently

$$
\overline{J_YT(B_X)}^{\,w^*}=T^{**}(B_{X^{**}}).
$$

Apply the preceding bounded [convex set](../../../../../convex-set.md) criterion in $Y$, and then scale the [closed unit ball](../../../../../closed-unit-ball.md). We obtain the [bidual characterization of weakly compact operators](../../../../../bidual-characterization-of-weakly-compact-operators.md):

$$
\boxed{\overline{T(B_X)}^{\,\|\cdot\|}\text{ is weakly compact}
\iff T^{**}(X^{**})\subseteq J_YY.}
$$

The [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md) on the right specifies exactly which copy of $Y$ is intended.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
