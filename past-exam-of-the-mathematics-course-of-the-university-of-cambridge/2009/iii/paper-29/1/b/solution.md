<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the representation from part (a), and put $\Delta_jM=M_{T_{j+1}}-M_{T_j}$, $U_j=h_j\Delta_jM$ and $N=H\cdot M$. The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) in the form needed here says that for a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md) $L$ and [stopping times](../../../../../../stopping-time.md) $\sigma\leq\tau$, including terminal infinite times, $\mathbb E[L_\tau\mid\mathcal F_\sigma]=L_\sigma$. An [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md) is [uniformly integrable](../../../../../../uniform-integrability.md) and has the required terminal value.

Consequently $\mathbb E[\Delta_jM\mid\mathcal F_{T_j}]=0$. Conditioning on $\mathcal F_t$ and distinguishing whether $T_j\leq t$ gives

$$
\mathbb E[U_j\mid\mathcal F_t]=h_j\bigl(M_{t\wedge T_{j+1}}-M_{t\wedge T_j}\bigr).
$$

Thus $N_t=\mathbb E[\sum_jU_j\mid\mathcal F_t]$ is a [martingale](../../../../../../martingale-split.md). Its paths are continuous, since each stopped increment is continuous and zero until its left endpoint.

For $i<j$, $U_i$ is $\mathcal F_{T_j}$-measurable, so the same conditional identity yields $\mathbb E(U_iU_j)=0$. These [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md) relations also hold for the unweighted increments. Therefore

$$
\begin{aligned}
\mathbb E N_\infty^2&=\sum_j\mathbb E\bigl(h_j^2(\Delta_jM)^2\bigr)\\
&\leq\|H\|_\infty^2\sum_j\mathbb E(\Delta_jM)^2
=\|H\|_\infty^2\mathbb E(M_\infty-M_0)^2.
\end{aligned}
$$

Here $N_\infty=\sum_jU_j\in L^2$. By conditional Jensen, $\mathbb E N_t^2\leq\mathbb E N_\infty^2$ for every $t$, so

$$
\boxed{H\cdot M\in\mathcal M_c^2,\qquad\mathbb E(H\cdot M)_\infty^2\leq\|H\|_\infty^2\mathbb E(M_\infty-M_0)^2.}
$$

This proves the norm bound without presupposing the [Itô isometry](../../../../../../ito-isometry.md) requested next.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
