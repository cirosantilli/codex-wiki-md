<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hoeffding lemma](../../../../../../hoeffding-lemma.md) states that if $a\leq X\leq b$ almost surely, then for every real $\lambda$,

$$
\log\mathbb E e^{\lambda(X-\mathbb EX)}
\leq\frac{\lambda^2(b-a)^2}{8}.
$$

Convexity of $e^{\lambda x}$ bounds it on $[a,b]$ by the secant joining its endpoint values. Taking expectations reduces the centered moment-generating function to that of a two-point variable on $\{a,b\}$ having the same mean. After rescaling to $[0,1]$, its logarithm is

$$
-\lambda q+\log(1-q+qe^\lambda),
$$

where $q$ is its mean. Twice differentiating in $\lambda$ shows that the second derivative is a Bernoulli variance and hence at most $1/4$. The value and first derivative vanish at zero, so Taylor's theorem gives at most $\lambda^2/8$. Rescaling proves the claim.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
