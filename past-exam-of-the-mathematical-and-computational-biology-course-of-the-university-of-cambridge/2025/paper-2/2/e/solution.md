<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $Z_t$ be the hidden state. With the usual convention $\alpha_t(i)=P(o_1,\ldots,o_t,Z_t=i)$ and $\beta_t(i)=P(o_{t+1},\ldots,o_T\mid Z_t=i)$, the [Markov property](../../../../../markov-property.md) and the [conditional independence](../../../../../conditional-independence.md) of emissions factor the joint probability as

$$
\begin{aligned}
&P(O,Z_t=i,Z_{t+1}=j,Z_{t+2}=k)\\
&\qquad=\alpha_t(i)\,a_{ij}\,b_j(o_{t+1})\,a_{jk}\,b_k(o_{t+2})\,\beta_{t+2}(k).
\end{aligned}
$$

The requested state-path probability after observing the complete data is the corresponding [conditional probability](../../../../../conditional-probability.md):

$$
\boxed{P(Z_t=i,Z_{t+1}=j,Z_{t+2}=k\mid O)=\frac{\alpha_t(i)a_{ij}b_j(o_{t+1})a_{jk}b_k(o_{t+2})\beta_{t+2}(k)}{P(O)}}.
$$

Here the [forward algorithm](../../../../../forward-algorithm.md) and [backward algorithm](../../../../../backward-algorithm.md) give the same normalizer at any interior time,

$$
P(O)=\sum_r\alpha_t(r)\beta_t(r).
$$

There is no extra factor $b_i(o_t)$: it is already included in $\alpha_t(i)$. If an unconditioned joint probability with the observations is intended, it is the numerator alone. Summing the boxed expression over all $i,j,k$ gives one.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
