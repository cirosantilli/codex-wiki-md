<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

First we prove the [Krein-Milman theorem](../../../../../krein-milman-theorem.md) in the required setting. If $K$ is empty the conclusion is immediate, so assume it is nonempty. A [face of a convex set](../../../../../face-of-a-convex-set.md) is a convex subset $F$ with the property that an interior point of a segment in $K$ belongs to $F$ only if both endpoints do. Consider all nonempty weakly compact faces of $K$, ordered by reverse inclusion. A chain has a nonempty intersection by [compactness](../../../../../compact-space.md) and the finite intersection property; that intersection is again a compact face. The [Zorn lemma](../../../../../zorn-s-lemma.md) gives a minimal compact face $F$.

If $F$ contained distinct points, a bounded [linear functional](../../../../../linear-functional.md) separating them would be nonconstant on $F$. Its maximizer set is a nonempty proper compact face of $F$, hence a face of $K$, contradicting minimality. Therefore $F$ is a singleton and its member is an [extreme point](../../../../../extreme-point.md) of $K$. The same reasoning applies to each nonempty compact face of $K$, so each such face contains an [extreme point](../../../../../extreme-point.md) of $K$.

Let $H$ be the norm-[closed convex hull](../../../../../closed-convex-hull.md) of the [extreme points](../../../../../extreme-point.md) of $K$. A weakly compact subset of a Banach space is weakly closed, hence norm closed, so $H\subseteq K$. If $x\in K\setminus H$, the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) gives $\ell\in E'$ with $\ell(x)>\sup_H\ell$. The maximizer face of $\ell$ on $K$ contains an [extreme point](../../../../../extreme-point.md) $e$ of $K$. Then $\ell(e)\geq\ell(x)>\sup_H\ell$, contradicting $e\in H$. We conclude

$$
\boxed{K=\overline{\operatorname{conv}}\operatorname{Ex}(K).}
$$

Norm and weak closed convex hulls coincide by the same separation theorem. The printed phrase “closed convex cover” is understood in this standard closed-convex-hull sense.

Now work in the real [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md) $C(C)$ on the [Cantor set](../../../../../cantor-set.md). The [extreme points of a real continuous-function unit ball](../../../../../extreme-points-of-a-real-continuous-function-unit-ball.md) are exactly the continuous sign functions:

$$
\boxed{\operatorname{Ex}(B)=\{f\in C(C):f(x)\in\{-1,1\}\text{ for every }x\in C\}.}
$$

If $|f(x_0)|<1$, continuity supplies a neighbourhood where $|f|\leq1-\varepsilon$. The [Cantor cylinder](../../../../../cantor-cylinder.md) sets form a [clopen](../../../../../clopen-set.md) base, so choose a nonempty cylinder $D$ inside that neighbourhood. Its [indicator function](../../../../../indicator-function.md) is continuous, and $f\pm\varepsilon1_D$ are distinct members of $B$ with midpoint $f$. Hence $f$ is not extreme. Conversely, if $f$ is pointwise sign-valued and $f=(g+h)/2$ with $g,h\in B$, equality at the endpoint of the scalar interval $[-1,1]$ forces $g(x)=h(x)=f(x)$ at every point.

To prove the closed-hull assertion without assuming weak [compactness](../../../../../compact-space.md), take $f\in B$ and $\varepsilon>0$. A sufficiently fine finite partition of $C$ into [Cantor cylinders](../../../../../cantor-cylinder.md) has oscillation of $f$ less than $\varepsilon$ on each cell, by [uniform continuity](../../../../../uniform-continuity.md). Choose a value $a_j\in[-1,1]$ on each cell and let $h$ be the corresponding continuous step function. Then $\|f-h\|_\infty<\varepsilon$. For each sign vector $s\in\{-1,1\}^m$, let $e_s$ take value $s_j$ on cell $j$, and assign the weight

$$
w_s=\prod_{j=1}^m\frac{1+s_ja_j}{2}.
$$

These weights are nonnegative, sum to one, and satisfy $\sum_s w_s s_j=a_j$. Thus $h=\sum_s w_se_s$ is a [convex combination](../../../../../convex-combination.md) of [extreme points](../../../../../extreme-point.md). This is [clopen sign approximation in the real Cantor unit ball](../../../../../clopen-sign-approximation-in-the-real-cantor-unit-ball.md), proving

$$
\boxed{B=\overline{\operatorname{conv}}\operatorname{Ex}(B).}
$$

Nevertheless $B$ is not weakly compact. The suggested functions $f_n(x)=\min(3^nx,1)$ lie in $B$ and converge pointwise to the function equal to zero at $0$ and one at every other point of $C$. It is discontinuous at zero, since $2\cdot3^{-j}\in C$ tends to zero. If $B$ were weakly compact, the sequence, viewed as a net, would have a weakly convergent [subnet](../../../../../subnet-of-a-net.md) with limit in $C(C)$. Point evaluations are [bounded linear functionals](../../../../../continuous-linear-functional.md), so that [subnet](../../../../../subnet-of-a-net.md) would have the same pointwise limit; its indices are cofinal in the original sequence. The limit would therefore be the discontinuous function just described, a contradiction. This [discontinuous pointwise limit obstruction to weak compactness](../../../../../discontinuous-pointwise-limit-obstruction-to-weak-compactness.md) gives **the required failure of weak [compactness](../../../../../compact-space.md)**, despite the closed-hull equality.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
