<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use these standard [ultrafilter](../../../../ultrafilter.md) facts: a space is [compact](../../../../compact-space.md) if and only if every [ultrafilter](../../../../ultrafilter.md) on it converges; the image [ultrafilter](../../../../ultrafilter.md) under a map is an [ultrafilter](../../../../ultrafilter.md); and a convergent [ultrafilter](../../../../ultrafilter.md) contains every [neighborhood](../../../../neighbourhood-mathematics.md) of its limit.

Let $X=\prod_{\lambda\in\Lambda}X_\lambda$ with all factors [compact](../../../../compact-space.md). An empty factor makes $X$ empty and hence [compact](../../../../compact-space.md). Otherwise, given an [ultrafilter](../../../../ultrafilter.md) $\mathcal U$ on $X$, push it forward by each [product projection](../../../../product-projection.md) to obtain an [ultrafilter](../../../../ultrafilter.md) $\mathcal U_\lambda$ on $X_\lambda$. Choose a limit $x_\lambda$ of each, and put $x=(x_\lambda)_\lambda$. A basic product [neighborhood](../../../../neighbourhood-mathematics.md) of $x$ is an intersection of finitely many inverse images of coordinate [neighborhoods](../../../../neighbourhood-mathematics.md). Each inverse image belongs to $\mathcal U$, so their [finite intersection](../../../../finite-intersection.md) does too. Thus $\mathcal U$ converges to $x$, proving **[compactness](../../../../compact-space.md) of the product**. Uniqueness of coordinate limits is not needed, so the factors need not be [Hausdorff](../../../../hausdorff-space.md).

For [local compactness](../../../../locally-compact-space.md), suppose only the factors indexed by a finite set $F$ may be noncompact. At $x\in X$ choose, for each $\lambda\in F$, a [compact](../../../../compact-space.md) [neighborhood](../../../../neighbourhood-mathematics.md) $K_\lambda$ of $x_\lambda$, with an [open neighborhood](../../../../open-neighbourhood.md) $U_\lambda\subseteq K_\lambda$. For other indices put $K_\lambda=X_\lambda$. The [compact](../../../../compact-space.md) product $\prod_\lambda K_\lambda$ contains the open product [neighborhood](../../../../neighbourhood-mathematics.md) restricting just the finitely many coordinates in $F$ to $U_\lambda$. Hence every [point](../../../../point-geometry.md) has a [compact](../../../../compact-space.md) [neighborhood](../../../../neighbourhood-mathematics.md) and **the product is locally [compact](../../../../compact-space.md)**.

The unrestricted assertion is **false**. Each factor of $\mathbb R^{\mathbb N}$ is locally [compact](../../../../compact-space.md), but its product is not. Any basic [neighborhood](../../../../neighbourhood-mathematics.md) restricts only finitely many coordinates. Choose a free coordinate $j$; its projection of that [neighborhood](../../../../neighbourhood-mathematics.md) is all of $\mathbb R$. A [compact](../../../../compact-space.md) [neighborhood](../../../../neighbourhood-mathematics.md) containing it would consequently have [compact](../../../../compact-space.md) image equal to $\mathbb R$, impossible. This shows directly that no [point](../../../../point-geometry.md) has a [compact](../../../../compact-space.md) [neighborhood](../../../../neighbourhood-mathematics.md).

## ↑ Ancestors (12)

1. [1](../1.md)
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
