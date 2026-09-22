<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For every decision with finite worst-case value, the previous dual represents that value as a maximum over $\alpha,\beta$. Maximizing it jointly with $x$ yields the [robust linear optimization over the probability simplex](../../../../../../../robust-linear-optimization-over-the-probability-simplex.md) formulation:

$$
\boxed{\begin{aligned}
\max_{x,\alpha,\beta}\quad&r_0^Tx-\mathbf1^T(\alpha+\beta),\\
\text{subject to}\quad&x\ge0,\quad\mathbf1^Tx=1,\\
&\alpha,\beta\ge0,\quad P^T(\alpha-\beta)=x.
\end{aligned}}
$$

Indeed every feasible triple gives a dual lower bound on that decision's worst-case revenue, while dual attainment supplies a triple reaching it. This argument only combines two maximizations after dualization; it does not interchange the original max and min.

If the [probability simplex](../../../../../../../probability-simplex.md) intersects $\operatorname{range}P^T$, this linear program is feasible and bounded above by $\max_i(r_0)_i$, and hence attains an optimum. Its maximizing $x$ is a robust optimizer. If the intersection is empty, every decision has worst-case value $-\infty$ and the linear program is infeasible, consistently with the extended-value convention. Full column rank of $P$ ensures every simplex decision has a finite inner optimum, but is not needed for the qualified equivalence.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
