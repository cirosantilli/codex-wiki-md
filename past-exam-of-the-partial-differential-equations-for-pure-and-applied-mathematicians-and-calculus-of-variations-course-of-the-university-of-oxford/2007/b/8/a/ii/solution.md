<h1 id="b/8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [De la Vallée-Poussin criterion](../../../../../../de-la-vallee-poussin-criterion.md) characterizes [uniform integrability](../../../../../../uniform-integrability.md) by existence of a nonnegative increasing [convex function](../../../../../../convex-function.md) $\Psi$ with $\Psi(s)/s\to\infty$ and a uniform bound on $\int\Psi(|v_j|)$. On a finite interval this gives a [weakly convergent](../../../../../../weak-convergence.md) [subsequence](../../../../../../subsequence.md) in $L^1$ by the [Dunford-Pettis theorem](../../../../../../dunford-pettis-theorem.md).

After discarding a finite prefix of the [minimizing sequence](../../../../../../minimizing-sequence.md) if needed, put $H(t)=\Phi(t)-M\geq0$. Its derivative [sequence](../../../../../../sequence.md) has $\int H(u_j')\leq C$. The superlinear bound directly gives [uniform integrability](../../../../../../uniform-integrability.md): for $H(t)\geq A|t|$ outside $[-R_A,R_A]$,

$$
\int_E|u_j'|\leq R_A|E|+C/A.
$$

If the convex version of the criterion is used, choose increasing $R_m\to\infty$ so $H(t)\geq m^2|t|$ for $|t|\geq R_m$, and set $\Psi(s)=\sum_{m\geq1}(s-R_m)_+$. This is locally a finite sum, convex and increasing. It is superlinear because for fixed $N$ and $s\geq2R_N$, $\Psi(s)\geq Ns/2$. If exactly $m$ terms are active, $\Psi(s)\leq ms\leq H(t)$ for $s=|t|$, so its integrals have the same bound. The criterion therefore supplies $u_{j_k}'\rightharpoonup v$ in $L^1$.

Define $u(x)=\alpha+\int_a^xv$. Interval-indicator tests give $u_{j_k}(x)\to u(x)$ for every $x$, including $b$, so its endpoint values are correct and $u\in W^{1,1}$. The common derivative $L^1$ bound makes these [functions](../../../../../../function-split.md) uniformly bounded. [Uniform integrability](../../../../../../uniform-integrability.md) also gives common equicontinuity, since an increment is bounded by the derivative integral on the intervening interval. The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) yields uniform convergence to the same identified limit, and in particular

$$
\boxed{u\in\mathcal A,\quad u_{j_k}'\rightharpoonup u'\text{ in }L^1,\quad u_{j_k}\to u\text{ in }L^1.}
$$

Here the printed admissible space is $W^{1,1}$, so this [compactness](../../../../../../compact-space.md) argument gives precisely the needed membership.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [B](../../../../b.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
