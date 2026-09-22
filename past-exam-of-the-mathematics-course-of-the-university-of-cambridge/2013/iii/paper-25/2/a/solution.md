<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $T\le s$, then $\phi(W_T)K$ is $\mathcal F_s$-measurable. Independence and centring of the future [Brownian increment](../../../../../../brownian-increment.md) make the desired left side zero; the time multiplier on the right is zero as well.

Suppose $T>s$. Conditional on $\mathcal F_s$, write $W_T=W_s+U$ and $W_t-W_s=V$. The pair $(U,V)$ is jointly normal and independent of $\mathcal F_s$, with

$$
\mathbb E V=0,\qquad\operatorname{Cov}(U,V)=\min(T-s,t-s)=T\wedge t-T\wedge s.
$$

Apply the supplied [Gaussian integration by parts](../../../../../../stein-s-lemma-probability.md) formula to $z\mapsto\phi(W_s+z)$, treating the known $W_s$ as its parameter. This gives

$$
\mathbb E[\phi(W_T)(W_t-W_s)\mid\mathcal F_s]=(T\wedge t-T\wedge s)\mathbb E[\phi'(W_T)\mid\mathcal F_s].
$$

Multiply by the bounded $\mathcal F_s$-measurable $K$ and use the defining property of [conditional expectation](../../../../../../conditional-expectation.md). Thus **the required expectation identity holds for every $s<t$, including intervals crossing or lying after $T$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
