# Truncated binomial cube root of the identity plus a nilpotent matrix

↑ **Parent:** [Nilpotent matrix](nilpotent-matrix.md)

Over the [complex numbers](complex-number.md), if $N^m=0$, then

$$
Q=\sum_{j=0}^{m-1}\binom{1/3}{j}N^j,\qquad Q^3=I+N.
$$

Here the generalized [binomial coefficient](binomial-coefficient-split.md) is $\binom{\alpha}{j}=\alpha(\alpha-1)\cdots(\alpha-j+1)/j!$, with $\binom{\alpha}{0}=1$. This is an exact finite identity, even when an infinite [binomial series](binomial-series.md) would not converge.

One can construct the required [polynomial](polynomial-split.md) $q(z)=1+\sum_{j=1}^{m-1}c_jz^j$ without any infinite series. At [polynomial degree](degree-of-a-polynomial.md) $j$, the [coefficient](coefficient.md) of $q(z)^3$ is $3c_j$ plus terms involving only earlier [coefficients](coefficient.md). Recursively choose it to agree with $1+z$ through [polynomial degree](degree-of-a-polynomial.md) $m-1$; the first [coefficients](coefficient.md) are $1/3,-1/9,5/81$. The stated generalized [binomial coefficients](binomial-coefficient-split.md) solve this recursion: near $z=0$, the [binomial series](binomial-series.md) for $(1+z)^{1/3}$ cubes to $1+z$, and truncating it changes no [coefficient](coefficient.md) below [polynomial degree](degree-of-a-polynomial.md) $m$. Thus $q(z)^3-(1+z)$ is divisible by $z^m$ as a [polynomial identity](polynomial-identity.md). Substituting the [nilpotent matrix](nilpotent-matrix.md) $N$ kills the remaining terms, all divisible by $N^m$. For a [Jordan block](jordan-block.md) $\lambda I+N$ with $\lambda\ne0$, replace $N$ by $N/\lambda$ and multiply $Q$ by a scalar [cube root](cube-root.md) of $\lambda$.

## ↑ Ancestors (8)

1. [Nilpotent matrix](nilpotent-matrix.md)
2. [Nilpotent linear map](nilpotent-linear-map.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cube root of a matrix](cube-root-of-a-matrix.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2021/2/c/i/solution.md)
