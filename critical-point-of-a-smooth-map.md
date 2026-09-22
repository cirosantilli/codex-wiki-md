# Critical point of a smooth map

↑ **Parent:** [Differential geometry](differential-geometry-split.md)

Imagine folding a sheet along its horizontal axis by the [smooth map](smooth-map-between-manifolds.md) $F:\mathbb R^2\to\mathbb R^2$, $F(x,y)=(x,y^2)$. The inputs $(a,r)$ and $(a,-r)$ have the same output. Along $y=0$, horizontal motion still changes the output, but vertical motion produces no first-order change: $F(a,\varepsilon)-F(a,0)=(0,\varepsilon^2)$. These inputs are [critical points of a smooth map](critical-point-of-a-smooth-map.md) even though their [differential](differential-of-a-smooth-map.md) is not the zero [linear map](linear-map.md). The missing direction in the target [tangent space](tangent-space.md) is what matters.

<a id="critical-points-values-fold"></a>
![](critical-points-values-fold.png)

**[Figure 2](#critical-points-values-fold). The fold $F(x,y)=(x,y^2)$: critical inputs, critical outputs, and fibers**.

Precisely, let $f:X^m\to Y^n$ be a [smooth map](smooth-map-between-manifolds.md) between [smooth manifolds](smooth-manifold.md) without boundary. An input $p\in X$ is a [critical point of a smooth map](critical-point-of-a-smooth-map.md) when its [differential](differential-of-a-smooth-map.md)

$$
df_p:T_pX\longrightarrow T_{f(p)}Y
$$

is not [surjective](surjective-function.md), equivalently when its [rank of a linear map](rank-of-a-linear-map.md) is less than $n$. An input where it is [surjective](surjective-function.md) is a regular point; a map with no [critical points of a smooth map](critical-point-of-a-smooth-map.md) is a [submersion](submersion.md). The threshold is the target [dimension](dimension-vector-space.md), not $\min(m,n)$. In [manifold charts](manifold-chart.md), compute the [matrix rank](matrix-rank.md) of the $n\times m$ [Jacobian matrix](jacobian-matrix.md); changes of charts preserve that [matrix rank](matrix-rank.md). [Eckhard Meinrenken, Differentiable Manifolds, Definitions 1.8 and 1.10](https://www.math.toronto.edu/mein/teaching/LectureNotes/Man.pdf)

For the fold,

$$
DF_{(x,y)}=\begin{pmatrix}1&0\\0&2y\end{pmatrix},\qquad
\operatorname{rank}DF_{(x,y)}=\begin{cases}2&y\ne0,\\1&y=0.\end{cases}
$$

Thus its set of [critical points of a smooth map](critical-point-of-a-smooth-map.md) is the entire horizontal axis. Away from that axis, its [differential](differential-of-a-smooth-map.md) can produce every infinitesimal target displacement. At the axis, it can produce only horizontal ones. This diagnoses where the two inverse branches in the picture merge.

For a scalar [smooth function](smooth-function.md) $f:X\to\mathbb R$, the target [dimension](dimension-vector-space.md) is one. A [linear map](linear-map.md) to $\mathbb R$ fails to be [surjective](surjective-function.md) exactly when it is zero, so here a [critical point of a smooth map](critical-point-of-a-smooth-map.md) means $df_p=0$. In [Euclidean space](euclidean-norm.md) this is precisely the familiar [critical point](critical-point.md) condition $\nabla f(p)=0$: every first [partial derivative](partial-derivative.md) vanishes. On a [Riemannian manifold](riemannian-manifold.md), it is equivalently $\nabla_gf(p)=0$ for the chosen [Riemannian metric](riemannian-metric.md); the [Riemannian gradient](riemannian-gradient.md) depends on that metric, but whether it vanishes does not. See [Loring W. Tu, An Introduction to Manifolds, Proposition 8.23](https://www.math.toronto.edu/~jeffrey/matd67/tu.pdf) for the scalar coordinate criterion. The scalar [smooth function](smooth-function.md) $f(t)=t^3$ has a [critical point](critical-point.md) at zero without a [local maximum](local-maximum.md) or [local minimum](local-minimum.md).

A source of lower [dimension](dimension-vector-space.md) gives a different warning. For the [smooth map](smooth-map-between-manifolds.md) $G:\mathbb R\to\mathbb R^2$, $G(t)=(t,t^2)$, the [Jacobian matrix](jacobian-matrix.md) is the column $(1,2t)^T$, of [matrix rank](matrix-rank.md) one at every input. Every input is a [critical point of a smooth map](critical-point-of-a-smooth-map.md), since the target [dimension](dimension-vector-space.md) is two, even though this [parametric curve](parametric-curve.md) has nonzero [velocity](velocity.md) everywhere and is an [immersion](immersion.md). More generally, if $m<n$, no [differential](differential-of-a-smooth-map.md) $T_pX\to T_{f(p)}Y$ can be [surjective](surjective-function.md), so every input is critical. The terminology measures the ability to fill target directions, rather than whether the parametrized [curve](curve.md) looks smooth.

**Table of contents**

- [Critical value](critical-value.md)

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Critical point of a smooth map](critical-point-of-a-smooth-map.md)
- [Critical value](critical-value.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/24h/i/solution.md)
