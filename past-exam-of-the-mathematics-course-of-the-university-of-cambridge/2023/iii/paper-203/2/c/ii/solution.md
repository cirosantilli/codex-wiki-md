<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

It is enough by [Scaling invariance of SLE](../../../../../../../scaling-invariance-of-sle.md) and reflection in the imaginary axis to treat $x=1$. Take $r=1+\epsilon$. The drift

$$
b(z)=\frac{\kappa-4}{2}-\frac2{1+e^z}
$$

tends to $(\kappa-8)/2<0$ as $z\to-\infty$. Choose $L<0$ and $a<0$ such that $b(z)\leq a$ for $z\leq L$. Before $\widetilde Z$ reaches $L$,

$$
\widetilde Z_t
\leq\log\epsilon+\sqrt\kappa W_t+at.
$$

The [infinite-horizon crossing probability for Brownian motion with negative drift](../../../../../../../infinite-horizon-crossing-probability-for-brownian-motion-with-negative-drift.md) shows that this process has a finite running maximum almost surely, so

$$
\mathbb P_{\log\epsilon}(T_L<\infty)\longrightarrow0
\qquad(\epsilon\downarrow0).
$$

Order preservation for the [Loewner flow](../../../../../../../loewner-chain.md) gives $\tau_1\leq\tau_{1+\epsilon}$. On $\{\tau_1<\tau_{1+\epsilon}\}$, one has $V_t^1\to0$ while $V_t^{1+\epsilon}$ remains positive, so $\widetilde Z_t\to+\infty$ and in particular $T_L<\infty$. Hence

$$
\mathbb P(\tau_1<\tau_{1+\epsilon})\longrightarrow0,
\qquad
\mathbb P(\tau_1=\tau_{1+\epsilon})\longrightarrow1.
$$

If the trace itself hit the fixed boundary point $1$, then $1$ would be the right endpoint of the swallowed interval and $\tau_1<\tau_{1+\epsilon}$ for every $\epsilon>0$. Its probability is therefore zero. Scaling and reflection prove that [SLE does not hit a fixed nonzero boundary point](../../../../../../../sle-does-not-hit-a-fixed-nonzero-boundary-point.md) for every $x\in\mathbb R\setminus\{0\}$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
