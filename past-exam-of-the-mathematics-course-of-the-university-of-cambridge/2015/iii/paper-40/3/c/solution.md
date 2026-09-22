<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the conditional second-moment matrix $V_t=\mathbb E[P_tP_t^\top\mid\mathcal F_{t-1}]$ from the PDF. By part (b), the filtration is finite-state at every finite time. On a time-$(t-1)$ atom let $p_1,\ldots,p_m$ be the successor price vectors and $q_1,\ldots,q_m>0$ their conditional probabilities. Then $m\leq n$ and

$$
V=\sum_{i=1}^m q_i p_i p_i^\top.
$$

Positive definiteness gives rank $n$, so $m\geq n$. Hence $m=n$, and the $n$ successor vectors have [linear independence](../../../../../../linear-independence.md).

We use the finite-horizon [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md) in deflator form: an arbitrage-free finite market admits a strictly positive adapted process $D$, with $D_0=1$, such that $DP$ is a [martingale](../../../../../../martingale-split.md). Equivalently, on every step,

$$
\mathbb E[D_tP_t\mid\mathcal F_{t-1}]=D_{t-1}P_{t-1}.
$$

Fix a finite horizon containing the step in question. On the parent atom, write $d_i=D_t/D_{t-1}>0$ on successor $i$ and $p_0=P_{t-1}$. Then

$$
\sum_iq_i d_i p_i=p_0.
$$

The proposed values $z_i=p_i^\top V^{-1}p_0$ satisfy precisely the same equation:

$$
\sum_iq_i z_i p_i
=\left(\sum_iq_i p_i p_i^\top\right)V^{-1}p_0=p_0.
$$

Because the $p_i$ have [linear independence](../../../../../../linear-independence.md) and the $q_i$ are positive, this linear system has a unique solution. Thus $z_i=d_i>0$, proving

$$
\boxed{Z_t>0\quad\text{almost surely for every }t\geq1.}
$$

This is the [positive regression deflator in a complete finite market](../../../../../../positive-regression-deflator-in-a-complete-finite-market.md). It also proves the suggested conclusion: with $Y_0=1$ and $Y_t=\prod_{u=1}^tZ_u$,

$$
\mathbb E[Y_tP_t\mid\mathcal F_{t-1}]
=Y_{t-1}\mathbb E[P_tP_t^\top\mid\mathcal F_{t-1}]V_t^{-1}P_{t-1}
=Y_{t-1}P_{t-1}.
$$

Hence $Y$ is a strictly positive [martingale deflator](../../../../../../martingale-deflator.md). Finite-state structure makes these expectations integrable on each finite horizon. Positive definiteness alone would not ensure positivity of the regression factor; [market completeness](../../../../../../complete-market.md) and the positive deflator are essential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
