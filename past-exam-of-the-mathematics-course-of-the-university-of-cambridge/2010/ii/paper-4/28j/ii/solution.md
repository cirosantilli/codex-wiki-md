<h1 id="28j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The adjoint equation is $\dot p=-rp$, so $p(t)=p_0e^{-rt}$. For the interior stationary candidate from part (i), writing $s=\beta c/\alpha$ gives $p\propto c^{\alpha+\beta-1}$. Therefore it formally has

$$
c(t)\propto e^{-rt/(\alpha+\beta-1)},
$$

which derives the printed formula as a stationary, generally nonoptimal candidate.

For the [work-then-consume optimum for a nonconcave consumption-leisure utility](../../../../../../work-then-consume-optimum-for-a-nonconcave-consumption-leisure-utility.md), the endpoint maximization in part (i) gives

$$
\ell(t)=0,\qquad c(t)=\left(\frac{\alpha}{p(t)}\right)^{1/(1-\alpha)}
=C e^{rt/(1-\alpha)}
$$

whenever consumption is chosen, and $\ell=1,c=0$ otherwise. Compare the two endpoint values: leisure and consumption are preferred when

$$
(1-\alpha)c^\alpha\ge p=\alpha c^{\alpha-1},
\quad\text{equivalently}\quad c\ge c_*:=\frac{\alpha}{1-\alpha}.
$$

Because the unconstrained consumption is increasing in time, there is at most one switch: **work first, then cease work and consume at an increasing rate**.

Here is a global verification, not just a [Pontryagin maximum principle](../../../../../../pontryagin-maximum-principle.md) condition. The terminal constraint is equivalent to

$$
\int_0^Te^{-rt}(c+s-1)\,dt\le x_0.
$$

For any $p_0>0$, pointwise maximization of $c^\alpha s^\beta-p_0e^{-rt}(c+s-1)$ gives an upper bound on every feasible objective, after adding $p_0x_0$. A control attaining this pointwise maximum and using the full budget attains the bound, so it is globally optimal.

Let $a=r\alpha/(1-\alpha)$. If

$$
C_0:=\frac{x_0}{(e^{aT}-1)/a}\ge c_*,
$$

the optimal switch time is $t_*=0$ and $C=C_0$. Otherwise choose the unique $t_*\in(0,T)$ such that

$$
C=c_*e^{-rt_* /(1-\alpha)},\qquad
C\frac{e^{aT}-e^{at_*}}a=x_0+\frac{1-e^{-rt_*}}r.
$$

The left side of the second equality after substitution decreases strictly from $c_*(e^{aT}-1)/a$ to zero, while the right side increases from $x_0$ to a positive number. Thus the switch exists and is unique. The control is $(\ell,c)=(1,0)$ before $t_*$ and $(0,Ce^{rt/(1-\alpha)})$ after it. It saturates the budget and attains the dual upper bound, completing the proof of optimality for the actual printed parameter range.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
