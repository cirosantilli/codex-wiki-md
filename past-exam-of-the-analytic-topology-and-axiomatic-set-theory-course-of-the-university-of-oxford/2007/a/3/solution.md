<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $\alpha X=X\cup\{\infty_X\}$. Its [open sets](../../../../open-set.md) are the open subsets of $X$ together with sets $\alpha X\setminus K$, where $K$ is a [compact subset](../../../../compact-space.md) of $X$. [Compact subsets](../../../../compact-space.md) of the [Hausdorff space](../../../../hausdorff-space.md) $X$ are closed. This fact, and finite unions of [compact sets](../../../../compact-space.md), verify the topology axioms, including intersections of an old [open set](../../../../open-set.md) with a [neighborhood](../../../../neighbourhood-mathematics.md) of infinity. The inclusion $h_1:X\to\alpha X$ is a [topological embedding](../../../../topological-embedding.md) with open image.

An [open cover](../../../../open-cover.md) of $\alpha X$ has a member containing infinity; its complement is [compact](../../../../compact-space.md) in $X$ and therefore is covered by finitely many other members. This proves [compactness](../../../../compact-space.md). Two [points](../../../../point-geometry.md) of $X$ can be separated in $X$. A [point](../../../../point-geometry.md) $x$ and infinity can be separated by an [open neighborhood](../../../../open-neighbourhood.md) $U$ of $x$ contained in a [compact](../../../../compact-space.md) [neighborhood](../../../../neighbourhood-mathematics.md) $K$, and $\alpha X\setminus K$. Thus $\alpha X$ is [Hausdorff](../../../../hausdorff-space.md). Since $X$ is noncompact, every [neighborhood](../../../../neighbourhood-mathematics.md) of infinity meets $X$, so the embedded copy of $X$ is [dense](../../../../dense-set.md). This proves it is a **[Hausdorff](../../../../hausdorff-space.md) compactification**.

For a [proper map](../../../../proper-map.md), use the standard locally [compact](../../../../compact-space.md) [Hausdorff](../../../../hausdorff-space.md) convention: it is [continuous](../../../../continuous-function.md) and inverse images of [compact sets](../../../../compact-space.md) are [compact](../../../../compact-space.md). Define

$$
\boxed{\alpha f(h_1(x))=h_2(f(x)),\qquad\alpha f(\infty_X)=\infty_Y.}
$$

An open subset of $Y$ has open inverse image in $X$, hence in $\alpha X$. A basic [neighborhood](../../../../neighbourhood-mathematics.md) $\alpha Y\setminus K$ of infinity has inverse image $\alpha X\setminus f^{-1}(K)$, open because $f^{-1}(K)$ is [compact](../../../../compact-space.md). Hence $\alpha f$ is [continuous](../../../../continuous-function.md) and the diagram commutes. Any [continuous](../../../../continuous-function.md) map from a [compact space](../../../../compact-space.md) to a [Hausdorff space](../../../../hausdorff-space.md) is proper: a [compact subset](../../../../compact-space.md) of the target is closed, its inverse image is closed in the [compact](../../../../compact-space.md) domain and therefore [compact](../../../../compact-space.md). This proves the required properness.

The last requested extension **does not exist**, even as a [continuous](../../../../continuous-function.md) map. Both sequences $h_1(0,n)$ and $h_1(1,n)$ tend to $\infty_{\mathbb R^2}$, since they eventually leave every [compact subset](../../../../compact-space.md) of the plane. Their prescribed images would be the constant sequences $h_2(0)$ and $h_2(1)$. [Continuity](../../../../continuous-function.md) would force both distinct [points](../../../../point-geometry.md) to equal $g(\infty_{\mathbb R^2})$, contradicting uniqueness of limits in the [Hausdorff](../../../../hausdorff-space.md) compactification of the line. The original [product projection](../../../../product-projection.md) is not proper, as its inverse image of a singleton is an unbounded line.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
