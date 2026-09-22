<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The printed differential in the transform integral is $dz$; it must be $dt$, since $z$ is the transform parameter. We prove the [Newman Tauberian theorem](../../../../../../newman-tauberian-theorem.md) in this corrected interpretation. Set

$$
F_T(z)=\int_0^T f(t)e^{-tz}\,dt,\qquad |f(t)|\leq M
$$

almost everywhere. The finite-interval transform $F_T$ is entire.

Fix $R>0$. Because the analytic domain contains the whole imaginary axis, compactness supplies a $\delta>0$ such that the thin rectangle $-\delta\leq\operatorname{Re}z\leq0$, $|\operatorname{Im}z|\leq R$ lies in the domain. Let $C_+$ be the right semicircle of radius $R$, oriented from $-iR$ to $iR$. Join its endpoints by a leftward path $L$ along the other three sides of that rectangle. This is a closed positively oriented contour.

Use [contour damping for bounded Laplace transforms](../../../../../../contour-damping-for-bounded-laplace-transforms.md) with

$$
K_T(z)=e^{Tz}\left(1+\frac{z^2}{R^2}\right)\frac1z.
$$

The [residue theorem](../../../../../../residue-theorem.md) gives

$$
F(0)-F_T(0)=\frac1{2\pi i}
\left[\int_{C_+}(F-F_T)K_T\,dz
+\int_L FK_T\,dz-\int_L F_TK_T\,dz\right].
$$

On $C_+$, with $x=\operatorname{Re}z>0$,

$$
|e^{Tz}(F-F_T)(z)|\leq M/x,\qquad
\left|1+z^2/R^2\right|=2x/R.
$$

Thus the integrand has modulus at most $2M/R^2$, and this half-circle contributes at most $M/R$ after division by $2\pi$.

On $L$, the $F$ term tends to zero as $T\to\infty$: every interior point of the path has negative real part, $F$ is bounded on this fixed compact path, and the remaining kernel factor is bounded because the path avoids zero. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) applies, with the two endpoints irrelevant to the path integral.

For the $F_T$ term, deform $L$ to the left semicircle $C_-$ of radius $R$. This deformation uses only the [entire function](../../../../../../entire-function.md) $F_T$; it does not demand that $F$ extend across a large left half-disk. Both paths lie to the left of zero and their enclosed deformation region avoids the kernel pole. On $C_-$, for $x<0$,

$$
|e^{Tz}F_T(z)|
\leq M\int_0^T e^{(T-t)x}\,dt\leq M/|x|.
$$

The same circle factor gives another bound $M/R$. Consequently

$$
\limsup_{T\to\infty}|F_T(0)-F(0)|\leq\frac{2M}{R}.
$$

The radius $R$ is arbitrary, so

$$
\boxed{\int_0^\infty f(t)\,dt=\lim_{T\to\infty}F_T(0)=F(0).}
$$

This proves convergence of the ordinary improper integral, not merely a damped limit.

For the weakened domain hypothesis, take $f(t)=1$. Its [Laplace transform](../../../../../../laplace-transform.md) is $F(z)=1/z$, analytic on the open right half-plane, but $\int_0^T f(t)\,dt=T$ diverges. **Analyticity only in the open right half-plane is insufficient.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
