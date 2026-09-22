<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) on the integers, starting at zero. It is recurrent: it returns to zero infinitely often [almost surely](../../../../../../almost-sure-convergence.md), and in fact visits every integer infinitely often. To see the two-sided unboundedness explicitly, [gambler's ruin](../../../../../../gambler-s-ruin.md) gives, for positive integers $a,b$,

$$
\mathbb P_0(T_b<T_{-a})=\frac{a}{a+b}.
$$

Letting $a\to\infty$ shows that $b$ is hit with probability one; the analogous argument hits every negative integer. From any state the same argument gives return to zero with probability one. Repeated use of the [Strong Markov property](../../../../../../strong-markov-property.md) then gives infinitely many returns and visits. Therefore

$$
\boxed{\limsup_{n\to\infty}X_n=+\infty,\qquad
\liminf_{n\to\infty}X_n=-\infty\quad\text{almost surely}.}
$$

In particular $X_n$ has no limit [almost surely](../../../../../../almost-sure-convergence.md), and $|X_n|$ does not tend to infinity because of the returns to zero. In contrast, the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $X_n/n\to0$ [almost surely](../../../../../../almost-sure-convergence.md), while the [central limit theorem](../../../../../../central-limit-theorem.md) gives $X_n/\sqrt n\xrightarrow dN(0,1)$. These distinguish oscillation of the path from scaling limits of its [probability distribution](../../../../../../probability-distribution.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
