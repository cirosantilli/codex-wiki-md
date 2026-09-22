<h1 id="11i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an odd prime $p$, the [Legendre symbol](../../../../../../legendre-symbol.md) is

$$
\left(\frac ap\right)
=
\begin{cases}
0,&p\mid a,\\
1,&a\not\equiv0\pmod p\text{ is a square},\\
-1,&a\text{ is a nonsquare}.
\end{cases}
$$

[Euler criterion](../../../../../../euler-criterion.md) states that

$$
a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.
$$

The [Gauss lemma](../../../../../../gauss-s-lemma-number-theory.md) says that, for $p\nmid a$, if $m$ of the least positive residues of

$$
a,2a,\ldots,\frac{p-1}{2}a
$$

lie in $(p/2,p)$, then

$$
\left(\frac ap\right)=(-1)^m.
$$

To prove it, replace every residue above $p/2$ by its negative. The resulting absolute residues are distinct up to sign and therefore form a permutation of

$$
1,2,\ldots,\frac{p-1}{2}.
$$

Multiplying the congruences gives

$$
a^{(p-1)/2}\left(\frac{p-1}{2}\right)!
\equiv
(-1)^m\left(\frac{p-1}{2}\right)!
\pmod p.
$$

Cancel the nonzero factorial and apply Euler's criterion.

For $a=2$, the residues are $2,4,\ldots,p-1$. The number above $p/2$ is

$$
m=\frac{p-1}{2}-\left\lfloor\frac p4\right\rfloor,
$$

whose parity gives the [second supplementary law for quadratic reciprocity](../../../../../../second-supplementary-law-for-quadratic-reciprocity.md)

$$
\left(\frac2p\right)
=(-1)^{(p^2-1)/8}.
$$

Consequently, for odd primes,

$$
\boxed{x^2\equiv2\pmod p
\quad\Longleftrightarrow\quad
p\equiv1\text{ or }7\pmod8}.
$$

The congruence is also soluble for $p=2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11I](../../11i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
