<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose an integer [right triangle](../../../../../../right-triangle.md) with square area exists, and choose one with the least positive hypotenuse $c$. It is primitive. Indeed, dividing all sides by their common divisor $d$ gives an integer right triangle whose area is the square of the rational number $s/d$, where $s^2$ was the original area. Its area is an integer, since one of its legs is even. A rational number whose square is an integer is itself an integer, as follows by writing it in lowest terms. Thus division by $d>1$ would give another square-area triangle with smaller hypotenuse.

By the [primitive Pythagorean parametrization](../../../../../../primitive-pythagorean-parametrization.md), after ordering the legs the triangle has sides $n^2-m^2,2nm,n^2+m^2$, with coprime $n>m>0$ of opposite parity. Its area is

$$
nm(n-m)(n+m).
$$

These four positive factors are pairwise [coprime](../../../../../../coprime-integers.md): the pair $n-m,n+m$ has gcd dividing $2m$ and is odd, and the other pairs have gcd one by $\gcd(n,m)=1$. Since the product is a square, each factor is a square. Write

$$
n=u^2,\qquad m=v^2,\qquad n+m=w^2,\qquad n-m=z^2.
$$

Both $w,z$ are odd. Odd squares are $1\pmod8$, so $2m=w^2-z^2$ is divisible by eight; hence $m$ is divisible by four and $v$ is even. Define positive integers

$$
r=\frac{w+z}{2},\qquad s=\frac{w-z}{2}.
$$

They satisfy

$$
r^2+s^2=\frac{w^2+z^2}{2}=n=u^2,\qquad
\frac{rs}{2}=\frac{w^2-z^2}{8}=\frac m4=\left(\frac v2\right)^2.
$$

Thus $(r,s,u)$ is another positive integer right triangle with square area, but its hypotenuse $u=\sqrt n$ is strictly smaller than $n^2+m^2=c$. This contradicts minimality. **No integer right triangle has a nonzero square area.** This is the [Fermat right triangle theorem](../../../../../../fermat-right-triangle-theorem.md), with the actual [infinite descent](../../../../../../infinite-descent.md) construction exhibited.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
