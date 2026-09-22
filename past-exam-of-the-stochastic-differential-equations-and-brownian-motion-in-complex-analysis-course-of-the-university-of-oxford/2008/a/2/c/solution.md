<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the logarithm of the explicit solution gives a linear function of the [normal random variable](../../../../../gaussian-random-variable.md) $B_t$:

$$
\log X_t=\log x+(r-\sigma^2/2)t+\sigma B_t.
$$

Thus

$$
\boxed{X_t\sim\operatorname{Lognormal}
(\log x+(r-\sigma^2/2)t,\ \sigma^2t).}
$$

For $z>0$ its density is

$$
\frac1{z\sigma\sqrt{2\pi t}}
\exp\left[-\frac{(\log(z/x)-(r-\sigma^2/2)t)^2}
{2\sigma^2t}\right],
$$

and it is zero for $z\leq0$. The factor $1/z$ is the Jacobian of the logarithmic change of variable.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
