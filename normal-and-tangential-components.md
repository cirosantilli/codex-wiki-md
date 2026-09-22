# Normal and tangential components

↑ **Parent:** [Unit normal](unit-normal.md)

At a point on a [plane curve](plane-curve.md), or on a [hypersurface](hypersurface.md) with [unit normal](unit-normal.md) $\mathbf n$, a [vector](vector.md) $\mathbf w$ splits into a [normal component](normal-component.md) and a [tangential component](tangential-component.md):

$$
\boxed{\mathbf w_N=(\mathbf w\cdot\mathbf n)\mathbf n,\qquad
\mathbf w_T=\mathbf w-\mathbf w_N,\qquad
\mathbf w=\mathbf w_T+\mathbf w_N.}
$$

The terms are [orthogonal projections](orthogonal-projection.md), and $\mathbf w_T\cdot\mathbf w_N=0$. Changing $\mathbf n$ to $-\mathbf n$ reverses the scalar coefficient $\mathbf w\cdot\mathbf n$, but leaves the [normal component](normal-component.md) [vector](vector.md) unchanged.

For a [plane curve](plane-curve.md), a [unit tangent vector](unit-tangent-vector.md) $T$ and a [unit normal](unit-normal.md) $N$ form an [orthonormal basis](orthonormal-basis.md), giving

$$
\mathbf w_T=(\mathbf w\cdot T)T,\qquad
\mathbf w_N=(\mathbf w\cdot N)N.
$$

At $(1,1)$ on the [parabola](parabola.md) $y=x^2$, choose $T=(1,2)^T/\sqrt5$ and $N=(-2,1)^T/\sqrt5$. For $\mathbf w=(3,1)^T$,

$$
\mathbf w\cdot T=\sqrt5,\qquad
\mathbf w\cdot N=-\sqrt5,\qquad
\boxed{\mathbf w_T=(1,2)^T,\quad \mathbf w_N=(2,-1)^T.}
$$

Their sum is $(3,1)^T$ and their [inner product](inner-product-split.md) is zero. A negative normal coefficient means that the [normal component](normal-component.md) points opposite the chosen $N$, rather than giving it a negative [Euclidean norm](euclidean-norm.md).

<a id="image-an-arbitrary-vector-at-a-point-of-a-parabola-splits-into-tangent-and-normal-projections"></a>
![](tangent-normal-vector-decomposition.png)

**[Figure 5](#image-an-arbitrary-vector-at-a-point-of-a-parabola-splits-into-tangent-and-normal-projections). An arbitrary vector at a point of a parabola splits into tangent and normal projections**. At $(1,1)$, the [vector](vector.md) $(3,1)^T$ decomposes as $(1,2)^T+(2,-1)^T$. Arrows are based at the same point; dashed connectors show their [vector addition](vector-addition.md).

These are local directions: being tangent at a point does not mean that a straight displacement stays on the [curve](curve.md). For a [space curve](space-curve.md), the normal part can have both [principal normal vector](principal-normal-vector.md) and [binormal vector](binormal-vector.md) components; projecting onto one chosen [unit normal](unit-normal.md) alone does not recover the entire normal plane.

**Table of contents**

- [Tangential and normal acceleration](tangential-and-normal-acceleration.md)
- [Normal component](normal-component.md)
- [Tangential component](tangential-component.md)

## ↑ Ancestors (7)

1. [Unit normal](unit-normal.md)
2. [Normal vector](normal-vector.md)
3. [Differential geometry](differential-geometry-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
