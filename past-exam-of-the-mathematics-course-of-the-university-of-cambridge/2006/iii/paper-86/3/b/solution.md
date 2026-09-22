<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $q$ is [harmonic](../../../../../../harmonic-function.md), $q_z$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) and the [one-form](../../../../../../one-form.md) $e^{-ikz}q_z\,dz$ is closed. Closing the physical quadrant at infinity gives the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md)

$$
\widehat q_1(k)+\widehat q_2(k)=0\qquad
(\operatorname{Re}k<0,\ \operatorname{Im}k<0).
$$

In this third spectral quadrant the exponential decays on both boundary axes. Set $\gamma=\beta_1+\beta_2$. The relation becomes

$$
H_1(k)-iJ_1(k)=e^{i\gamma}[H_2(k)-iJ_2(k)].
$$

All four boundary [functions](../../../../../../function-split.md) are real. Consequently their transforms obey

$$
\overline{H_1(\bar k)}=H_1(k),\qquad
\overline{H_2(-\bar k)}=H_2(k),
$$

and the same identities for $J_1,J_2$. [Complex conjugation](../../../../../../complex-conjugation.md) of the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) therefore gives its upper-left consequence

$$
H_1(k)+iJ_1(k)=e^{-i\gamma}[H_2(-k)+iJ_2(-k)]
\qquad(\operatorname{Re}k<0,\ \operatorname{Im}k>0).
$$

Introduce just one unknown [function](../../../../../../function-split.md),

$$
\boxed{\Phi(k)=H_2(-k)-iJ_2(-k)
=\int_0^\infty e^{ikx}[h_2(x)-ij_2(x)]\,dx,\qquad\operatorname{Im}k>0.}
$$

It is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) in the [upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). Under the transform-admissible decay assumptions, $|\Phi(k)|\leq\int_0^\infty(|h_2|+|j_2|)\,dx$, so it is bounded there.

For $k$ on the positive real ray, use both consequences of the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) at $-k$. Adding them removes $J_1(-k)$ and gives

$$
H_2(k)+iJ_2(k)=2e^{i\gamma}H_1(-k)-e^{2i\gamma}\Phi(k).
$$

For $k$ on the positive imaginary ray, use the upper-left relation and $H_2(-k)+iJ_2(-k)=2H_2(-k)-\Phi(k)$. The resulting [single-function spectral elimination for a rational-angle quadrant](../../../../../../single-function-spectral-elimination-for-a-rational-angle-quadrant.md) is

$$
\boxed{\begin{aligned}
\widehat q_2(k)&=-e^{i\beta_2}[H_2(k)-e^{i\gamma}H_1(-k)]
-\frac{e^{i\beta_2+2i\gamma}}2\Phi(k),\qquad k>0,\\
\widehat q_1(k)&=e^{-i\beta_1}[H_1(k)-e^{-i\gamma}H_2(-k)]
+\frac{e^{-i\beta_1-i\gamma}}2\Phi(k),\qquad k\in i\mathbb R_+.
\end{aligned}}
$$

Boundary limits from the appropriate transform domains are understood. Every remaining unknown boundary [derivative](../../../../../../derivative.md) is contained in the one bounded upper-half-plane [function](../../../../../../function-split.md) $\Phi$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
