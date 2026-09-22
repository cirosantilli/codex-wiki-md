<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One form of the [Hensel lemma](../../../../../../hensel-s-lemma.md) is the following. Let $R$ be a complete [discrete valuation ring](../../../../../../discrete-valuation-ring.md) with maximal ideal $\mathfrak m$, and let $f\in R[X]$. If $a_0\in R$ satisfies

$$
f(a_0)\equiv0\pmod{\mathfrak m},
\qquad f'(a_0)\not\equiv0\pmod{\mathfrak m},
$$

then there is a unique $a\in R$ with $f(a)=0$ and $a\equiv a_0\pmod{\mathfrak m}$.

Define $a_{n+1}=a_n-f(a_n)/f'(a_n)$. Since $f'(a_n)$ remains a unit, Taylor expansion gives

$$
f(a_{n+1})\equiv0\pmod{f(a_n)^2},
$$

so the valuations of the errors at least double. The corrections tend to zero, making $(a_n)$ a [Cauchy sequence](../../../../../../cauchy-sequence.md); completeness gives a limit $a$, and continuity gives $f(a)=0$. If $a,b$ are two such roots, then

$$
0=f(a)-f(b)=(a-b)(f'(a_0)+u)
$$

with $u\in\mathfrak m$, so the second factor is a unit and $a=b$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
