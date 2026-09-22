<h1 id="9h/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True.** First suppose $p^e\mid N$ with $e\geq2$ maximal. By the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md), choose $a\equiv1+p^{e-1}\pmod{p^e}$ and $a\equiv1$ modulo all other prime-power factors. This is a unit, with [Jacobi symbol](../../../../../../jacobi-symbol.md) one, because it is one modulo every prime. For $m=(N-1)/2$, the [binomial theorem](../../../../../../binomial-theorem.md) gives

$$
a^m\equiv1+mp^{e-1}\not\equiv1\pmod{p^e},
$$

because $p\nmid m$ and all higher terms contain $p^e$. It is therefore a witness to the desired failure.

If $N$ is square-free and composite, it has at least two prime factors. Choose $a$ to be a [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) at one prime $p$ and one at every other prime, again using the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md). Then $(a/N)=-1$. At a different odd prime $q\mid N$, however, $a^m\equiv1\not\equiv-1\pmod q$. These two cases prove that **every odd composite has an Euler-Jacobi witness**, unlike the situation for the ordinary [Fermat primality test](../../../../../../fermat-primality-test.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [9H](../../9h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
