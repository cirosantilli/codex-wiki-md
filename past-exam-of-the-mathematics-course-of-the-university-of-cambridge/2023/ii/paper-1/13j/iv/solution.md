<h1 id="13j/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\widehat\beta_{(i)}$ be the least-squares estimate after deleting observation $i$, and put $\widehat Y=X\widehat\beta$ and $\widehat Y_{(i)}=X\widehat\beta_{(i)}$. [Cook's distance](../../../../../../cook-s-distance.md) is

$$
\boxed{
D_i
=\frac{\|\widehat Y_{(i)}-\widehat Y\|^2}
 {p\widehat\sigma^2}
=\frac{(\widehat\beta_{(i)}-\widehat\beta)^TX^TX
 (\widehat\beta_{(i)}-\widehat\beta)}
 {p\widehat\sigma^2}
}.
$$

Thus $D_i$ is the squared displacement caused by deleting observation $i$, measured in the same $X^TX$ metric and scale as the confidence ellipsoid. In particular, $\widehat\beta_{(i)}$ lies outside the $(1-\alpha)$ ellipsoid centered at $\widehat\beta$ exactly when

$$
D_i>F_{p,n-p}(1-\alpha).
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
