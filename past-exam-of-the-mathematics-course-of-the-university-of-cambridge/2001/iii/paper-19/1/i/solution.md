<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

There is a necessary ordering qualification: the printed formula requires the even leg to be called $b$. The primitive [Pythagorean triple](../../../../../../pythagorean-triple.md) $(a,b,c)=(4,3,5)$ satisfies the printed hypotheses but cannot have $b=2nm$. Thus the intended assertion is true **after interchanging the two legs if necessary**. We prove that version, including the parity condition on the parameters.

A primitive [Pythagorean triple](../../../../../../pythagorean-triple.md) has pairwise [coprime](../../../../../../coprime-integers.md) sides: a prime dividing any two also divides the third. The two legs cannot both be odd, since their squares would sum to $2\pmod4$, and cannot both be even. Call the odd leg $a$ and the even leg $b$; then $c$ is odd. The positive integers

$$
u=\frac{c+a}{2},\qquad v=\frac{c-a}{2}
$$

satisfy $uv=(b/2)^2$ and are [coprime](../../../../../../coprime-integers.md), since a common divisor divides both $c$ and $a$. A product of [coprime](../../../../../../coprime-integers.md) positive [integers](../../../../../../integer.md) is a square only when both factors are squares, by their [prime factorizations](../../../../../../fundamental-theorem-of-arithmetic.md). Write $u=n^2$, $v=m^2$. Then $n>m>0$, $\gcd(n,m)=1$, and

$$
\boxed{a=n^2-m^2,\qquad b=2nm,\qquad c=n^2+m^2.}
$$

Furthermore $n,m$ have opposite parity, since $c$ is odd. Conversely these coprimality and parity conditions give a primitive triple: the square identity follows by expansion, and a common odd prime divisor of its legs would divide both $n,m$, while the odd leg excludes a common factor two. This is the [primitive Pythagorean parametrization](../../../../../../primitive-pythagorean-parametrization.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
