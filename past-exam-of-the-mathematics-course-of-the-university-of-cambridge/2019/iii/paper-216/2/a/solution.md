<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Given the current state $x=(x_1,\ldots,x_d)$, a [Random-scan Gibbs sampler](../../../../../../random-scan-gibbs-sampler.md) chooses $I$ uniformly from $\{1,\ldots,d\}$, leaves $x_{-I}$ unchanged, and samples the new coordinate from the complete conditional distribution

$$
X_I'\sim\pi(dx_I\mid x_{-I}).
$$

Its transition kernel is

$$
K(x,dy)=\frac1d\sum_{i=1}^d
\pi(dy_i\mid x_{-i})\,\delta_{x_{-i}}(dy_{-i}),
$$

and it leaves $\pi$ invariant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
