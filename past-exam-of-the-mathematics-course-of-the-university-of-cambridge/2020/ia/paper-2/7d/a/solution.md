<h1 id="7d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Euler totient function](../../../../../../euler-totient-function.md) $\phi(n)$ is the number of residue classes modulo $n$ that are coprime to $n$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) says that for pairwise coprime moduli $m_i$, reduction induces a bijection

$$
\mathbb Z/(m_1\cdots m_r)\mathbb Z
\longrightarrow\prod_{i=1}^r\mathbb Z/m_i\mathbb Z.
$$

It restricts to a bijection of unit groups. If $n=p_1\cdots p_r$ is squarefree, then

$$
\boxed{\phi(n)=\prod_{i=1}^r(p_i-1)}.
$$

Each of the primes $3,5,17,257$ is one more than a power of two, so every squarefree product of them has power-of-two totient. Ten odd examples are

$$
\boxed{3,5,15,17,51,85,255,257,771,1285}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7D](../../7d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
