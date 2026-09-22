<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Extend the integrand by zero to all of $(0,\infty)$:

$$
h_n(x)=\mathbf1_{(0,2n\pi)}(x)\frac{(n+x)\sin(x/n)}{x(1+x^2)}.
$$

For each fixed $x>0$, eventually the [indicator function](../../../../indicator-function.md) is one and $\sin(x/n)/(x/n)\to1$. Hence $h_n(x)\to(1+x^2)^{-1}$ [pointwise](../../../../pointwise-convergence.md). On its support, $x/n\leq2\pi$, so $|\sin t|\leq t$ for $t\geq0$ gives

$$
|h_n(x)|\leq\frac{1+x/n}{1+x^2}\leq\frac{1+2\pi}{1+x^2}.
$$

The final bound is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) on $(0,\infty)$ and independent of $n$. The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) therefore gives

$$
\boxed{\lim_{n\to\infty}\int_0^{2n\pi}\frac{(n+x)\sin(x/n)}{x(1+x^2)}\,dx
=\int_0^\infty\frac{dx}{1+x^2}=\frac\pi2.}
$$

The last integral follows from the [antiderivative](../../../../antiderivative.md) $\arctan x$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
