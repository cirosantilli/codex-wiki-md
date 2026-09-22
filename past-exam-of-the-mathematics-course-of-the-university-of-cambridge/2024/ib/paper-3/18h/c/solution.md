<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Bayes' formula divides the point-null contribution to the mixture density by the full marginal density:

$$
q(\overline x)
=\frac{\phi_{1/n}(\overline x)}
{\phi_{1/n}(\overline x)+
 \phi_{\tau^2+1/n}(\overline x)}.
$$

Since

$$
\frac{\phi_{\tau^2+1/n}(\overline x)}
{\phi_{1/n}(\overline x)}
=\frac1{\sqrt{1+n\tau^2}}
\exp\left[
\frac{n^2\tau^2\overline x^2}{2(1+n\tau^2)}
\right],
$$

the [posterior probability of a Gaussian point null](../../../../../../posterior-probability-of-a-gaussian-point-null.md) is

$$
\boxed{
q(\overline x)=
\left\{
1+\frac1{\sqrt{1+n\tau^2}}
\exp\left[
\frac{n^2\tau^2\overline x^2}{2(1+n\tau^2)}
\right]
\right\}^{-1}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
