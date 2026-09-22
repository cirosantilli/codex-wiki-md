<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

For an odd composite $N$ and a unit $b$ modulo $N$, $N$ is a [Fermat pseudoprime](../../../../../fermat-pseudoprime.md) to base $b$ when

$$
b^{N-1}\equiv1\pmod N.
$$

It is an [Euler pseudoprime](../../../../../euler-pseudoprime.md) to base $b$ when

$$
b^{(N-1)/2}\equiv\left(\frac bN\right)\pmod N,
$$

where the right side is the Jacobi symbol.

By the Chinese remainder theorem,

$$
(\mathbb Z/105\mathbb Z)^\times
\cong(\mathbb Z/3\mathbb Z)^\times
\times(\mathbb Z/5\mathbb Z)^\times
\times(\mathbb Z/7\mathbb Z)^\times,
$$

and $\varphi(105)=2\cdot4\cdot6=48$. The condition $b^{104}=1$ is automatic modulo $3$ and $5$. Modulo $7$ it has

$$
\gcd(104,6)=2
$$

solutions. Thus there are $2\cdot4\cdot2=16$ Fermat [bases](../../../../../basis.md), giving proportion

$$
\boxed{\frac{16}{48}=\frac13}.
$$

For the Euler condition, $b^{52}=1$ modulo $3$, so the Jacobi symbol must be $+1$. The power condition is automatic modulo $5$, while modulo $7$ it again restricts $b$ to the two solutions of $b^2=1$. For each of those two residues, exactly half of the $2\cdot4$ choices modulo $3$ and $5$ have Jacobi symbol $+1$. Hence there are $2\cdot4=8$ Euler [bases](../../../../../basis.md) and proportion

$$
\boxed{\frac8{48}=\frac16}.
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
