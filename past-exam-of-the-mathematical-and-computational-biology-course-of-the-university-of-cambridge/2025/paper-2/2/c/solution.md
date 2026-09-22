<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a uniform independent [DNA](../../../../../deoxyribonucleic-acid.md) background, so each [nucleotide](../../../../../nucleotide.md) has probability $1/4$. Conditional on length five, its sequence probability is $4^{-5}=1/1024$. The requested score, often called log-odds in sequence analysis, is a [log-likelihood ratio](../../../../../log-likelihood-ratio.md) against this background:

$$
\boxed{\log_2\frac{P(\texttt{CGTTA})}{4^{-5}}=\log_2\frac{27}{4}\approx2.75489\ \text{bits}}.
$$

Using [natural logarithms](../../../../../natural-logarithm.md) instead gives $\ln(27/4)\approx1.90954$. Identically distributed independent positions do not, by themselves, require equal base frequencies. If the intended background instead has specified frequencies $q_A,q_T,q_G,q_C$, the general answer is

$$
\log\frac{27/4096}{q_Cq_Gq_T^2q_A}.
$$

The numerical value above uses the conventional equal-frequency random [DNA](../../../../../deoxyribonucleic-acid.md) model.

Taking a [logarithm](../../../../../logarithm.md) only after multiplying probabilities does not prevent [floating-point underflow](../../../../../floating-point-underflow.md): the product may already have rounded to zero, and its [logarithm](../../../../../logarithm.md) is then $-\infty$. **Accumulate logarithms before forming tiny products**; where alternative paths must be added, use [log-sum-exp](../../../../../log-sum-exp-function.md) in the [forward algorithm](../../../../../forward-algorithm.md) or rescale its intermediate probabilities.

## ↑ Ancestors (13)

1. [C](../c.md)
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
