<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

A [Rabin cryptosystem](../../../../../rabin-cryptosystem.md) chooses Blum primes $p,q$, publishes $N=pq$, and encrypts $m$ as $c=m^2\bmod N$. Decryption takes square roots modulo $p$ and $q$, combines them with CRT, and uses redundancy to select the intended one of four roots. Here $2355^2\equiv25\pmod{2773}$, while the obvious root is $5$. Thus

$$
\gcd(2355-5,2773)=47,\qquad\gcd(2355+5,2773)=59.
$$

So $2773=47\cdot59$ is factored, allowing all future square roots and hence all ciphertexts to be decrypted.

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
