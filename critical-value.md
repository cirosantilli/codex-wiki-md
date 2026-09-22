# Critical value

↑ **Parent:** [Critical point of a smooth map](critical-point-of-a-smooth-map.md)

A [critical point of a smooth map](critical-point-of-a-smooth-map.md) is an input; a [critical value](critical-value.md) is an output reached from at least one such input. For the fold $F(x,y)=(x,y^2)$, all inputs $(a,0)$ are [critical points of a smooth map](critical-point-of-a-smooth-map.md), and all outputs $(a,0)$ are [critical values](critical-value.md). The identical coordinate pairs live in different copies of $\mathbb R^2$. To classify an output $(a,b)$, inspect its entire [fiber of a function](fiber-of-a-function.md):

$$
F^{-1}(a,b)=\begin{cases}\{(a,\sqrt b),(a,-\sqrt b)\}&b>0,\\\{(a,0)\}&b=0,\\\varnothing&b<0.\end{cases}
$$

For $b>0$ both inputs have [matrix rank](matrix-rank.md) two, so the output is a [regular value](regular-value.md). For $b=0$ its input has [matrix rank](matrix-rank.md) one, so the output is a [critical value](critical-value.md). For $b<0$ the [fiber of a function](fiber-of-a-function.md) is the [empty set](empty-set.md), and the output is a [regular value](regular-value.md) despite being outside the [image of a function](image-of-a-function.md).

In general, for a [smooth map](smooth-map-between-manifolds.md) $f:X\to Y$, write $C_f$ for its set of [critical points of a smooth map](critical-point-of-a-smooth-map.md). Its set of [critical values](critical-value.md) is $f(C_f)\subseteq Y$. Equivalently, $q\in Y$ is a [critical value](critical-value.md) if some $p\in f^{-1}(q)$ has a [differential](differential-of-a-smooth-map.md) that is not [surjective](surjective-function.md). A [regular value](regular-value.md) requires a [surjective](surjective-function.md) [differential](differential-of-a-smooth-map.md) at every input in that [fiber of a function](fiber-of-a-function.md). The universal condition holds vacuously for an empty [fiber of a function](fiber-of-a-function.md): every output outside $f(X)$ is a [regular value](regular-value.md). These quantifiers are explicit in [Loring W. Tu, An Introduction to Manifolds, Definition 8.22 and its two following remarks](https://www.math.toronto.edu/~jeffrey/matd67/tu.pdf).

<a id="critical-points-values-fibers"></a>
![](critical-points-values-fibers.png)

**[Figure 3](#critical-points-values-fibers). Regular circular fibers and a critical value reached from both critical and regular inputs**.

The distinction is useful when solving equations. For a [smooth map](smooth-map-between-manifolds.md) $f:X^m\to Y^n$ between [smooth manifolds](smooth-manifold-split.md) without boundary and a [regular value](regular-value.md) $q$ with nonempty [fiber of a function](fiber-of-a-function.md), the [regular level set theorem](regular-level-set-theorem.md) makes $f^{-1}(q)$ an [embedded submanifold](embedded-submanifold.md) of [dimension](dimension-vector-space.md) $m-n$, with [tangent space](tangent-space.md)

$$
T_pf^{-1}(q)=\ker df_p.
$$

The [implicit function theorem](implicit-function-theorem.md) explains the freedom count: locally, $n$ independent equations fix $n$ coordinates and leave $m-n$ free. The [rank-nullity theorem](rank-nullity-theorem.md) gives the same count for the displayed [kernel of a linear map](kernel-of-a-linear-map-split.md). See [Eckhard Meinrenken, Differentiable Manifolds, Theorems 1.11 and 1.15](https://www.math.toronto.edu/mein/teaching/LectureNotes/Man.pdf) for the local projection description and its consequence for [level sets](level-set.md).

For example, $H:\mathbb R^2\to\mathbb R$, $H(x,y)=x^2+y^2$, has [gradient](gradient.md) $(2x,2y)$ and just one [critical point](critical-point.md), the origin, with [critical value](critical-value.md) zero. For $c>0$, its [fiber of a function](fiber-of-a-function.md) is the [circle](circle.md) of [radius](radius.md) $\sqrt c$, a one-dimensional [embedded submanifold](embedded-submanifold.md); negative $c$ are [regular values](regular-value.md) with empty [fibers](fiber-of-a-function.md). At $c=0$, the [fiber of a function](fiber-of-a-function.md) is a single point instead of a [circle](circle.md). A [critical value](critical-value.md) does not force its [fiber of a function](fiber-of-a-function.md) to be nonsmooth: that singleton is itself a zero-dimensional [embedded submanifold](embedded-submanifold.md), but the regular [dimension](dimension-vector-space.md) conclusion $2-1=1$ does not apply.

Nor does a single regular input certify a [regular value](regular-value.md). The scalar [smooth function](smooth-function.md) $h(t)=t^2(t-1)$ has $h^{-1}(0)=\{0,1\}$ and [derivative](derivative.md) $h'(t)=3t^2-2t$. The input zero is a [critical point](critical-point.md), while the input one is regular because $h'(1)=1$. Their shared output zero is nevertheless a [critical value](critical-value.md). Conversely, different [critical points of a smooth map](critical-point-of-a-smooth-map.md) can share one [critical value](critical-value.md): $f(t)=(t^2-1)^2$ sends both critical inputs $-1$ and $1$ to zero. Counting inputs and counting critical outputs are different tasks.

Finally, for $G(t)=(t,t^2):\mathbb R\to\mathbb R^2$, every output on the [parabola](parabola.md) is a [critical value](critical-value.md), and every output off it is a [regular value](regular-value.md) with empty [fiber of a function](fiber-of-a-function.md). There is no nonempty regular [fiber of a function](fiber-of-a-function.md) here, so the negative expression $1-2$ never becomes a claimed [manifold](topological-manifold-split.md) [dimension](dimension-vector-space.md). Both diagrams show exact mathematical examples, not measured data.

## ↑ Ancestors (6)

1. [Critical point of a smooth map](critical-point-of-a-smooth-map.md)
2. [Differential geometry](differential-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cobordism Morse function](cobordism-morse-function.md)
- [Critical value](critical-value.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/24h/i/solution.md)
