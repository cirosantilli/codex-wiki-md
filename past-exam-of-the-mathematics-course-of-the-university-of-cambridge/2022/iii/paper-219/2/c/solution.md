<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set

$$
a=e^{-(t_2-t_1)/\tau},
\qquad
b=e^{-(t_3-t_2)/\tau}.
$$

The [Markov factorization](../../../../../../markov-factorization.md) and the conditional normal laws from part b give the fully univariate product

$$
p(y\mid t,\mu,\tau)
=\phi(y_1;\mu,1)
\phi\!\left(y_2;\mu+a(y_1-\mu),1-a^2\right)
\phi\!\left(y_3;\mu+b(y_2-\mu),1-b^2\right),
$$

where $\phi(\mathord\cdot;m,v)$ denotes the $N(m,v)$ density. This is a [weighted least squares](../../../../../../weighted-least-squares.md) problem in $\mu$. Differentiating its log-likelihood gives

$$
\widehat\mu=
\frac{
y_1+\dfrac{y_2-ay_1}{1+a}+\dfrac{y_3-by_2}{1+b}
}{
1+\dfrac{1-a}{1+a}+\dfrac{1-b}{1+b}
}.
$$

Every innovation in the numerator has expectation equal to its coefficient in the denominator times $\mu$. Therefore $\mathbb E\widehat\mu=\mu$, so this maximum likelihood estimator is unbiased.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
