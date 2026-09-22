<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

[Liouville approximation theorem](../../../../../liouville-approximation-theorem.md) states that if an irrational algebraic number $\alpha$ has degree $d\geq2$, then some $C(\alpha)>0$ satisfies

$$
\left|\alpha-\frac pq\right|>\frac{C(\alpha)}{q^d}
$$

for every rational $p/q$ with $q>0$.

The omitted $n=0$ term is rational and does not affect transcendence. Let

$$
\xi=\sum_{n\geq1}10^{-n^n},\qquad
\xi_N=\sum_{n=1}^N10^{-n^n}=\frac{p_N}{q_N},\quad q_N=10^{N^N}.
$$

The decimal expansion has ones at the increasingly separated positions $n^n$ and zeros elsewhere, so it is not eventually periodic and $\xi$ is irrational. Moreover,

$$
0<\xi-\xi_N<2\,10^{-(N+1)^{N+1}}.
$$

For every fixed $d$, the exponent $(N+1)^{N+1}$ eventually exceeds $dN^N$ by an arbitrarily large amount, so this upper bound is smaller than $Cq_N^{-d}$. Liouville's theorem therefore rules out every finite algebraic degree, proving that $\xi$ is transcendental.

There are only countably many integer [polynomials](../../../../../polynomial-split.md) and each has finitely many roots, so the algebraic numbers are countable. Since $\mathbb R$ is uncountable, its complement, the set of transcendental numbers, is uncountable.

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
