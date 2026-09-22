<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

The [probability generating function](../../../../../probability-generating-function.md) is

$$
p_X(z)=\mathbb E[z^X]=\sum_{n\geq1}\mathbb P(X=n)z^n,\qquad |z|\leq1.
$$

For [independent random variables](../../../../../independent-random-variables.md), the bounded factors $z^X$ and $z^Y$ have factorizing [expectation](../../../../../expected-value.md), so

$$
\boxed{p_{X+Y}(z)=\mathbb E[z^Xz^Y]=\mathbb E[z^X]\mathbb E[z^Y]=p_X(z)p_Y(z).}
$$

This includes complex $z$ in the indicated disk by absolute convergence.

For the dice construction, encode the labels of an ordinary die by $F(z)=z+z^2+\cdots+z^6$. Its [probability generating function](../../../../../probability-generating-function.md) is $F(z)/6$. A useful factorization into [polynomial factors](../../../../../polynomial-factor.md) is

$$
F(z)=z(1+z)(1+z+z^2)(1-z+z^2).
$$

Use [redistribution of polynomial factors for dice](../../../../../redistribution-of-polynomial-factors-for-dice.md) to define

$$
\begin{aligned}
A(z)&=\frac{F(z)}{1-z+z^2}=z(1+z)(1+z+z^2)=z+2z^2+2z^3+z^4,\\
B(z)&=F(z)(1-z+z^2)=z+z^3+z^4+z^5+z^6+z^8.
\end{aligned}
$$

Both [polynomials](../../../../../polynomial-split.md) have nonnegative integer [coefficients](../../../../../coefficient.md), no constant term, and coefficient sum six. They therefore describe fair six-sided dice with strictly positive face labels

$$
\boxed{A:(1,2,2,3,3,4),\qquad B:(1,3,4,5,6,8).}
$$

When these dice are thrown with [independent](../../../../../independent-random-variables.md) outcomes, the sum has [probability generating function](../../../../../probability-generating-function.md) $A(z)B(z)/36=F(z)^2/36$. Equality of [coefficients](../../../../../coefficient.md) proves equality of every sum [probability](../../../../../probability.md), including all totals from two to twelve, with zero probability outside that range. Both dice are nonstandard, completing the construction.

## ↑ Ancestors (11)

1. [9F](../9f.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
