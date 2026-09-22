<h1 id="11g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $H=(p-1)/2$. Because $p\equiv7\pmod8$, the supplementary laws give

$$
\left(\frac{-1}{p}\right)=-1,
\qquad
\left(\frac2p\right)=1.
$$

Let $R$ and $N$ be the quadratic residues and nonresidues, respectively, among $1,\ldots,H$, and put

$$
S=\sum_{r\in R}r.
$$

Since $-1$ is a nonresidue, the complete set $Q$ of least positive quadratic residues is

$$
Q=R\cup\{p-n:n\in N\}.
$$

If $u=|N|$, its sum is

$$
\sum_{q\in Q}q
=S+up-\sum_{n\in N}n
=2S+up-\frac{H(H+1)}2.
$$

Since $2$ is a residue, multiplication by two permutes $Q$ modulo $p$. Exactly the $u$ upper-half residues $p-n$ cross $p$ when doubled. Equality of the sums before and after reduction therefore gives

$$
\sum_{q\in Q}q
=2\sum_{q\in Q}q-up,
\qquad
\sum_{q\in Q}q=up.
$$

Comparing the two formulas yields

$$
2S=\frac{H(H+1)}2.
$$

As $H=(p-1)/2$,

$$
\boxed{
S=\frac{H(H+1)}4=\frac{p^2-1}{16}.}
$$

This is the [lower-half quadratic-residue sum for primes congruent to seven modulo eight](../../../../../../lower-half-quadratic-residue-sum-for-primes-congruent-to-seven-modulo-eight.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
