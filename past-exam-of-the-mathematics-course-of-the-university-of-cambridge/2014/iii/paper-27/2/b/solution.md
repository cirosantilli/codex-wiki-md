<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the radial [martingale](../../../../../../martingale-split.md) and its clock by

$$
H_t=\int_0^tX_s\,dX_s+Y_s\,dY_s,\qquad\boxed{A(t)=\int_0^t(X_s^2+Y_s^2)\,ds.}
$$

The [Itô formula](../../../../../../ito-s-lemma.md) gives $R_t^2=2H_t+2t$. Independence of the coordinate [Brownian motions](../../../../../../brownian-motion-split.md) makes their cross variation zero, so

$$
\langle H\rangle_t=A(t),\qquad\langle Z\rangle_t=A(t),\qquad\langle H,Z\rangle_t=\int_0^t(X_sY_s-Y_sX_s)\,ds=0.
$$

The last identity is [orthogonality of the radial martingale and planar Brownian area](../../../../../../orthogonality-of-the-radial-martingale-and-planar-brownian-area.md).

The clock is adapted and continuous, and it is strictly increasing almost surely. Otherwise the two coordinate paths would both vanish throughout a nontrivial interval. Such an interval contains a rational subinterval, while a Brownian increment over each fixed rational subinterval is a nondegenerate Gaussian and cannot be zero with positive probability.

Also $A(\infty)=\infty$ almost surely. If it were finite, the [finite-bracket convergence lemma](../../../../../../finite-bracket-convergence-lemma.md) would make $H_t$ converge to a finite limit. Then $R_t^2=2t+O(1)$ on that event, forcing $\int_0^\infty R_t^2\,dt=\infty$, a contradiction. Thus no finite-lifetime extension is needed here.

Use the same inverse clock $T_u=\inf\{t:A(t)>u\}$ for both [martingales](../../../../../../martingale-split.md), and set $W_u=H_{T_u}$, $B_u=Z_{T_u}$. Their bracket matrix is

$$
\begin{pmatrix}\langle W\rangle_u&\langle W,B\rangle_u\\\langle W,B\rangle_u&\langle B\rangle_u\end{pmatrix}
=\begin{pmatrix}u&0\\0&u\end{pmatrix}.
$$

The vector characterization proved in part (a) makes $(W,B)$ a two-dimensional [Brownian motion](../../../../../../brownian-motion-split.md); in particular its two coordinate processes are independent. Reversing the common clock gives

$$
\boxed{R_t^2=2W_{A(t)}+2t,\qquad Z_t=B_{A(t)},\qquad W\text{ and }B\text{ are independent}.}
$$

This is a [common-clock Brownian representation of radius and area](../../../../../../common-clock-brownian-representation-of-radius-and-area.md). Independence follows from the joint time change and identity bracket matrix; no independence of either [Brownian motion](../../../../../../brownian-motion-split.md) from $A$ is asserted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
