<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [elliptic curve method](../../../../../elliptic-curve-method.md), addition is attempted modulo the composite number. A denominator that is not a [unit in a ring](../../../../../unit-in-a-ring.md) supplies a factor through its [greatest common divisor](../../../../../greatest-common-divisor.md) with that number.

First double $P$ using the [elliptic-curve addition formula](../../../../../elliptic-curve-addition-formula.md). Its tangent slope is

$$
m=\frac{3\cdot1^2+5}{2\cdot1}=4,
\qquad x(2P)=4^2-2=14,\qquad
y(2P)=4(1-14)-1=-53.
$$

These calculations are valid modulo $221$ since the only initial denominator is two, which is invertible. Thus $2P=(14,-53)$, equivalently $(14,168)$ modulo $221$.

To form $3P=P+2P$, the chord slope would require

$$
\frac{-53-1}{14-1}=\frac{-54}{13}\pmod{221}.
$$

The denominator has

$$
\boxed{\gcd(13,221)=13,\qquad221=13\cdot17.}
$$

It cannot be inverted, and thirteen is the requested proper factor. The failure has a geometric explanation: modulo thirteen, $2P=(1,-1)=-P$, so $3P$ is the point at infinity. Modulo seventeen that chord denominator remains nonzero. The differing behavior at the two [primes](../../../../../prime-number-split.md) is exactly what the [elliptic curve method](../../../../../elliptic-curve-method.md) detects.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
