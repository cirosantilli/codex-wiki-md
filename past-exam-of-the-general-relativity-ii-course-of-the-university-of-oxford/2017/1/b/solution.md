<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the order $(u,v,x,y)$ the [metric tensor](../../../../metric-tensor.md) and [inverse metric](../../../../inverse-metric.md) are

$$
(g_{ab})=
\begin{pmatrix}
F&1&0&0\\
1&0&0&0\\
0&0&1&0\\
0&0&0&1
\end{pmatrix},
\qquad
(g^{ab})=
\begin{pmatrix}
0&1&0&0\\
1&-F&0&0\\
0&0&1&0\\
0&0&0&1
\end{pmatrix}.
$$

Only $g_{uu}$ has nonzero [partial derivatives](../../../../partial-derivative.md). Substitution into the formula for the [Levi-Civita connection](../../../../levi-civita-connection.md),

$$
\Gamma^a{}_{bc}
=\frac12g^{ad}
(\partial_bg_{dc}+\partial_cg_{db}-\partial_dg_{bc}),
$$

therefore gives

$$
\boxed{
\Gamma^v{}_{uu}=\frac12F_{,u},\qquad
\Gamma^v{}_{ui}=\Gamma^v{}_{iu}=\frac12F_{,i},\qquad
\Gamma^i{}_{uu}=-\frac12F_{,i}.
}
$$

Every other [Christoffel symbol](../../../../christoffel-symbol.md) vanishes. For example $g^{ud}$ selects $d=v$, and the [metric tensor](../../../../metric-tensor.md) is independent of $v$ with constant $g_{av}$; hence $\Gamma^u{}_{bc}=0$.

Use the paper's [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) convention

$$
R^d{}_{cab}
=\partial_a\Gamma^d{}_{bc}-\partial_b\Gamma^d{}_{ac}
+\Gamma^d{}_{ae}\Gamma^e{}_{bc}
-\Gamma^d{}_{be}\Gamma^e{}_{ac},
\qquad
R_{abcd}=g_{ae}R^e{}_{bcd}.
$$

For the independent components,

$$
R^v{}_{iuj}
=-\partial_j\Gamma^v{}_{ui}
=-\frac12F_{,ij}.
$$

The quadratic [Christoffel symbol](../../../../christoffel-symbol.md) terms vanish here: any potentially contributing intermediate $u$ index gives a factor $\Gamma^u{}_{ab}=0$, and the remaining possible products have a lower $v$ index and vanish. Since the [symmetric matrix](../../../../symmetric-matrix.md) $M$ gives $F_{,ij}=2M_{ij}$, lowering the first index gives

$$
\boxed{R_{uiuj}=R^v{}_{iuj}=-M_{ij}(u).}
$$

All remaining nonzero components follow from the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) symmetries

$$
R_{abcd}=-R_{bacd}=-R_{abdc}=R_{cdab}.
$$

There are no other independent components: terms involving a $v$ index vanish, while nonzero terms require one $u$ in each antisymmetric pair.

The [Ricci tensor](../../../../ricci-tensor.md) is consequently

$$
R_{uu}=\delta^{ij}R_{iuju}=-\operatorname{tr}M,\qquad
R_{ab}=0\quad\text{otherwise}.
$$

The [Ricci scalar](../../../../ricci-scalar.md) vanishes even when the [trace](../../../../matrix-trace.md) is nonzero, since $g^{uu}=0$. With zero [cosmological constant](../../../../cosmological-constant.md), the vacuum [Einstein field equations](../../../../einstein-field-equations-split.md) reduce to $R_{ab}=0$. Therefore the necessary and sufficient condition is

$$
\boxed{\operatorname{tr}M(u)=0\quad\text{for every }u.}
$$

This is the [Ricci tensor of a Brinkmann plane wave](../../../../ricci-tensor-of-a-brinkmann-plane-wave.md): a nonzero, trace-free profile can have nonzero [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) despite vanishing [Ricci tensor](../../../../ricci-tensor.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
