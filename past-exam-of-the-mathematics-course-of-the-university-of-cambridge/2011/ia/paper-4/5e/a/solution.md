<h1 id="5e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [greatest common divisor](../../../../../../greatest-common-divisor.md) $d=\gcd(a,b)$ is the largest positive integer dividing both $a$ and $b$. To prove [Bezout identity](../../../../../../bezout-identity.md) without assuming unique factorization, let $d_0$ be the least positive member of

$$
\{\lambda a+\mu b:\lambda,\mu\in\mathbb Z\}.
$$

This set has positive members, for example $a$, so [well-ordering principle](../../../../../../well-ordering-principle-for-the-natural-numbers.md) supplies $d_0$. Divide $a$ by $d_0$ using [Euclidean division](../../../../../../euclidean-division.md): $a=qd_0+r$, $0\leq r<d_0$. The remainder $r=a-qd_0$ is another integer linear combination of $a,b$. Minimality forces $r=0$, so $d_0\mid a$. The same argument gives $d_0\mid b$. Every common divisor divides every integer linear combination, hence divides $d_0$. Therefore $d_0$ is the [greatest common divisor](../../../../../../greatest-common-divisor.md), and

$$
\boxed{\gcd(a,b)=\lambda a+\mu b\quad\text{for some }\lambda,\mu\in\mathbb Z.}
$$

This argument also proves that every common divisor divides the [greatest common divisor](../../../../../../greatest-common-divisor.md).

The positive integers with the stated product-divisibility property are

$$
\boxed{n=1\quad\text{or}\quad n\text{ is a prime number}.}
$$

The case $n=1$ is immediate. If $p$ is [prime](../../../../../../prime-number.md) and $p\nmid a$, its only possible common positive divisor with $a$ is one. By [Bezout identity](../../../../../../bezout-identity.md), $\lambda p+\mu a=1$. Multiplying by $b$ shows that $p\mid ab$ implies $p\mid b$. This proves [Euclid lemma](../../../../../../euclid-lemma.md) directly. Conversely, if $n>1$ is not [prime](../../../../../../prime-number.md), it has a divisor $r$ with $1<r<n$. Put $s=n/r$; then $1<s<n$. Although $n\mid rs$, neither $r$ nor $s$ is divisible by $n$, disproving the property for a composite $n$.

Finally, suppose $ab=cd$ for four distinct [primes](../../../../../../prime-number.md). Then $a\mid cd$, so [Euclid lemma](../../../../../../euclid-lemma.md) gives $a\mid c$ or $a\mid d$. A [prime](../../../../../../prime-number.md) has no positive divisor other than one and itself, so this would mean $a=c$ or $a=d$, a contradiction. **Products of these two disjoint pairs cannot be equal.** No form of the fundamental theorem of arithmetic was used: the required prime-divisibility fact was proved from [Bezout identity](../../../../../../bezout-identity.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
