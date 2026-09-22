<h1 id="30e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
\phi(t)=t^3-2t^2+t=t(t-1)^2.
$$

On $[0,2]$, its global maximum is the endpoint $t=2$, where

$$
\phi(2)=2,
\qquad
\phi'(2)=5,
$$

and the amplitude $\log t$ has value $\log2$. The endpoint form of [Laplace's method](../../../../../../laplace-s-method.md) therefore gives

$$
\boxed{
I(x)\sim\frac{\log2}{5x}e^{2x}
}.
$$

Indeed, with $u=2-t$, Taylor expansion gives $\phi(2-u)=2-5u+O(u^2)$ and $\log(2-u)=\log2+O(u)$; the scale contributing to the integral is $u=O(x^{-1})$. Outside any fixed neighbourhood of $2$, $\phi$ is bounded above by $2-\delta$, so that part is exponentially smaller. This also controls the integrable logarithmic singularity at zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30E](../../30e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
