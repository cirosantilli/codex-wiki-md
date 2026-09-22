<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A simple-root version of [Hensel lemma](../../../../../../hensel-s-lemma.md) is: if $R$ is a complete [discrete valuation ring](../../../../../../discrete-valuation-ring.md), $f\in R[T]$, $f(a_1)\equiv0\pmod\pi$, and $f'(a_1)$ is a unit, then there is a unique root $a\in R$ congruent to $a_1$ modulo $\pi$.

Suppose $f(a_n)\in\pi^nR$. The derivative remains a unit, so choose a residue $c_n$ satisfying

$$
\frac{f(a_n)}{\pi^n}+c_nf'(a_n)\equiv0\pmod\pi,
$$

and put $a_{n+1}=a_n+c_n\pi^n$. Taylor expansion gives $f(a_{n+1})\equiv f(a_n)+c_n\pi^nf'(a_n)\pmod{\pi^{n+1}}$, because $2n\ge n+1$. Thus $f(a_{n+1})\in\pi^{n+1}R$. The sequence is a [Cauchy sequence](../../../../../../cauchy-sequence.md) and converges by completeness; continuity of polynomial evaluation makes its limit a root.

If roots $a,b$ have the prescribed residue, factor $f(a)-f(b)=(a-b)Q(a,b)$. Modulo $\pi$, the second factor is $f'(a_1)$, so it is a unit. Therefore $a=b$. This is the [simple-root Hensel lifting by successive residues](../../../../../../simple-root-hensel-lifting-by-successive-residues.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
