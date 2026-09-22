<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Insert the [Poisson distribution](../../../../../../poisson-distribution.md) [probability generating function](../../../../../../probability-generating-function.md) into the preceding bound:

$$
\mathbb P(X\geq x)\leq\exp\bigl(\lambda(s-1)-x\log s\bigr),\qquad s>1.
$$

For fixed $x>\lambda$, differentiate the exponent with respect to $s$. Its [derivative](../../../../../../derivative.md) is $\lambda-x/s$, and its [second derivative](../../../../../../second-derivative.md) is $x/s^2>0$, so its unique minimum occurs at $s=x/\lambda>1$. At that value,

$$
\lambda(s-1)-x\log s=x-\lambda-x\log(x/\lambda).
$$

Consequently

$$
\boxed{\mathbb P(X\geq x)\leq e^{-\lambda}\left(\frac{e\lambda}{x}\right)^x.}
$$

This [Chernoff bound](../../../../../../chernoff-bound.md) remains valid for noninteger positive thresholds $x>\lambda$; the [event](../../../../../../event.md) is then the same as exceeding or equalling its [integer](../../../../../../integer-split.md) ceiling.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
