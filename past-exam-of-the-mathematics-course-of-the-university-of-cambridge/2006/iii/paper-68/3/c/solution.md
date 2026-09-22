<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $|\alpha|>1$, an exterior [polynomial root](../../../../../../root-of-a-polynomial.md) of $\rho$ persists by [continuity](../../../../../../continuous-function.md) for sufficiently small negative real $z$ in the [stability](../../../../../../stability-of-a-numerical-method.md) [polynomial](../../../../../../polynomial-split.md) $\rho(w)-z\sigma(w)$. Hence these parameters cannot be [A-stable](../../../../../../a-stability.md).

For $-1\le\alpha<1$, the principal [polynomial root](../../../../../../root-of-a-polynomial.md) at $w=1,z=0$ is simple. Let $s(z)=\log w(z)$ denote its analytic [logarithm](../../../../../../logarithm.md) near zero. Using the expansion in part (b), and $\rho'(1)=2(1-\alpha)$, solve the [polynomial root](../../../../../../root-of-a-polynomial.md) equation to obtain

$$
s(z)=z+Cz^4+O(z^5),\qquad C=\frac{\alpha+5}{24(1-\alpha)}>0.
$$

Indeed the residual at $s=z$ is $-(\alpha+5)z^4/12$, and the correction in $s$ cancels it by multiplication with $2(1-\alpha)$. Choose $z=-C\varepsilon^4/2+i\varepsilon$. This lies strictly in the left half-plane, but

$$
\operatorname{Re}s(z)=\frac C2\varepsilon^4+O(\varepsilon^5)>0
$$

for small positive $\varepsilon$. Thus $|w(z)|=e^{\operatorname{Re}s(z)}>1$, proving [linear instability](../../../../../../linear-instability.md) within the [A-stability](../../../../../../a-stability.md) domain. This is a direct [principal-root obstruction to A-stability](../../../../../../principal-root-obstruction-to-a-stability.md), rather than an appeal to an order-barrier theorem alone.

Finally, at $\alpha=1$, the full [stability](../../../../../../stability-of-a-numerical-method.md) [polynomial](../../../../../../polynomial-split.md) is

$$
\rho(w)-z\sigma(w)=(w-1)^2\bigl((1-z)w-1\bigr).
$$

It retains a double unit [polynomial root](../../../../../../root-of-a-polynomial.md) for every negative $z$, allowing growing parasitic solutions. Therefore

$$
\boxed{\text{There is no real }\alpha\text{ for which the printed recurrence is A-stable}.}
$$

The canceled [Backward Euler method](../../../../../../backward-euler-method.md) recurrence at $\alpha=1$ is [A-stable](../../../../../../a-stability.md), but its admissible solutions and starting relations differ from those of the original method.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
