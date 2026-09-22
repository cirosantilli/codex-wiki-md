<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Complete the square in the transformation:

$$
Y=X(2-X)=1-(X-1)^2.
$$

Since $0<X<2$ almost surely, $0<Y\leq1$. For $0\leq y<1$, put $r=\sqrt{1-y}$. The [event](../../../../../event.md) $Y>y$ is equivalent to $1-r<X<1+r$. Integrating the given [probability density function](../../../../../probability-density-function.md) over both branches at once gives the [survival function](../../../../../survival-function.md)

$$
\begin{aligned}
\mathbb P(Y>y)&=\int_{1-r}^{1+r}\frac x2\,dx
=\frac{(1+r)^2-(1-r)^2}{4}=r.
\end{aligned}
$$

Thus, including the tails,

$$
\boxed{\mathbb P(Y>y)=\begin{cases}1&y<0,\\\sqrt{1-y}&0\leq y<1,\\0&y\geq1.\end{cases}}
$$

The [cumulative distribution function](../../../../../cumulative-distribution-function.md) on $(0,1)$ is $1-\sqrt{1-y}$. Differentiation gives

$$
\boxed{f_Y(y)=\begin{cases}\dfrac1{2\sqrt{1-y}}&0<y<1,\\0&\text{otherwise}.\end{cases}}
$$

Both inverse branches matter: $x=1\pm\sqrt{1-y}$. The endpoint divergence is integrable, and $\mathbb P(Y=1)=\mathbb P(X=1)=0$, so no endpoint atom is needed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
