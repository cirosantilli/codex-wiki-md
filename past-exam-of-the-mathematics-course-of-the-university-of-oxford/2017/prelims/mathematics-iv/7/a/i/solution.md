<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

The [euclidean algorithm](../../../../../../../euclidean-algorithm.md) computes the [greatest common divisor](../../../../../../../greatest-common-divisor.md) of two [integers](../../../../../../../integer-split.md) by repeated [division with remainder](../../../../../../../euclidean-division.md). Start with $r_0=|A|$, $r_1=|B|$, interchanging them if necessary, and repeatedly write

$$
r_{j-1}=q_jr_j+r_{j+1},\qquad 0\le r_{j+1}<r_j,
$$

until a zero remainder occurs. The positive remainders strictly decrease, so the process terminates. At each step the common [divisors](../../../../../../../divisor.md) of $r_{j-1},r_j$ are exactly the common [divisors](../../../../../../../divisor.md) of $r_j,r_{j+1}$, because $r_{j+1}=r_{j-1}-q_jr_j$. Hence

$$
\boxed{\gcd(A,B)=\text{the last nonzero remainder}.}
$$

If one input is zero, the answer is the [absolute value](../../../../../../../absolute-value.md) of the other; the usual convention sets $\gcd(0,0)=0$. Back-substitution also expresses the [greatest common divisor](../../../../../../../greatest-common-divisor.md) as an [integer linear combination](../../../../../../../integer-linear-combination.md) of the inputs, as in [Bézout's identity](../../../../../../../bezout-s-identity.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [7](../../../7.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
