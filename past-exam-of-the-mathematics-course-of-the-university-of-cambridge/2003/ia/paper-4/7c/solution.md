<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

For [integers](../../../../../integer.md) $m,n$ not both zero, their [greatest common divisor](../../../../../greatest-common-divisor.md) is the greatest [positive integer](../../../../../positive-integer.md) dividing both. For the degenerate pair $(0,0)$ use the conventional value zero. A number $d$ divides both $m,n$ exactly when it divides both $m+kn,n$: one direction uses closure of divisibility under sums; the reverse subtracts $kn$. The positive common-divisor sets are therefore identical, proving

$$
\boxed{\gcd(m,n)=\gcd(m+kn,n)}.
$$

This also holds for $(0,0)$ under the stated convention and does not depend on the signs of the [integers](../../../../../integer.md).

[Bezout identity](../../../../../bezout-identity.md) states that there exist [integers](../../../../../integer.md) $a,b$ such that $am+bn=\gcd(m,n)$. If a prime $p$ divides $mn$ but does not divide $m$, then $\gcd(p,m)=1$, so choose $a,b$ with $ap+bm=1$. Multiplying by $n$ gives $apn+bmn=n$. Both terms on the left are divisible by $p$, so $p\mid n$. Thus

$$
\boxed{p\mid mn\ \Longrightarrow\ p\mid m\text{ or }p\mid n},
$$

which proves the [Euclid lemma](../../../../../euclid-lemma.md) from the requested identity. The separately numbered entries use these arithmetic facts for the [Fibonacci numbers](../../../../../fibonacci-number.md).

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
