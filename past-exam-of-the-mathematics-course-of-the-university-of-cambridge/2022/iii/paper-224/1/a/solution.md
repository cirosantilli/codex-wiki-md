<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Stein's lemma](../../../../../../stein-s-lemma-information-theory.md) states that for distinct probability mass functions $P,Q$ on a finite alphabet, the best exponential decay rate of the [Type II error](../../../../../../type-i-and-type-ii-errors.md) $\beta_n=Q^{\otimes n}(B_n)$ among tests whose [Type I error](../../../../../../type-i-and-type-ii-errors.md) $\alpha_n=P^{\otimes n}(B_n^c)$ is eventually at most any fixed $\epsilon\in(0,1)$ is

$$
\lim_{n\to\infty}-\frac1n\log_2\beta_n=D(P\Vert Q).
$$

For the direct part, define the information-density typical region

$$
B_n=\left\{x_1^n:
\frac1n\log_2\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\geq D(P\Vert Q)-\delta
\right\}.
$$

The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) under $P$ gives $\alpha_n\to0$, while

$$
\begin{aligned}
\beta_n
&=\sum_{x_1^n\in B_n}Q^{\otimes n}(x_1^n)\\
&\leq2^{-n\{D(P\Vert Q)-\delta\}}
\sum_{x_1^n\in B_n}P^{\otimes n}(x_1^n)\\
&\leq2^{-n\{D(P\Vert Q)-\delta\}}.
\end{aligned}
$$

For the converse, let

$$
C_n=\left\{x_1^n:
\frac1n\log_2\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\leq D(P\Vert Q)+\delta
\right\}.
$$

Again $P^{\otimes n}(C_n)\to1$. Any test with $P^{\otimes n}(B_n)\geq1-\epsilon$ satisfies

$$
P^{\otimes n}(B_n\cap C_n)\geq1-\epsilon-o(1).
$$

On $C_n$, $Q^{\otimes n}\geq2^{-n(D+\delta)}P^{\otimes n}$, hence

$$
\beta_n\geq2^{-n(D+\delta)}\{1-\epsilon-o(1)\}.
$$

**Thus $\limsup_n-n^{-1}\log_2\beta_n\leq D+\delta$. Letting $\delta\downarrow0$ proves optimality.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
