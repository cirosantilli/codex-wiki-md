<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $N_j(A)$ be the number of particles of gas $j$ in a bounded [Lebesgue measurable set](../../../../../../lebesgue-measurable-set.md) $A$. Because Lebesgue measure is diffuse, two independent spatial [Poisson point processes](../../../../../../poisson-point-process.md) have no common particle almost surely. Hence the mixture count is

$$
N(A)=N_1(A)+N_2(A).
$$

Writing $\lambda_j=z_j|A|$, independence gives the [probability generating function](../../../../../../probability-generating-function.md)

$$
\begin{aligned}
\mathbb E[s^{N(A)}]
&=\mathbb E[s^{N_1(A)}]\mathbb E[s^{N_2(A)}]\\
&=\exp(\lambda_1(s-1))\exp(\lambda_2(s-1))\\
&=\exp\bigl((z_1+z_2)|A|(s-1)\bigr).
\end{aligned}
$$

Thus

$$
N(A)\sim\operatorname{Pois}\bigl((z_1+z_2)|A|\bigr).
$$

If $A_1,\ldots,A_m$ are pairwise disjoint, the family

$$
\{N_j(A_r):j=1,2,\ 1\leq r\leq m\}
$$

is independent: counts in disjoint sets are independent within each gas, and the two gases are independent. Therefore the sums $N(A_r)$ are independent. These two facts prove directly that the mixture is a Poisson point process. By the [Superposition theorem for Poisson point processes](../../../../../../superposition-theorem-for-poisson-point-processes.md), its activity is

$$
\boxed{z_1+z_2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
