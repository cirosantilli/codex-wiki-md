<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

[Fermat's little theorem](../../../../../fermat-little-theorem.md) states that, for a [prime number](../../../../../prime-number.md) $p$ and any integer $a$,

$$
a^p\equiv a\pmod p.
$$

If $p\mid a$, both sides vanish modulo $p$. Otherwise multiplication by $a$ permutes the nonzero residue classes modulo $p$: it is injective because $ai\equiv aj$ implies $i\equiv j$ by cancellation. Taking the products of these residues gives

$$
a^{p-1}(p-1)!\equiv(p-1)!\pmod p.
$$

The [factorial](../../../../../factorial.md) is [coprime](../../../../../coprime-integers.md) to $p$, so cancellation proves $a^{p-1}\equiv1\pmod p$ and hence the stated version. This proves [Fermat's little theorem](../../../../../fermat-little-theorem.md) in both cases.

Let $n$ be a [Carmichael number](../../../../../carmichael-number.md). If a [prime](../../../../../prime-number.md) square $p^2$ divided $n$, choose $a=p$. Since $n$ is an odd composite integer, $n>1$, and $p^n-p\equiv-p\not\equiv0\pmod{p^2}$. This contradicts the required [modular congruence](../../../../../modular-congruence.md) modulo $n$. Therefore **every Carmichael number is squarefree**.

For each [prime](../../../../../prime-number.md) divisor $p$ of $n$, choose the allowed [primitive root](../../../../../primitive-root-modulo-n.md) $g$ modulo $p$. The Carmichael identity applied to the positive integer $g$ gives $g^n\equiv g\pmod p$, and cancellation gives $g^{n-1}\equiv1\pmod p$. By its defining order property,

$$
p-1\mid n-1.
$$

Conversely, suppose a composite integer $n$ is squarefree and has this divisibility for every [prime](../../../../../prime-number.md) divisor. For an arbitrary integer $a$, modulo a [prime](../../../../../prime-number.md) divisor $p$ there are two cases. If $p\mid a$, then $a^n\equiv a\equiv0$. Otherwise [Fermat's little theorem](../../../../../fermat-little-theorem.md) and $p-1\mid n-1$ give $a^{n-1}\equiv1$, so again $a^n\equiv a$. Since the [prime](../../../../../prime-number.md) divisors are distinct and pairwise [coprime](../../../../../coprime-integers.md), their product $n$ divides $a^n-a$. This is the [proof of Korselt criterion](../../../../../proof-of-korselt-criterion.md):

$$
\boxed{n\text{ is Carmichael}\ \Longleftrightarrow\
n\text{ is composite and squarefree, and }p-1\mid n-1\text{ for all }p\mid n.}
$$

If $n=pq$ for distinct odd [primes](../../../../../prime-number.md) with $p<q$, the condition at $q$ would require $q-1\mid pq-1$. Reducing $p q-1$ modulo $q-1$ gives $p-1$, so $q-1\mid p-1$. But $0<p-1<q-1$, which is impossible. Thus **a product of two distinct odd [primes](../../../../../prime-number.md) is not Carmichael**.

For $n=pqr$, squarefreeness is automatic. Since $p\equiv1\pmod{p-1}$,

$$
pqr-1\equiv qr-1\pmod{p-1}.
$$

Apply the analogous reductions at $q$ and $r$ to obtain

$$
\boxed{pqr\text{ is Carmichael}\ \Longleftrightarrow\
p-1\mid qr-1,\quad q-1\mid pr-1,\quad r-1\mid pq-1.}
$$

Finally $1729=7\cdot13\cdot19$, with distinct odd [prime factors](../../../../../prime-factor.md), and

$$
13\cdot19-1=246=6\cdot41,\qquad
7\cdot19-1=132=12\cdot11,\qquad
7\cdot13-1=90=18\cdot5.
$$

All three divisibilities hold, so **1729 is a Carmichael number**.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
