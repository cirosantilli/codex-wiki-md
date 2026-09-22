<h1 id="11g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An odd composite $N$ coprime to $b$ is a [Fermat pseudoprime](../../../../../../fermat-pseudoprime.md) to base $b$ when $b^{N-1}\equiv1\pmod N$. It is a [Carmichael number](../../../../../../carmichael-number.md) when this congruence holds for every $b$ coprime to $N$.

Suppose a Carmichael number has $p^a\Vert N$ with $a\geq2$. The group $(\mathbb Z/p^a\mathbb Z)^*$ is cyclic, so choose a residue of order

$$
\varphi(p^a)=p^{a-1}(p-1).
$$

By the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md), extend it to an integer $b$ that is congruent to $1$ modulo every other prime-power factor of $N$. Then $\gcd(b,N)=1$, and the Carmichael congruence forces the order of $b$ modulo $p^a$ to divide $N-1$. In particular $p\mid N-1$, contradicting $p\mid N$. Therefore every Carmichael number is [square-free](../../../../../../square-free-integer.md).

Now assume $N$ is square-free. If $p-1\mid N-1$ for every $p\mid N$, then for every $b$ coprime to $N$, [Fermat little theorem](../../../../../../fermat-little-theorem.md) gives

$$
b^{N-1}\equiv1\pmod p
$$

for each $p\mid N$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) then gives the congruence modulo $N$, so $N$ is Carmichael.

Conversely, if $N$ is Carmichael, fix $p\mid N$. Choose a [primitive root](../../../../../../primitive-root-modulo-n.md) $g$ modulo $p$ and use the Chinese remainder theorem to choose $b\equiv g\pmod p$ and $b\equiv1\pmod{N/p}$. Then $b^{N-1}\equiv1\pmod p$, so the order $p-1$ of $g$ divides $N-1$. This proves the [Korselt criterion](../../../../../../korselt-criterion.md) in the required form:

$$
\boxed{N\text{ is Carmichael}\iff
N\text{ is square-free and }p-1\mid N-1\text{ for every }p\mid N.}
$$

A Carmichael number cannot have one prime factor because it is composite. If $N=pq$ with distinct primes $p<q$, the condition $q-1\mid pq-1$ implies $q-1\mid p-1$, which is impossible. Hence **every Carmichael number has at least three prime factors**.

## ↑ Ancestors (11)

1. [B](../b.md)
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
