<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $A=\langle M\rangle$ be the [quadratic variation](../../../../../../quadratic-variation.md) and stop at $T_b=\inf\{u\geq0:A_u>b\}$. Its continuity and monotonicity imply $A_{u\wedge T_b}\leq b$ and $A_{T_b}=b$ whenever $T_b<\infty$. The standard [martingale](../../../../../../martingale-split.md) isometry after stopping by bounded [quadratic variation](../../../../../../quadratic-variation.md) gives $\mathbb E(M_{t\wedge T_b}^2)=\mathbb EA_{t\wedge T_b}\leq b$; in particular the stopped [local martingale](../../../../../../local-martingale.md) is [square-integrable](../../../../../../square-integrable-function.md). This criterion follows by localization and the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md), which bound the second [moment](../../../../../../moment.md) of the stopped supremum by $4b$ and then permit removal of localization.

On $\{A_t\leq b\}$ one has $T_b\geq t$, so the original and stopped paths agree through time $t$. Therefore the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) and the [Markov inequality](../../../../../../markov-inequality.md) give

$$
\begin{aligned}
\mathbb P\left(\sup_{s\leq t}M_s>a\right)
&\leq\mathbb P\left(\sup_{s\leq t}|M_{s\wedge T_b}|>a\right)+\mathbb P(A_t>b)\\
&\leq\frac{4b}{a^2}+\mathbb P(A_t>b).
\end{aligned}
$$

Thus

$$
\boxed{\mathbb P(\sup_{s\leq t}M_s>a)\leq4b/a^2+\mathbb P(\langle M\rangle_t>b).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
