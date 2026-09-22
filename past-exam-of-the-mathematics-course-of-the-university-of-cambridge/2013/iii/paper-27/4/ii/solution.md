<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take increasing to mean strict growth on every nonempty time interval; otherwise a constant family has no uniquely determined driving point. The [half-plane-capacity parameterization](../../../../../../half-plane-capacity-parameterization.md) imposed below guarantees strict growth. For $s<t$, define the increment hull in the mapped domain by

$$
K_{s,t}=\mathbb H\setminus g_s(\mathbb H\setminus K_t).
$$

This definition includes filling and boundary conventions automatically. Its [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) is $g_{s,t}=g_t\circ g_s^{-1}$. The [Loewner local growth property](../../../../../../loewner-local-growth-property.md) means

$$
\boxed{\sup_{0\le t\le T}\operatorname{rad}(K_{t,t+h})
\longrightarrow0\quad(h\downarrow0)}
$$

for every finite $T$ within the parameter range. Equivalently, the mapped increments have uniformly vanishing diameter on compact time intervals.

For fixed $t$, the nonempty compact Euclidean closures $\overline K_{t,t+h}$ are nested as $h$ decreases. Their diameters tend to zero, so their intersection is a singleton. Its point lies on the real axis: the imaginary part of any point in a hull is at most its enclosing radius. Define the [Loewner transform](../../../../../../loewner-driving-function.md) by

$$
\boxed{\{\xi_t\}=\bigcap_{h>0}\overline K_{t,t+h}.}
$$

Since $\xi_t$ lies in each closure, every point of $K_{t,t+h}$ is at distance at most $2\operatorname{rad}(K_{t,t+h})$ from it.

To prove continuity, choose $z\in K_{t+2h}\setminus K_{t+h}$ and write $w=g_t(z)$, $w'=g_{t+h}(z)$. Then $w\in K_{t,t+2h}$, $w'\in K_{t+h,t+2h}$ and $w'=g_{t,t+h}(w)$. The continuity estimate from part (i) gives

$$
\begin{aligned}
|\xi_{t+h}-\xi_t|
&\le|\xi_t-w|+|w-w'|+|w'-\xi_{t+h}|\\
&\le2\operatorname{rad}(K_{t,t+2h})
+3\operatorname{rad}(K_{t,t+h})
+2\operatorname{rad}(K_{t+h,t+2h}).
\end{aligned}
$$

The right-hand side tends to zero uniformly on compact time intervals. Applying the same inequality with the earlier time as the base proves left continuity as well. Thus **the Loewner transform is continuous**.

Now impose $\operatorname{hcap}(K_t)=2t$. The [half-plane-capacity composition rule](../../../../../../half-plane-capacity-composition-rule.md) follows by composing Laurent expansions at infinity and gives

$$
\operatorname{hcap}(K_{s,t})=2(t-s).
$$

For a point not yet swallowed, put $z_s=g_s(z)$ and $r_{s,t}=2\operatorname{rad}(K_{s,t})$. The increment is contained in the half-disc of radius $r_{s,t}$ centred at $\xi_s$. The continuity estimate first proves continuity of $s\mapsto g_s(z)$: its increment is bounded by $3\operatorname{rad}(K_{s,t})$. The [differentiability estimate for a mapping-out function](../../../../../../differentiability-estimate-for-a-mapping-out-function.md) then gives, when $t-s$ is small enough,

$$
g_t(z)-g_s(z)
=\frac{2(t-s)}{g_s(z)-\xi_s}
+O\!\left(\frac{r_{s,t}(t-s)}{|g_s(z)-\xi_s|^2}\right).
$$

On a compact interval before swallowing the denominator stays away from zero. Divide by $t-s$ and let $t\downarrow s$. The local-growth property makes the error tend to zero. The analogous backward quotient has the same limit, using continuity of $g_s(z)$ and $\xi_s$. Thus the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) follows:

$$
\boxed{\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},\qquad g_0(z)=z.}
$$

The initial value follows from $\operatorname{hcap}(K_0)=0$, hence $K_0=\varnothing$. Without the capacity parameterization, the same argument gives $dg_t(z)=d\,\operatorname{hcap}(K_t)/(g_t(z)-\xi_t)$, interpreted with the capacity clock.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
