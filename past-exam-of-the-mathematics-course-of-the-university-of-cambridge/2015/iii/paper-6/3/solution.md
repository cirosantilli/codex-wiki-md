<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

All [vector spaces](../../../../../vector-space-split.md) in this solution are complex, while [convex combinations](../../../../../convex-combination.md) use real coefficients. An [extreme point](../../../../../extreme-point.md) $x$ of a [convex set](../../../../../convex-set.md) $C$ is one for which $x=ty+(1-t)z$, $y,z\in C$ and $0<t<1$, forces $y=z=x$. Equivalently, $x$ is not the midpoint of two distinct points of $C$.

The [Krein-Milman theorem](../../../../../krein-milman-theorem.md) says that every nonempty compact [convex set](../../../../../convex-set.md) $K$ in a Hausdorff [locally convex space](../../../../../locally-convex-space.md) is the [closed convex hull](../../../../../closed-convex-hull.md) of its [extreme points](../../../../../extreme-point.md). Here is a proof. A [face of a convex set](../../../../../face-of-a-convex-set.md) $F\subseteq K$ is a [convex set](../../../../../convex-set.md) such that whenever an interior point of a segment in $K$ belongs to $F$, both endpoints belong to $F$. Consider nonempty compact faces, ordered by reverse inclusion. A chain has nonempty intersection by compactness and the [finite intersection property](../../../../../finite-intersection-property.md); that intersection is again a compact face. The [Zorn lemma](../../../../../zorn-s-lemma.md) therefore gives a minimal nonempty compact face $F$.

If $F$ contains distinct $x,y$, a continuous real [linear functional](../../../../../linear-functional.md) $\ell$ on the underlying real [locally convex space](../../../../../locally-convex-space.md) distinguishes them. Such a [linear functional](../../../../../linear-functional.md) exists because the space is Hausdorff and locally convex, by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). The maximizers of $\ell$ on $F$ form a nonempty proper compact face of $F$. A face of a face is a face of $K$, contradicting minimality. Therefore $F$ is a singleton, yielding an [extreme point](../../../../../extreme-point.md). The same argument inside any nonempty compact face of $K$ supplies an [extreme point](../../../../../extreme-point.md) of $K$ lying in that face.

Let $D$ be the [closed convex hull](../../../../../closed-convex-hull.md) of the [extreme points](../../../../../extreme-point.md) of $K$. It is a nonempty closed subset of compact $K$, hence compact. If $x_0\in K\setminus D$, the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) provides a continuous real [linear functional](../../../../../linear-functional.md) $\ell$ with $\ell(x_0)>\sup_D\ell$. Its maximizer set on $K$ is a nonempty compact face, which contains an [extreme point](../../../../../extreme-point.md) $e$ of $K$. But $e\in D$ and $\ell(e)\geq\ell(x_0)>\sup_D\ell$, a contradiction. Thus **$\boxed{K=\overline{\operatorname{co}}(\operatorname{ext}K)}$**, proving [Krein-Milman theorem](../../../../../krein-milman-theorem.md).

For a nonempty compact [Hausdorff space](../../../../../hausdorff-space.md) $K$, the [extreme points of the dual unit ball of C(K)](../../../../../extreme-points-of-the-dual-unit-ball-of-c-k.md) are

$$
\boxed{\operatorname{ext}B_{C(K)^*}=\{\alpha\delta_x:x\in K,\ |\alpha|=1\},}
\qquad \delta_x(f)=f(x).
$$

This is the permitted description without proof, with $C(K)$ denoting the complex [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md) equipped with the [supremum norm](../../../../../supremum-norm.md). If $K$ is empty, $C(K)=\{0\}$ and the [closed unit ball](../../../../../closed-unit-ball.md) of its [continuous dual space](../../../../../continuous-dual-space-split.md) has the single [extreme point](../../../../../extreme-point.md) $0$ instead.

The complex [Banach–Stone theorem](../../../../../banach-stone-theorem.md) states that a surjective complex-linear [isometric isomorphism of normed spaces](../../../../../isometric-isomorphism-of-normed-spaces.md) $T:C(K)\to C(L)$ has the form

$$
\boxed{(Tf)(y)=u(y)f(\varphi(y)),\qquad |u(y)|=1,}
$$

where $u\in C(L)$ and $\varphi:L\to K$ is a [homeomorphism](../../../../../homeomorphism.md). Conversely, every such map is a surjective complex-linear [isometric isomorphism of normed spaces](../../../../../isometric-isomorphism-of-normed-spaces.md) for the [supremum norm](../../../../../supremum-norm.md).

To prove this, suppose first that $K,L$ are nonempty. The [Banach-space adjoint](../../../../../transpose-of-a-bounded-linear-operator.md) $T^*$ is a bijective [isometric isomorphism of normed spaces](../../../../../isometric-isomorphism-of-normed-spaces.md) on the [continuous dual spaces](../../../../../continuous-dual-space-split.md), so it bijects their [closed unit balls](../../../../../closed-unit-ball.md) and preserves [extreme points](../../../../../extreme-point.md). The displayed [extreme point](../../../../../extreme-point.md) description gives uniquely

$$
T^*\delta_y=u(y)\delta_{\varphi(y)},\qquad |u(y)|=1.
$$

Uniqueness follows by evaluating at the constant function $1$, and then using that [continuous functions](../../../../../continuous-function.md) separate points of a compact [Hausdorff space](../../../../../hausdorff-space.md). Evaluation gives the required formula for $Tf$, and $u=T1$ is continuous. Surjectivity of $T^*$ on [extreme points](../../../../../extreme-point.md) proves surjectivity of $\varphi$: the preimage of any $\delta_x$ is $\alpha\delta_y$ for some $y$. If $\varphi(y_1)=\varphi(y_2)$, every function in the range of $T$ has equal values at these two points after division by $u$; surjectivity of $T$ and separation of points force $y_1=y_2$. Thus $\varphi$ is bijective.

For every $f\in C(K)$, $f\circ\varphi=(Tf)/u$ is continuous. The evaluation map $K\to\mathbb C^{C(K)}$, $x\mapsto(f(x))_f$, is a continuous injection of a compact [Hausdorff space](../../../../../hausdorff-space.md) into a Hausdorff [product topology](../../../../../product-topology.md), hence a [homeomorphism](../../../../../homeomorphism.md) onto its image. Continuity of every coordinate $f\circ\varphi$ proves continuity of $\varphi$. A continuous bijection between compact [Hausdorff spaces](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md). Conversely the weighted-composition formula plainly preserves the [supremum norm](../../../../../supremum-norm.md), and its inverse is

$$
(T^{-1}g)(x)=\frac{g(\varphi^{-1}(x))}{u(\varphi^{-1}(x))}.
$$

If one compact space is empty, a surjective [isometric isomorphism of normed spaces](../../../../../isometric-isomorphism-of-normed-spaces.md) forces the other to be empty, and the empty [homeomorphism](../../../../../homeomorphism.md) gives the corresponding trivial case. This completes [Banach–Stone theorem](../../../../../banach-stone-theorem.md).

Neither the [space of sequences converging to zero](../../../../../space-of-sequences-converging-to-zero.md) $c_0$ nor $L^1[0,1]$ can be isometrically a [continuous dual space](../../../../../continuous-dual-space-split.md) of a [Banach space](../../../../../banach-space-split.md). Indeed, every nonzero [continuous dual space](../../../../../continuous-dual-space-split.md) has a nonempty weak-star compact [closed unit ball](../../../../../closed-unit-ball.md) by [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md), and [Krein-Milman theorem](../../../../../krein-milman-theorem.md) then guarantees an [extreme point](../../../../../extreme-point.md). A bijective linear [isometry](../../../../../isometry.md) preserves [extreme points](../../../../../extreme-point.md) of [closed unit balls](../../../../../closed-unit-ball.md).

The [closed unit ball](../../../../../closed-unit-ball.md) of $c_0$ has no [extreme points](../../../../../extreme-point.md). Given $x\in c_0$ with $\|x\|_\infty\leq1$, choose $n$ with $|x_n|<1$ and $0<\varepsilon<1-|x_n|$. The two distinct elements $x\pm\varepsilon e_n$ remain in that [closed unit ball](../../../../../closed-unit-ball.md) and have midpoint $x$.

The [closed unit ball](../../../../../closed-unit-ball.md) of the complex [Lp space](../../../../../lp-space.md) $L^1[0,1]$ also has no [extreme points](../../../../../extreme-point.md). An element of [norm](../../../../../norm.md) less than one can be perturbed by a sufficiently small nonzero [Lp space](../../../../../lp-space.md) element in both directions. If $\|f\|_1=1$, the [non-atomic measure](../../../../../non-atomic-measure.md) $|f(t)|\,dt$ admits a measurable set $A$ of mass $1/2$; for example the continuous function $s\mapsto\int_0^s|f(t)|\,dt$ attains $1/2$. Put $h=f(\mathbf1_A-\mathbf1_{A^c})$. For $0<\varepsilon<1$, the distinct functions $f\pm\varepsilon h$ both have [Lp norm](../../../../../lp-norm.md)

$$
(1+\varepsilon)\int_A|f|+(1-\varepsilon)\int_{A^c}|f|=1,
$$

with the two coefficients interchanged for the minus sign. Their midpoint is $f$. Thus **neither proposed space is isometrically a Banach dual**.

Finally, $[0,1]$ is a [connected space](../../../../../connected-space.md), whereas $[0,1]\cup[2,3]$ is disconnected. They cannot be homeomorphic. By [Banach–Stone theorem](../../../../../banach-stone-theorem.md), **$C[0,1]$ and $C([0,1]\cup[2,3])$ are not isometrically isomorphic** as complex [Banach spaces](../../../../../banach-space-split.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
