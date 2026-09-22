# Nullity of a linear map

↑ **Parent:** [Kernel of a linear map](kernel-of-a-linear-map-split.md)

The [nullity of a linear map](nullity-of-a-linear-map.md) $T:V\to W$ is $n(T)=\dim\ker T$, the [dimension](dimension-vector-space.md) of its [kernel](kernel-of-a-linear-map-split.md). It counts independent input directions that can change without changing the output. For a [finite-dimensional vector space](finite-dimensional-vector-space.md) $V$, the [rank-nullity theorem](rank-nullity-theorem.md) gives

$$
n(T)=\dim V-\operatorname{rank}T.
$$

For an $m\times n$ [matrix](matrix.md) $A$ of [matrix rank](matrix-rank.md) $r$, this is $n-r$, using the number of columns, not the number of rows. This dimension identity is [Sheldon Axler, Linear Algebra Done Right, fourth edition, §3B, theorem 3.21](linear-algebra-done-right-by-sheldon-axler-4th-edition.md).

The [nullity](nullity-of-a-linear-map.md) answers a practical question about a [linear system](system-of-linear-equations.md): once one input is known to produce the requested output, how much freedom remains? If $T(x_0)=b$, its [fiber of a function](fiber-of-a-function.md) over $b$ is

$$
\boxed{T^{-1}(\{b\})=x_0+\ker T.}
$$

Indeed, $T(x)=T(x_0)$ exactly when $T(x-x_0)=0$. Thus every nonempty [fiber](fiber-of-a-function.md) is an [affine subspace](affine-subspace.md) of [dimension](dimension-vector-space.md) $n(T)$, with the same direction space as the [kernel](kernel-of-a-linear-map-split.md). The [kernel](kernel-of-a-linear-map-split.md) itself is the [fiber](fiber-of-a-function.md) over zero. Outputs outside the [image of a linear map](image-of-a-linear-map.md) have empty [fibers](fiber-of-a-function.md); the [nullity](nullity-of-a-linear-map.md) does not guarantee existence, and we assign no solution-space [dimension](dimension-vector-space.md) to an empty [fiber](fiber-of-a-function.md) here.

<a id="image-nullity-one-gives-parallel-solution-lines-for-f-x-y-x-plus-y-0"></a>
![](singularity-nullity-fibers.png)

**[Figure 3](#image-nullity-one-gives-parallel-solution-lines-for-f-x-y-x-plus-y-0). Nullity one gives parallel solution lines for $F(x,y)=(x+y,0)$**. Each colored input [straight line](straight-line.md) $x+y=c$ is the [fiber](fiber-of-a-function.md) over the corresponding output $(c,0)$. The blue line through the origin is the [kernel](kernel-of-a-linear-map-split.md). The orange inputs $(1,0)$ and $(0,1)$ give the same output; their difference belongs to the [kernel](kernel-of-a-linear-map-split.md). The output $(1,1)$ lies outside the [image of a linear map](image-of-a-linear-map.md) and has no input. Exact toy geometry, not measured data.

In the diagram, $F:\mathbb R^2\to\mathbb R^2$ has [matrix](matrix.md) $\begin{pmatrix}1&1\\0&0\end{pmatrix}$, [matrix rank](matrix-rank.md) one and [nullity](nullity-of-a-linear-map.md) one. Its [kernel](kernel-of-a-linear-map-split.md) has [basis](basis.md) $(1,-1)$, and the full solution of $F(x,y)=(c,0)$ is $(x,y)=(c,0)+s(1,-1)$. One free [scalar](scalar.md) moves the solution along a [straight line](straight-line.md); the output $(c,1)$ is impossible.

The existing three-input example $T(x,y,z)=(x+y,z)$ instead has [rank](rank-one-quadratic-form.md) two and [nullity](nullity-of-a-linear-map.md) one. Its [image of a linear map](image-of-a-linear-map.md) is all of $\mathbb R^2$, and

$$
T^{-1}(\{(a,b)\})=(a,0,b)+\operatorname{span}\{(1,-1,0)\}.
$$

Every output has a solution [straight line](straight-line.md). In contrast, $U(x,y,z)=(x+y,0)$ has [rank](rank-one-quadratic-form.md) one and [nullity](nullity-of-a-linear-map.md) two, with [kernel](kernel-of-a-linear-map-split.md) [basis](basis.md) $(1,-1,0),(0,0,1)$. Its reachable output $(a,0)$ has the solution [affine subspace](affine-subspace.md)

$$
(x,y,z)=(a,0,0)+s(1,-1,0)+u(0,0,1),\qquad s,u\in\mathbb R,
$$

a plane, while $(a,b)$ with $b\ne0$ has no solution. These two [linear maps](linear-map.md) have the same input and output dimensions but different freedom and reachability. Computing the [kernel](kernel-of-a-linear-map-split.md) separates what an output determines from what an extra constraint would have to fix. For either example, a [basis](basis.md) of the [kernel](kernel-of-a-linear-map-split.md) gives one independent free [scalar](scalar.md) per [basis vector](basis-vector.md), which is why [nullity](nullity-of-a-linear-map.md) measures freedom rather than the number of solutions.

## ↑ Ancestors (6)

1. [Kernel of a linear map](kernel-of-a-linear-map-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Nullity of a linear map](nullity-of-a-linear-map.md)
