<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

The supplied [integral basis](../../../../../integral-basis.md) differs unimodularly from $1,\zeta,\zeta^2,\zeta^3$, since $1=-\zeta-\zeta^2-\zeta^3-\zeta^4$. With $f(t)=\Phi_5(t)=(t^5-1)/(t-1)$, the [field discriminant](../../../../../field-discriminant.md) is $\operatorname{Norm}(f'(\zeta))$, the degree-four sign being positive. At a nonidentity fifth root,

$$
f'(\zeta)=\frac{5\zeta^4}{\zeta-1},\qquad
\operatorname{Norm}(1-\zeta)=\Phi_5(1)=5,
$$

so

$$
\boxed{\operatorname{disc}K=5^4/5=125}.
$$

The [Minkowski bound for ideal classes](../../../../../minkowski-s-bound.md) gives an integral ideal in every ideal class with norm at most $[3/(2\pi^2)]\sqrt{125}<2$. Its positive integer norm must be one, so it is the whole integer ring. Every class is trivial, proving **all ideals are principal**.

For $1\le n\le4$, $u_n=(1-\zeta^n)/(1-\zeta)=1+\zeta+\cdots+\zeta^{n-1}$ is an [algebraic integer](../../../../../algebraic-integer.md). The numerator has the same norm five as the denominator, because its conjugates permute the nonidentity fifth roots. Thus $\operatorname{Norm}(u_n)=1$, proving it is a unit. Multiplying the four numerator factors gives five, hence

$$
\boxed{5/(1-\zeta)^4=\prod_{n=1}^4u_n\ \text{is a unit}}.
$$

The ideal $P=(1-\zeta)$ has norm five; explicitly reduction modulo it sets $\zeta=1$ and gives the quotient $\mathbb F_5$. Thus it is prime and $(5)=P^4$: five is totally ramified, with [ramification index](../../../../../ramification-index.md) four and [residue degree](../../../../../residue-degree.md) one. A rational prime can ramify only if it divides the field [field discriminant](../../../../../field-discriminant.md), so no rational prime other than five ramifies, and there are no other ramified prime ideals.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
