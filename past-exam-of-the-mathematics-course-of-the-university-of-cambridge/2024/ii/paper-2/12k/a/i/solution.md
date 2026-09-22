<h1 id="12k/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the [Rabin cryptosystem](../../../../../../../rabin-cryptosystem.md), the public key is $N=pq$, usually with distinct secret primes $p,q\equiv3\pmod4$. A message $m$ is encrypted as

$$
c\equiv m^2\pmod N.
$$

Knowing $p$ and $q$, the receiver finds the two square roots of $c$ modulo each prime and combines them by the Chinese remainder theorem, obtaining the four square roots modulo $N$; redundancy identifies the intended message.

Factoring $N$ plainly enables this decryption. Conversely, suppose an algorithm returns a square root of a chosen quadratic residue. Choose random invertible $x$, submit $x^2\bmod N$, and receive a root $y$. With probability at least $1/2$, $y\not\equiv\pm x\pmod N$; then

$$
\gcd(x-y,N)\quad\hbox{or}\quad\gcd(x+y,N)
$$

is a nontrivial factor. Thus decryption and factoring are equivalent up to a randomized polynomial-time reduction.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [12K](../../../12k.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
