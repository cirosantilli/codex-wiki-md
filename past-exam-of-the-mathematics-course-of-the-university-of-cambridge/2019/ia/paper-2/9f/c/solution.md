<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Urn $i$ has $2^i$ balls, so a draw from it is white with probability $2^{-i}$. Given that the first ball is white, [Bayes' theorem](../../../../../../bayes-theorem.md) gives the [posterior probability](../../../../../../posterior-probability.md)

$$
\mathbb P(I=i\mid W)=\frac{2^{-i}}{\sum_{j=1}^n2^{-j}}.
$$

After replacement, the second draw is [conditionally independent](../../../../../../conditional-independence.md) of the first given the urn. Hence

$$
p(n)=\frac{\sum_{i=1}^n4^{-i}}{\sum_{i=1}^n2^{-i}}
=\frac{\frac13(1-4^{-n})}{1-2^{-n}}
=\frac13(1+2^{-n}).
$$

Consequently $\boxed{p(n)\to1/3}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
