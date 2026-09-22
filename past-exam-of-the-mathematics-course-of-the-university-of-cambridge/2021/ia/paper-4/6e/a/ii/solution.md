<h1 id="6e/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because $\gcd(m,n)=1$, choose $u,v\in\mathbb Z$ with $um+vn=1$ by [Bézout's identity](../../../../../../../bezout-identity.md). Then

$$
c=avn+bum
$$

satisfies $c\equiv a\pmod m$ and $c\equiv b\pmod n$. Any two simultaneous solutions differ by a multiple of both coprime integers and hence by a multiple of $mn$. This proves the two-modulus [Chinese remainder theorem](../../../../../../../chinese-remainder-theorem.md).

The three congruences reduce to

$$
x\equiv2\pmod5,
\qquad x\equiv3\pmod7,
\qquad x\equiv1\pmod3.
$$

The first two give $x\equiv17\pmod{35}$; imposing the last gives

$$
\boxed{x\equiv52\pmod{105}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6E](../../../6e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
