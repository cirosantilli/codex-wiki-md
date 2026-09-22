<h1 id="12k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [Rabin cryptosystem](../../../../../../rabin-cryptosystem.md), the public key is $N=pq$ and encryption sends an encoded message $m$ to

$$
c\equiv m^2\pmod N.
$$

Knowing $p,q$, the receiver finds the two square roots modulo each prime and combines them with the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) to obtain four roots modulo $N$; prescribed redundancy identifies the intended one.

Omicron has

$$
m^2\equiv c\pmod N,\qquad m^2\equiv c'\pmod{N'}.
$$

The Chinese remainder theorem determines $m^2$ uniquely modulo $NN'$ (assuming the independently generated moduli are coprime; a nontrivial gcd would itself factor them). Since $1\leq m<N<N'$, one has $m^2<NN'$, so this residue is the ordinary integer $m^2$. Taking its positive integer square root recovers $m$.

This does not normally decrypt another ciphertext sent under only one modulus. The recovered pair reveals no nontrivial square root collision modulo that modulus and hence supplies no factorization; breaking a single Rabin instance remains equivalent to factoring its modulus.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12K](../../12k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
