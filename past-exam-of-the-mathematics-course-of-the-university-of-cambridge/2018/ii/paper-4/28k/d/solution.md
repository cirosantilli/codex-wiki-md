<h1 id="28k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Substituting part (b) gives

$$
\widehat g_N-g'(x_0)
=\frac{h}{2N}\sum_{i=1}^NZ_i g''(\xi_i)
+\frac1{Nh}\sum_{i=1}^NZ_i\varepsilon_i
=A+B.
$$

The curvature bound gives $|A|\leq hM/2$. Conditional on the $Z_i$ and the evaluation points, $B$ has mean zero, so the cross term has expectation zero. Independence of the [normal random variables](../../../../../../gaussian-random-variable.md) $\varepsilon_i$ gives

$$
\mathbb E B^2=\frac1{N^2h^2}\sum_{i=1}^N\mathbb E\varepsilon_i^2
=\frac{\sigma^2}{Nh^2}.
$$

Consequently

$$
\boxed{\mathbb E|\widehat g_N-g'(x_0)|^2
\leq\frac{h^2M^2}{4}+\frac{\sigma^2}{Nh^2}}.
$$

The two terms are balanced by

$$
h_N^2=\frac{2\sigma}{M\sqrt N},
\qquad
h_N=\left(\frac{2\sigma}{M}\right)^{1/2}N^{-1/4}.
$$

At this value both terms equal $\sigma M/(2\sqrt N)$, and hence

$$
\boxed{\mathbb E|\widehat g_N-g'(x_0)|^2\leq\frac{\sigma M}{\sqrt N}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
