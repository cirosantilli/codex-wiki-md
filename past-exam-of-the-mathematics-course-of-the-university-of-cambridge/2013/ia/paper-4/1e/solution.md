<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [greatest common divisor](../../../../../greatest-common-divisor.md) $d=\gcd(m,n)$ is the largest positive integer dividing both $m$ and $n$. To prove [Bézout's identity](../../../../../bezout-identity.md) without assuming a factorization theorem, consider the nonempty set of positive integer linear combinations

$$
\mathcal L=\{am+bn>0:a,b\in\mathbb Z\}.
$$

It contains $m$, so the [well-ordering principle](../../../../../well-ordering-principle-for-the-natural-numbers.md) gives a least element $d_0=am+bn$. By [Euclidean division](../../../../../euclidean-division.md), write $m=qd_0+r$ with $0\leq r<d_0$. Then

$$
r=(1-qa)m-qbn
$$

is another integer linear combination. If $r>0$, it contradicts minimality, so $r=0$ and $d_0\mid m$. Applying the same argument to $n$ gives $d_0\mid n$. Conversely, every common divisor divides every integer linear combination and therefore divides $d_0$. In particular every positive common divisor is at most $d_0$. Thus $d_0=d$ and

$$
\boxed{\gcd(m,n)=am+bn\quad\text{for some }a,b\in\mathbb Z.}
$$

This also proves the requested divisibility implication for any integer $k$: if $k\mid m$ and $k\mid n$, then $k\mid(am+bn)=d$.

For the [scaling identity for greatest common divisors](../../../../../scaling-identity-for-greatest-common-divisors.md), put $D=\gcd(km,kn)$ with $k>0$. Since $kd$ divides $km$ and $kn$, $D\geq kd$. On the other hand, multiplying [Bézout's identity](../../../../../bezout-identity.md) by $k$ expresses $kd$ as $a(km)+b(kn)$, so $D\mid kd$. Positivity gives $D\leq kd$. Therefore **without using prime factorization**,

$$
\boxed{\gcd(km,kn)=k\gcd(m,n).}
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
