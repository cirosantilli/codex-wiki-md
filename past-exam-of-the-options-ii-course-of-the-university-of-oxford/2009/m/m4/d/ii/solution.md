<h1 id="m/m4/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $Z_t=\sum_{j=1}^{N_t}Y_j$, with an empty sum equal to zero. Conditioning on the independent [Poisson random variable](../../../../../../poisson-distribution.md) $N_t$, the [moment-generating function](../../../../../../moment-generating-function.md) is

$$
\mathbb E e^{\theta Z_t}=\sum_{n=0}^\infty e^{-\lambda t}\frac{(\lambda t)^n}{n!}M_Y(\theta)^n
=\boxed{\exp\{\lambda t(M_Y(\theta)-1)\}}.
$$

This is the [compound Poisson distribution](../../../../../../compound-poisson-distribution.md). Differentiating its log moment-generating [function](../../../../../../function-split.md) at zero, when the first two moments are finite, gives

$$
\boxed{\mathbb E Z_t=\lambda t\mathbb EY,\qquad\operatorname{Var}(Z_t)=\lambda t\mathbb E(Y^2)}.
$$

The [variance](../../../../../../variance-split.md) includes variability in the number of coaches, and so uses the second moment, not merely $\operatorname{Var}(Y)$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [M4](../../../m4.md)
4. [M](../../../../m.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
