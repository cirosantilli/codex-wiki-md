<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each leave-one-out statistic has the same distribution as $T_{n-1}$, so

$$
\mathbb E\widehat B_n
=(n-1)(B_{n-1}(\theta)-B_n(\theta)).
$$

Consequently the bias of the [jackknife bias correction](../../../../../../jackknife-bias-correction.md) is

$$
\mathbb E\widetilde T_{\rm JACK}-\theta
=nB_n-(n-1)B_{n-1}.
$$

The assumed expansion gives

$$
nB_n=a+\frac bn+O(n^{-2})
$$

and

$$
(n-1)B_{n-1}
=a+\frac b{n-1}+O(n^{-2})
=a+\frac bn+O(n^{-2}).
$$

Their difference is therefore $O(n^{-2})$, as required.

## ↑ Ancestors (11)

1. [A](../a.md)
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
