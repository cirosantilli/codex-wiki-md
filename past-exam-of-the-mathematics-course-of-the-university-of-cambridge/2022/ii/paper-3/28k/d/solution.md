<h1 id="28k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The given identities imply

$$
\frac1n\sum_{i=1}^n
\left(\overline X_{n-1,i}^2-\overline X_n^2\right)
=\frac1{n(n-1)^2}
\sum_{i=1}^n(X_i-\overline X_n)^2.
$$

Thus, writing

$$
s_n^2=\frac1{n-1}\sum_{i=1}^n(X_i-\overline X_n)^2,
$$

we have the exact identity

$$
\widetilde T_{\rm JACK}
=T_n-\frac{s_n^2}{n}.
$$

The [sample variance](../../../../../../sample-variance.md) satisfies $s_n^2\xrightarrow{P}1$, so

$$
\sqrt n(\widetilde T_{\rm JACK}-T_n)
=-\frac{s_n^2}{\sqrt n}\xrightarrow{P}0.
$$

The [Slutsky theorem](../../../../../../slutsky-theorem.md) and part (c) now give

$$
\boxed{
\sqrt n(\widetilde T_{\rm JACK}-\mu^2)
\xrightarrow{d}N(0,4\mu^2)
}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
