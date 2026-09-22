<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The converted source omits $r$ from the product; the PDF asks about $N=pqr$. Fix the odd prime $r$, and suppose $pqr$ is Carmichael. Its three prime factors are distinct by the [Korselt criterion](../../../../../../korselt-criterion.md). Relabel $p,q$ so that $p<q$.

The divisibility conditions include

$$
q-1\mid pr-1,\qquad p-1\mid qr-1.
$$

Write

$$
pr-1=b(q-1)
$$

for a positive integer $b$. Since $p<q$,

$$
pr-1<r(q-1),
$$

so $1\leq b<r$. Moreover,

$$
q=\frac{pr+b-1}{b}.
$$

Multiplying the second divisibility by $b$ and reducing modulo $p-1$ gives

$$
p-1\mid b(qr-1)
=pr^2+r(b-1)-b
\equiv(r-1)(r+b)\pmod{p-1}.
$$

The positive integer on the right is at most $(r-1)(2r-1)$. Consequently

$$
p\leq(r-1)(2r-1)+1.
$$

There are only finitely many possible primes $p$ and integers $b\in\{1,\ldots,r-1\}$, and each pair determines at most one $q=(pr+b-1)/b$. Therefore

$$
\boxed{\text{for fixed }r,\text{ only finitely many prime pairs }(p,q)
\text{ make }pqr\text{ Carmichael}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
