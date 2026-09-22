<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

For odd $N>1$ coprime to $b$, the [Fermat pseudoprime](../../../../../fermat-pseudoprime.md) test is $b^{N-1}\equiv1\pmod N$. The [Euler pseudoprime](../../../../../euler-pseudoprime.md) test meant here is the Euler–Jacobi test,

$$
b^{(N-1)/2}\equiv\left(\frac bN\right)\pmod N,
$$

where the right side is the [Jacobi symbol](../../../../../jacobi-symbol.md). Write $N-1=2^sd$, with $d$ odd. The [strong pseudoprime](../../../../../strong-pseudoprime.md) test passes when $b^d\equiv1$, or when $b^{2^jd}\equiv-1$ for some $0\le j<s$. Terminology often reserves “pseudoprime” for composite numbers; the question uses it for passing the respective test, including primes.

For the final example, $341=11\cdot31$ is composite and $2^{10}=1024\equiv1\pmod{341}$, so $2^{340}\equiv1$. It passes the [Fermat primality test](../../../../../fermat-primality-test.md). However $2^{170}\equiv1$, whereas the supplementary law for the [Jacobi symbol](../../../../../jacobi-symbol.md) gives $(2/341)=-1$ since $341\equiv5\pmod8$. Thus **341 is Fermat but not Euler–Jacobi pseudoprime to base two**. A weaker convention defining an Euler test merely by $b^{(N-1)/2}=\pm1$ would not give the claimed distinction, which is why the Jacobi convention matters.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
