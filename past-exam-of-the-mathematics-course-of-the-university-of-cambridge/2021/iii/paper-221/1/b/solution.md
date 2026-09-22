<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the second [causal directed acyclic graph](../../../../../../causal-directed-acyclic-graph.md), $Y(a_1,a_2)$ depends on $U_2$ but not on $U_1$, whereas $A_1$ depends on $U_1$ and the two latent roots are independent. Hence

$$
Y(a_1,a_2)\mathrel\perp A_1.
$$

Although conditioning on $X$ conveys information about $U_2$, the assignment $A_2$ uses only $(A_1,X)$ and fresh randomization, so

$$
Y(a_1,a_2)\mathrel\perp A_2\mid A_1,X.
$$

These are the two [sequential exchangeability](../../../../../../sequential-exchangeability.md) conditions. Using them successively, together with [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md), gives

$$
\begin{aligned}
\mathbb E[Y(a_1,a_2)]
&=\sum_x\mathbb E[Y(a_1,a_2)\mid A_1=a_1,X=x]
\mathbb P(X=x\mid A_1=a_1)\\
&=\sum_x\mathbb E[Y\mid A_1=a_1,X=x,A_2=a_2]
\mathbb P(X=x\mid A_1=a_1),
\end{aligned}
$$

which is the formula from part a.

Adding $X\to Y$ invalidates the argument in general. The latent variable $U_1$ confounds $A_1$ and $X$, so $\mathbb P(X\mid A_1=a_1)$ need not equal the distribution of $X(a_1)$. When $X$ directly affects $Y$, that discrepancy no longer cancels after summing over $x$. The same observed distribution can then correspond to different intervention means, so the displayed formula need not identify the effect.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
