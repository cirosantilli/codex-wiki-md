<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $D=\operatorname{diag}(a_1,\ldots,a_{n+1})$. The invertible [linear map](../../../../../../linear-map.md) $x\mapsto u=Dx$ takes the [ellipsoid](../../../../../../ellipsoid.md) to the unit [sphere](../../../../../../sphere.md) $S^n$. Write $u=(v,s)$ with $v\in\mathbb R^n$, and let $N=(0,1)$ and $S=(0,-1)$ be its two poles. The following two [stereographic projections](../../../../../../stereographic-projection.md) define [manifold charts](../../../../../../manifold-chart.md) on the ellipsoid:

$$
U_N=\mathcal Q_n\setminus\{D^{-1}N\},\qquad \chi_N(x)=\frac{v}{1-s},\qquad U_S=\mathcal Q_n\setminus\{D^{-1}S\},\qquad \chi_S(x)=\frac{v}{1+s}.
$$

Their ranges are $\mathbb R^n$. With $r^2=|w|^2$, their inverses, followed by $D^{-1}$, are

$$
\chi_N^{-1}(w)=D^{-1}\left(\frac{2w}{1+r^2},\frac{r^2-1}{1+r^2}\right),\qquad \chi_S^{-1}(w)=D^{-1}\left(\frac{2w}{1+r^2},\frac{1-r^2}{1+r^2}\right).
$$

These are continuous and [smooth functions](../../../../../../smooth-function.md), and directly satisfy the defining constraint. On the overlap, the [smooth transition map](../../../../../../smooth-transition-map.md) is

$$
\boxed{\chi_S\circ\chi_N^{-1}(w)=\frac{w}{|w|^2}\quad(w\ne0).}
$$

It is its own inverse and is smooth away from zero. The two domains are open in the [subspace topology](../../../../../../subspace-topology.md) and cover the ellipsoid. Its [subspace topology](../../../../../../subspace-topology.md) is inherited from [Euclidean space](../../../../../../euclidean-norm.md), so the ellipsoid is [Hausdorff](../../../../../../hausdorff-space.md) and has a [second-countable space](../../../../../../second-countable-space.md) topology. Thus these charts form a [smooth atlas](../../../../../../smooth-atlas.md) and make it an $n$-dimensional [smooth manifold](../../../../../../smooth-manifold.md), with an explicit [diffeomorphism](../../../../../../diffeomorphism.md) to $S^n$. For the degenerate dimension $n=0$, each chart consists of a single point with range $\mathbb R^0$, and their overlap is empty; the same conclusion holds.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
