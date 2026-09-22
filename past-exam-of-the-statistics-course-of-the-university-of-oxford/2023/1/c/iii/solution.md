<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The derivative of the log ratio is $\tfrac12(n/q-1)$, so $\lambda(q)$ increases from zero to one on $(0,n)$ and decreases to zero on $(n,\infty)$. Rejecting for a sufficiently small ratio therefore gives two tails with $0<q_1<n<q_2$.

Under $H_0$, [Cochran's theorem](../../../../../cochran-s-theorem.md) gives the exact [sampling distribution](../../../../../sampling-distribution.md) $Q=S/\sigma_0^2\sim\chi_{n-1}^2$, independently of the unknown mean. Writing $F_{n-1}$ for its [cumulative distribution function](../../../../../cumulative-distribution-function.md), the two cutoffs are determined by

$$
\boxed{F_{n-1}(q_1)+1-F_{n-1}(q_2)=\alpha,\qquad n\log(q_2/q_1)=q_2-q_1}.
$$

The first equation calibrates the exact [size of a statistical test](../../../../../size-of-a-statistical-test.md). The second is $\lambda(q_1)=\lambda(q_2)$, so both tails belong to one [likelihood ratio](../../../../../likelihood-ratio.md) cutoff. Hence the exact [critical region](../../../../../rejection-region.md) is $\boxed{\{q\leq q_1\}\cup\{q\geq q_2\}}$. Its two tail probabilities are not generally equal: equal-tailed chi-squared cutoffs give a different test.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
