<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $Q=Q_r(x)$ and $v_Q=|Q|^{-1}\int_Qv$. The [fundamental theorem of calculus along a line segment](../../../../../../fundamental-theorem-of-calculus-along-a-line-segment.md), followed by averaging, gives

$$
|v(y)-v_Q|\leq\frac1{r^n}\int_Q\int_0^1|Dv(y+t(z-y))|\,|z-y|\,dt\,dz.
$$

For fixed $t$, use the [change of variables formula](../../../../../../change-of-variables-formula.md) $w=y+t(z-y)$. Its [Jacobian determinant](../../../../../../jacobian-determinant.md) is $t^n$. The transformed domain $Q_t=y+t(Q-y)$ lies in $Q$, because a cube is a [convex set](../../../../../../convex-set.md). Moreover, $w\in Q_t$ implies $|w-y|\leq\sqrt n\,rt$. Thus [Tonelli theorem](../../../../../../tonelli-theorem.md) gives

$$
\begin{aligned}
|v(y)-v_Q|
&\leq\frac1{r^n}\int_Q |Dv(w)|\,|w-y|
\int_{|w-y|/(\sqrt n r)}^1t^{-n-1}dt\,dw\\
&\leq C_n\int_Q\frac{|Dv(w)|}{|w-y|^{n-1}}\,dw.
\end{aligned}
$$

The diagonal $w=y$ is a null set. The [Holder inequality](../../../../../../holder-inequality.md) with $p'=p/(p-1)$ now applies: $p>n$ implies $(n-1)p'<n$, and integration in [spherical coordinates](../../../../../../spherical-coordinate-system.md) bounds the kernel by

$$
\left(\int_Q|w-y|^{-(n-1)p'}dw\right)^{1/p'}
\leq C_{n,p}r^{n/p'-(n-1)}=C_{n,p}r^{1-n/p}.
$$

This proves the [Morrey inequality on a cube](../../../../../../morrey-inequality-on-a-cube.md), uniformly even when $y$ approaches its boundary:

$$
\boxed{|v_Q-v(y)|\leq C_1r^{1-n/p}\|Dv\|_{L^p(Q)}.}
$$

Apply this at both $y$ and the center $x$ and use the triangle inequality to obtain

$$
\boxed{|v(y)-v(x)|\leq C_2r^{1-n/p}\|Dv\|_{L^p(Q)},\qquad C_2=2C_1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
