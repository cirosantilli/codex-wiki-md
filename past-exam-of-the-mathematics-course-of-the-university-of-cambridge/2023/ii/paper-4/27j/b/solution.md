<h1 id="27j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N$ be the homogeneous [Poisson point process](../../../../../../poisson-point-process.md) in $\mathbb R^3$ with intensity measure $\lambda\,dx$, and map each point $x$ to its radius $g(x)=|x|$. For an interval $(a,b]\subseteq\mathbb R_+$, the [pushforward measure](../../../../../../pushforward-measure.md) of the intensity is

$$
\lambda\,\operatorname{vol}\{x:a<|x|\leq b\}
=\frac{4\pi\lambda}{3}(b^3-a^3).
$$

The [Mapping theorem for Poisson point processes](../../../../../../mapping-theorem-point-process.md) therefore shows that the radii form a Non-homogeneous Poisson point process with intensity function

$$
\rho(r)=\frac{d}{dr}\left(\frac{4\pi\lambda r^3}{3}\right)=4\pi\lambda r^2,
\qquad r>0.
$$

If $R$ is the distance to the closest star, the event $\{R>r\}$ says that the ball of radius $r$ contains no points. The zero-count probability of a [Poisson distribution](../../../../../../poisson-distribution.md) gives

$$
\mathbb P(R>r)=\exp\left(-\frac{4\pi\lambda r^3}{3}\right).
$$

Differentiating its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) yields the [probability density function](../../../../../../probability-density-function.md)

$$
\boxed{f_R(r)=4\pi\lambda r^2
\exp\left(-\frac{4\pi\lambda r^3}{3}\right),
\qquad r\geq0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27J](../../27j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
