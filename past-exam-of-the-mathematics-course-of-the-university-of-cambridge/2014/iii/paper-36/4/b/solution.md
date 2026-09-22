<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each proposal $X\sim g$, independently draw $U\sim\operatorname{Unif}(0,1)$ and accept it when

$$
\boxed{U\leq\frac{f(X)}{Mg(X)}.}
$$

The ratio is at most one, as required. For any measurable set $A$,

$$
\mathbb P(X\in A,\text{accept})=\frac1M\int_Af(x)\,dx,
$$

so the acceptance probability is $p=1/M$ and the conditional distribution of an accepted proposal has density $f$. Repeating independent trials until acceptance therefore gives an exact draw from $f$, and repeating the whole procedure gives iid target draws. This proves [rejection sampling](../../../../../../rejection-sampling.md).

The number of proposals for one successful draw is geometric with mean $M$. Thus $M$ is also the expected proposal cost of this exact simulation method.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
