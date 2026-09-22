<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [Pollard's p-1 algorithm](../../../../pollard-s-p-1-algorithm.md), a large exponent containing many small factors makes $a^M-1$ divisible by a [prime factor](../../../../prime-factor.md) whose predecessor divides $M$, by [Fermat's little theorem](../../../../fermat-little-theorem.md). A [greatest common divisor](../../../../greatest-common-divisor.md) with the number being factored can then separate that [prime factor](../../../../prime-factor.md) from the others.

Choose base $a=2$ and build factorial exponents using [modular exponentiation](../../../../modular-exponentiation.md). The successive exponents $2!$, $3!$, and $4!$ give

$$
2^2\equiv4,\qquad 2^6\equiv64,\qquad
2^{24}\equiv64^4\equiv35\pmod{1003}.
$$

The first two [greatest common divisors](../../../../greatest-common-divisor.md) are $\gcd(3,1003)=\gcd(63,1003)=1$. At the next step the [Euclidean algorithm](../../../../euclidean-algorithm.md) gives

$$
\gcd(2^{24}-1,1003)=\gcd(34,1003)=17,
\qquad 1003=29\cdot34+17.
$$

Hence

$$
\boxed{17\text{ is a factor of }1003,\qquad1003=17\cdot59.}
$$

Here the [element order](../../../../order-of-a-group-element.md) of $2$ modulo $17$ is $8$, which divides $24$, even though $17-1=16$ does not divide $24$. The algorithm only needs the [element order](../../../../order-of-a-group-element.md) to divide the chosen exponent; divisibility by the full predecessor is a sufficient condition, not a necessary one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
