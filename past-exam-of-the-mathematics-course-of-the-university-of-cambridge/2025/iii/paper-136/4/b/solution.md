<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [local factorization and extended absolute values](../../../../../../local-factorization-and-extended-absolute-values.md), extensions of $|\cdot|_p$ to the number field $L=\mathbb Q(\alpha)$ correspond to the irreducible factors of $X^3-2$ over $\mathbb Q_p$.

For $p=2$, the polynomial is Eisenstein, hence irreducible, so there is one extension. For $p=3$, a root would be a unit $x$ with $x\equiv-1\pmod3$, but then $x^3\equiv-1\equiv8\pmod9$, not $2\pmod9$. A reducible cubic has a root, so the polynomial is again irreducible and there is one extension.

For $p=5$, reduction gives

$$
X^3-2=(X-3)(X^2+3X+4)\pmod5.
$$

The factors are coprime, and the quadratic has discriminant $3$, a nonsquare modulo $5$. [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts this as one linear and one irreducible quadratic factor over $\mathbb Q_5$, giving two extensions. The requested numbers are therefore

$$
\boxed{1,1,2}
$$

for $p=2,3,5$, respectively.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
