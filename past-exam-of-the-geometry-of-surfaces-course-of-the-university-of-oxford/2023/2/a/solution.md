<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $x\in X$ and choose holomorphic [coordinate charts](../../../../manifold-chart.md) centred at $x$ and $f(x)$. A nonconstant [holomorphic map](../../../../holomorphic-map.md) has a local expansion $w\circ f(z)=c z^m+O(z^{m+1})$, where $c\ne0$ and $m\geq1$. Taking a local holomorphic $m$th root of the nonvanishing factor and changing the source coordinate gives the exact local form $w=z^m$. The integer

$$
\boxed{\nu_f(x)=m}
$$

is the [ramification index of a holomorphic map](../../../../ramification-index-of-a-holomorphic-map.md). A [ramification point of a holomorphic map](../../../../ramification-point-of-a-holomorphic-map.md) is a source point with $\nu_f(x)>1$, equivalently where its [derivative](../../../../derivative.md) vanishes; a [branch value of a holomorphic map](../../../../branch-value-of-a-holomorphic-map.md), also called a branch point here, is the image of such a point in $Y$. These are different sets, one in the source and one in the target.

Every [fiber of a function](../../../../fiber-of-a-function.md) is finite: locally it is the zero set of a nonzero [holomorphic function](../../../../holomorphic-function-split.md), so its points are isolated, and [compactness](../../../../compact-space.md) prevents infinitely many such zeros without an accumulation point. The same argument applied to the local [derivatives](../../../../derivative.md) makes the set of [ramification points of a holomorphic map](../../../../ramification-point-of-a-holomorphic-map.md) finite. The [open mapping theorem](../../../../open-mapping-theorem-functional-analysis.md) and [compactness](../../../../compact-space.md) show that $f(X)$ is both open and closed in the [connected](../../../../connected-space.md) target $Y$, hence $f$ is [surjective](../../../../surjective-function.md).

For any $y\in Y$, the [degree of a holomorphic map](../../../../degree-of-a-holomorphic-map.md) is

$$
\boxed{d=\deg f=\sum_{x\in f^{-1}(y)}\nu_f(x).}
$$

To see independence of $y$, choose disjoint small [coordinate charts](../../../../manifold-chart.md) about its finitely many preimages. The local form $z\mapsto z^{\nu_f(x)}$ shows that nearby values have $\nu_f(x)$ preimages counted with multiplicity in the corresponding chart. [Compactness](../../../../compact-space.md) excludes additional preimages outside these charts for sufficiently nearby values: a sequence of such preimages would have a limit in $f^{-1}(y)$. The displayed sum is therefore locally constant, hence constant on [connected](../../../../connected-space.md) $Y$. Away from [branch values of a holomorphic map](../../../../branch-value-of-a-holomorphic-map.md) it is the ordinary number of preimages, and $f$ is a $d$-sheeted [covering map](../../../../covering-space.md) there.

The [Riemann-Hurwitz formula](../../../../riemann-hurwitz-formula.md) is

$$
\boxed{\chi(X)=d\chi(Y)-\sum_{x\in X}(\nu_f(x)-1),}
$$

or, in terms of the two [genera](../../../../genus-of-a-surface.md),

$$
\boxed{2g_X-2=d(2g_Y-2)+\sum_{x\in X}(\nu_f(x)-1).}
$$

For its proof, choose a [triangulation of a surface](../../../../triangulation-of-a-surface.md) on $Y$ containing every [branch value of a holomorphic map](../../../../branch-value-of-a-holomorphic-map.md) among its vertices. Every open edge and open face has $d$ lifts, since its interior avoids [branch values of a holomorphic map](../../../../branch-value-of-a-holomorphic-map.md). The lifted cells give a finite [CW complex](../../../../cw-complex.md) structure on $X$. If $V_Y,E_Y,F_Y$ are the target counts and $R=\sum_x(\nu_f(x)-1)$, the source counts are

$$
E_X=dE_Y,\qquad F_X=dF_Y,\qquad
V_X=\sum_{y\text{ vertex}}\#f^{-1}(y)=dV_Y-R.
$$

Indeed, at a target vertex the deficit from $d$ distinct preimages is precisely $\sum_{x\mapsto y}(\nu_f(x)-1)$, and all nonzero contributions occur over vertices. Taking the alternating sum gives $\chi(X)=d(V_Y-E_Y+F_Y)-R$, as required. This is the [Triangulation proof of the Riemann-Hurwitz formula](../../../../triangulation-proof-of-the-riemann-hurwitz-formula.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
