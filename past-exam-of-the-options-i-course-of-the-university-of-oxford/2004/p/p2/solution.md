<h1 id="p/p2/solution">Solution</h1>

↑ **Parent:** [P2](../p2.md)

For any $q$ in the [polynomial](../../../../polynomial-split.md) trial space, $f-q=(f-p)+(p-q)$ and $p-q$ is in that same space. The assumed [orthogonality](../../../../orthogonal-vectors.md) therefore gives the Pythagorean identity

$$
\boxed{\|f-q\|^2=\|f-p\|^2+\|p-q\|^2\geq\|f-p\|^2.}
$$

Thus $p$ is the [best approximation](../../../../best-approximation-in-a-normed-space.md); equality is possible only when $q=p$ because the [inner product](../../../../inner-product-split.md) is [positive-definite](../../../../positive-definite-bilinear-form.md).

Write the linear [polynomial](../../../../polynomial-split.md) as $p=A+Bx$. [Orthogonality](../../../../orthogonal-vectors.md) of $x^2-p$ to $1$ and $x$ in the [weighted inner product](../../../../weighted-inner-product.md) gives

$$
\frac14-\frac A2-\frac B3=0,\qquad
\frac15-\frac A3-\frac B4=0.
$$

Solving yields

$$
\boxed{p(x)=-\frac3{10}+\frac65x.}
$$

The weighted squared error is $\int_0^1x(x^2-6x/5+3/10)^2dx=1/600$, providing an additional exact check. The weight's zero value at one endpoint does not destroy positive definiteness on [continuous](../../../../continuous-function.md) functions: a nonzero [continuous](../../../../continuous-function.md) function is nonzero on an interval of positive weight.

## ↑ Ancestors (12)

1. [P2](../p2.md)
2. [P](../../p.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
