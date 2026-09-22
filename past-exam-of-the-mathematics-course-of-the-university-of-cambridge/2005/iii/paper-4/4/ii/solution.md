<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $D=\operatorname{ad}x$, and choose $N$ with $D^N=0$. The [exponential of a nilpotent Lie algebra derivation](../../../../../../exponential-of-a-nilpotent-lie-algebra-derivation.md) is the finite [linear operator](../../../../../../linear-operator.md)

$$
E=\exp D=\sum_{j=0}^{N-1}\frac{D^j}{j!}.
$$

For a [derivation of a Lie algebra](../../../../../../derivation-of-a-lie-algebra.md), induction on $k$ using the Leibniz rule and Pascal's identity proves

$$
D^k[y,z]=\sum_{j=0}^k\binom{k}{j}[D^jy,D^{k-j}z].
$$

Expanding $[Ey,Ez]$ and grouping by $k=j+l$ consequently gives

$$
[Ey,Ez]=\sum_{k=0}^{2N-2}\frac1{k!}\sum_{j=0}^k\binom{k}{j}[D^jy,D^{k-j}z]
=\sum_{k=0}^{2N-2}\frac{D^k[y,z]}{k!}=E[y,z].
$$

Terms with an exponent at least $N$ vanish, which justifies extending each inner sum; and $D^k=0$ for $k\ge N$. Finally the finite product of the two exponentials has coefficient

$$
[D^k]\bigl(\exp D\exp(-D)\bigr)=\sum_{j=0}^k\frac{(-1)^{k-j}}{j!(k-j)!}=\frac{(1-1)^k}{k!},
$$

so $\exp(-D)$ is the inverse. We have proved bracket preservation and invertibility, hence **$\exp(\operatorname{ad}x)$ is a Lie algebra automorphism**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
