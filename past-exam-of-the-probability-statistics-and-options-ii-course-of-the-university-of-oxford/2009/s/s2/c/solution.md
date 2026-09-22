<h1 id="s/s2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each $N_i$ is geometric on $\{1,2,\ldots\}$ with success probability $a=Z_p/(MZ_q)$. Hence

$$
\boxed{\mathbb E[N_i]=\frac{MZ_q}{Z_p},\qquad\widehat{Z_q/Z_p}=\frac1{MN}\sum_{i=1}^Nn_i.}
$$

Linearity of [expectation](../../../../../expected-value-split.md) proves the estimator is unbiased. Moreover the joint probability factors:

$$
P(N_i=k,X_i=x)=(1-a)^{k-1}\frac{\tilde p(x)}{MZ_q}=[(1-a)^{k-1}a]p(x).
$$

Thus $\boxed{N_i\text{ and }X_i\text{ are independent}}$, not merely uncorrelated. Fresh [independent](../../../../../independent-random-variables.md) trials make the simulated cycles [independent](../../../../../independent-random-variables.md) as well.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
