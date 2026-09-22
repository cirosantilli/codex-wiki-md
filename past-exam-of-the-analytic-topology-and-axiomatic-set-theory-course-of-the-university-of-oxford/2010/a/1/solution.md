<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [T0 space](../../../../kolmogorov-space.md) distinguishes any two distinct points by an [open set](../../../../open-set.md) containing one and not the other. A [Tychonoff space](../../../../completely-regular-hausdorff-space.md), also called a completely regular [Hausdorff](../../../../hausdorff-space.md) space, is a $T_1$ space in which a point outside a [closed set](../../../../closed-set.md) can be separated from it by a [continuous function](../../../../continuous-function.md): after rescaling, $f(x)=0$ and $f|_C=1$ with values in $[0,1]$.

The [product topology](../../../../product-topology.md) has the [subbasis of a topology](../../../../subbasis-of-a-topology.md)

$$
\boxed{\{\pi_\lambda^{-1}(U):\lambda\in\Lambda,\ U\text{ open in }X_\lambda\}.}
$$

A map into the product is continuous exactly when each coordinate map is continuous. One direction follows by composition with the continuous [product projections](../../../../product-projection.md); the other follows by taking [inverse images](../../../../preimage.md) of the displayed subbasic sets.

Define the [diagonal evaluation map](../../../../diagonal-evaluation-map.md) $\Delta(x)=(f_\lambda(x))_{\lambda\in\Lambda}$. Its coordinates are continuous, so the map is continuous by [continuity into a product space](../../../../continuity-into-a-product-space.md). Point separation makes it [injective](../../../../injective-function.md). For a basic [open set](../../../../open-set.md) $B=f_\lambda^{-1}(U)$,

$$
\Delta(B)=\Delta(X)\cap\pi_\lambda^{-1}(U).
$$

Every [open subset](../../../../open-set.md) of $X$ is a [union](../../../../set-union.md) of such $B$, so its image is open in $\Delta(X)$. The inverse on the image is continuous, and $\boxed{\Delta\text{ is a topological embedding}}$. If $X$ is $T_0$, any two distinct points are distinguished by an [open set](../../../../open-set.md) and then by one basic neighborhood within it. Equality of all coordinates would prevent that distinction. Thus the basis hypothesis alone implies point separation in a $T_0$ space. The unsubscripted $f$ in the printed separation hypothesis is understood as the chosen coordinate $f_\lambda$.

For the [Sierpiński space](../../../../sierpinski-space.md) $S=\{0,1\}$ with opens $\varnothing,\{1\},S$, each open $U\subseteq X$ gives a continuous characteristic map $\chi_U:X\to S$ with $\chi_U^{-1}(\{1\})=U$. These [inverse images](../../../../preimage.md) form the whole [topology](../../../../topology-split.md), hence a basis. In a $T_0$ space they separate points, proving the embedding into $S^{\tau}$.

For a [Tychonoff space](../../../../completely-regular-hausdorff-space.md), use all [continuous maps](../../../../continuous-map.md) $X\to[0,1]$. Given $x\in U$ with $U$ open, complete regularity supplies $f(x)=0$ and $f=1$ on $X\setminus U$. Then $f^{-1}([0,1/2))$ is an [open neighborhood](../../../../open-neighbourhood.md) of $x$ contained in $U$. These [inverse images](../../../../preimage.md) form a basis. The diagonal theorem gives an embedding into a product of closed unit intervals.

**A three-point space works even without any separation axiom.** Take

$$
\boxed{Y=\{0,1,2\},\qquad\tau_Y=\{\varnothing,\{2\},Y\}.}
$$

For each open $U$ of an arbitrary space, let $g_U=2$ on $U$ and $0$ elsewhere. It is continuous. For each point $a$, let $h_a=1$ at $a$ and $0$ elsewhere. It is also continuous, because its image lies in the subspace $\{0,1\}$ of $Y$, which has the [indiscrete topology](../../../../indiscrete-topology.md); equivalently $h_a^{-1}(\{2\})=\varnothing$. The $g_U$ supply every [open set](../../../../open-set.md) as an [inverse image](../../../../preimage.md), and the $h_a$ distinguish every pair of points. Using the [diagonal evaluation map](../../../../diagonal-evaluation-map.md) for their combined family gives a [universal three-point space for product embeddings](../../../../universal-three-point-space-for-product-embeddings.md):

$$
\boxed{X\hookrightarrow Y^{\tau\sqcup X}.}
$$

Finally embed the given completely regular [Hausdorff](../../../../hausdorff-space.md) space into a cube $K=[0,1]^I$. The [Tychonoff theorem](../../../../tychonoff-s-theorem.md) makes $K$ [compact](../../../../compact-space.md); it is [Hausdorff](../../../../hausdorff-space.md) and hence normal. The image of the [compact subset](../../../../compact-space.md) $C$ is [compact](../../../../compact-space.md), so closed in $K$. The [Tietze extension theorem](../../../../tietze-extension-theorem.md) says that a continuous bounded real-valued function on a [closed subset](../../../../closed-set.md) of a [normal space](../../../../normal-space.md) extends continuously to the whole space. The given function on $C$ is bounded by [compactness](../../../../compact-space.md), so apply this theorem to its transported function on the image of $C$ in $K$. Restrict the extension to the image of $X$ and pull it back along the embedding. This yields $\boxed{F:X\to\mathbb R\text{ continuous},\ F|_C=f}$. This proves that [compact subsets of Tychonoff spaces are C-embedded](../../../../compact-subsets-of-tychonoff-spaces-are-c-embedded.md), using normality of the [compact](../../../../compact-space.md) cube.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
