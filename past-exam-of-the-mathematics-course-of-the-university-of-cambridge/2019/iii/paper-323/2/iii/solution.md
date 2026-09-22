<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $Z$ indicate whether the outcome differs from $x_1$. Then $\mathbb P(Z=1)=q$. The [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) gives

$$
H(X)=H(Z)+qH(X\mid Z=1),
$$

since $X=x_1$ is determined when $Z=0$. The remaining conditional distribution has at most $m-1$ outcomes, so the [maximum entropy on a finite alphabet](../../../../../../maximum-entropy-on-a-finite-alphabet.md) is $\log_2(m-1)$. Therefore the [Shannon source coding theorem](../../../../../../shannon-s-source-coding-theorem.md) limit obeys

$$
\boxed{H(X)\leq h_2(q)+q\log_2(m-1)}.
$$

Here $h_2$ is the [binary entropy function](../../../../../../binary-entropy-function.md); equality holds when the rare outcomes are equiprobable. A convenient explicit small-$q$ bound is

$$
\boxed{H(X)\leq q\log_2\frac{e(m-1)}q},
$$

because $-(1-q)\log_2(1-q)\leq q\log_2e$. For a fixed alphabet, this upper bound tends to zero as $q\to0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
