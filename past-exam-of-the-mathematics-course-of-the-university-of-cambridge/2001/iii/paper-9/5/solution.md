<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $s=A(S)=4\pi$, $L=L(\partial U)$, and $a=\min\{A(U),A(S\setminus U)\}$. We first prove a constant-version [spherical isoperimetric inequality](../../../../../spherical-isoperimetric-inequality.md) directly, including regions with several boundary components.

If $L\ge1$, the arithmetic bound $A(U)A(S\setminus U)\le s^2/4=4\pi^2$ already gives $A(U)A(S\setminus U)\le4\pi^2L^2$. If $L=0$, a region with smooth boundary is empty or the whole connected sphere up to boundary-null changes, and its area product is zero. For $0<L<1$, write the smooth boundary as finitely many disjoint [simple closed curves](../../../../../simple-closed-curve.md) $\gamma_j$ of lengths $l_j$. Fix a point $p_j$ on each curve. The shorter boundary arc from $p_j$ to any other point has length at most $l_j/2$, so $\gamma_j$ is contained in the closed geodesic ball of radius $l_j/2$ about $p_j$.

The complement of that small ball is connected and lies entirely on one side of $\gamma_j$. The [Jordan curve theorem](../../../../../jordan-curve-theorem.md) therefore gives a disk $E_j$ bounded by $\gamma_j$ contained in the ball. Its area satisfies

$$
A(E_j)\le2\pi(1-\cos(l_j/2))\le\frac\pi4l_j^2.
$$

The [indicator function](../../../../../indicator-function.md) of $U$ and the sum $\sum_j\mathbf1_{E_j}$ have the same jumps modulo two across every boundary curve. Their difference modulo two is consequently constant throughout the sphere off the boundary. Thus either $U$ or its complement lies in $\bigcup_jE_j$, up to its area-zero boundary. This also handles nested curves and disconnected regions. It follows that

$$
a\le\sum_jA(E_j)\le\frac\pi4\sum_jl_j^2\le\frac\pi4L^2,\qquad A(U)A(S\setminus U)\le sa\le\pi^2L^2.
$$

Combining the cases, **one valid universal choice is $\kappa=4\pi^2$**. Sharpness is not required.

For the inclusion estimate put $x=A(V)$, $d=A(D)>0$ and $y=A(V\cap D)$. Splitting $D$ into its portions inside and outside $V$ gives

$$
xd-sy=xA(D\setminus V)-(s-x)A(D\cap V).
$$

Because $0\le A(D\setminus V)\le s-x$ and $0\le A(D\cap V)\le x$, this expression lies between $-x(s-x)$ and $x(s-x)$. Apply the preceding [spherical isoperimetric inequality](../../../../../spherical-isoperimetric-inequality.md) to $V$ and divide by $sd$:

$$
\boxed{\left|\frac{A(V)}{A(S)}-\frac{A(V\cap D)}{A(D)}\right|\le\frac{\kappa L(\partial V)^2}{A(S)A(D)}.}
$$

Thus the constant in the [spherical inclusion area discrepancy](../../../../../spherical-inclusion-area-discrepancy.md) is independent of the nonempty open set $D$.

Let $g$ and $\widetilde g$ be the old and new smooth [Riemannian metrics](../../../../../riemannian-metric.md). Their area forms satisfy

$$
d\widetilde A=\theta\,dA,\qquad \theta=\sqrt{\frac{\det\widetilde g}{\det g}}>0.
$$

The determinant ratio is invariant under changes of coordinates, so $\theta$ is a globally defined smooth [function](../../../../../function-split.md). The [layer cake representation](../../../../../layer-cake-representation.md) follows from $\theta(x)=\int_0^\infty\mathbf1_{\{\theta(x)>t\}}\,dt$ and [Tonelli's theorem](../../../../../tonelli-theorem.md):

$$
\boxed{\widetilde A(U)=\int_U\theta\,dA=\int_0^\infty A(U\cap D_t)\,dt,\qquad D_t=\{x:\theta(x)>t\}.}
$$

Smoothness makes every $D_t$ open. Compactness of the sphere gives $0<m=\min\theta\le M=\max\theta<\infty$. Multiply the inclusion bound by $A(D_t)$ before integrating; for empty $D_t$ the resulting bound is trivially zero. For $t<m$, $D_t=S$ and the discrepancy is exactly zero; for $t>M$, $D_t$ is empty. Therefore

$$
\left|\frac{x}{s}\widetilde A(S)-\widetilde A(V)\right|\le\int_m^M\left|\frac{x}{s}A(D_t)-A(V\cap D_t)\right|dt\le\frac{\kappa(M-m)}s L(\partial V)^2.
$$

Dividing by $\widetilde A(S)>0$ proves

$$
\boxed{\left|\frac{A(V)}{A(S)}-\frac{\widetilde A(V)}{\widetilde A(S)}\right|\le\frac{C'L(\partial V)^2}{A(S)\widetilde A(S)},\qquad C'=\kappa(M-m).}
$$

This constant depends only on the two metrics. If $\theta$ is constant the normalized areas agree exactly, as the bound also shows.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
