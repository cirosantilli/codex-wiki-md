<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The relation that $X$ is [finitely representable](../../../../../finite-representability-of-a-banach-space.md) in $Y$ means that every finite-dimensional subspace $E\subseteq X$ has, for every $\varepsilon>0$, a linear copy in $Y$ of distortion below $1+\varepsilon$. A [superreflexive Banach space](../../../../../superreflexive-banach-space.md) is one for which every Banach space finitely representable in it is a [reflexive Banach space](../../../../../reflexive-banach-space.md).

Suppose first that $X$ is reflexive and $(x_i)\subseteq B_X$. By weak compactness, the sequence has a weak cluster point $x\in B_X$. The point $x$ belongs to the weak closure of every tail convex hull, and the weak and norm closures of a convex set agree by the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md). Choose a convex combination

$$
y\in\operatorname{conv}\{x_i:1\leq i\leq n\}
$$

within $\theta/2$ of $x$, enlarging $n$ beyond all indices used. Then choose

$$
z\in\operatorname{conv}\{x_i:i>n\}
$$

within $\theta/2$ of $x$. It follows that $\|y-z\|<\theta$.

Conversely, the [James reflexivity criterion](../../../../../james-s-theorem.md) in convex-block form says that a nonreflexive Banach space has a number $\theta>0$ and a sequence $(x_i)\subseteq B_X$ such that

$$
\operatorname{dist}\left(
\operatorname{conv}\{x_1,\ldots,x_n\},
\operatorname{conv}\{x_{n+1},x_{n+2},\ldots\}
\right)\geq\theta
$$

for every $n$. One obtains this form from the usual bidual separation proof by applying the [principle of local reflexivity](../../../../../principle-of-local-reflexivity.md) to each finite-dimensional stage. Such a sequence contradicts the asserted property. This proves the [convex-block separation criterion for reflexivity](../../../../../convex-block-separation-criterion-for-reflexivity.md).

Consider now the uniform finite version. If it fails for some $\theta>0$, choose for every $N$ a sequence $(x_i^{(N)})_{i=1}^N\subseteq B_X$ for which every cut has convex-hull distance at least $\theta$. In a free [ultrapower](../../../../../ultrapower.md) $X_{\mathcal U}$, let

$$
\xi_i=[(x_i^{(N)})_{N\geq i}],
$$

filling the finitely many missing coordinates arbitrarily. Every initial-tail pair of convex hulls of $(\xi_i)$ remains at distance at least $\theta$, so the first criterion makes $X_{\mathcal U}$ nonreflexive. Since an ultrapower is finitely representable in $X$, this contradicts superreflexivity.

Conversely, if $X$ is not superreflexive, choose a nonreflexive space $Y$ finitely representable in $X$. The first criterion supplies a sequence in $B_Y$ whose convex blocks are separated by some $\theta>0$. For each $N$, transfer the span of its first $N$ vectors to $X$ with distortion arbitrarily close to one and normalize. The resulting $N$-term sequence violates the uniform condition, with separation at least, say, $\theta/2$. This proves the [uniform finite convex-block criterion for superreflexivity](../../../../../uniform-finite-convex-block-criterion-for-superreflexivity.md).

A purely metric equivalent is the [diamond-graph characterization of superreflexivity](../../../../../diamond-graph-characterization-of-superreflexivity.md):

$$
X\text{ is superreflexive}
\quad\Longleftrightarrow\quad
c_X(D_m)\longrightarrow\infty.
$$

For sufficiency, argue contrapositively. If $X$ is not superreflexive, the preceding uniform criterion supplies arbitrarily long unit-ball sequences whose convex hulls stay a fixed distance apart across every cut. At each replacement step in the diamond graph, map the two new branches to convex combinations on opposite sides of the corresponding cut. The upper bound follows from convexity and the lower bound from the fixed separation. The standard recursive diamond construction therefore embeds every $D_m$ into $X$ with one distortion constant independent of $m$. Thus divergence of the diamond distortions forces superreflexivity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 155](../../paper-155-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
