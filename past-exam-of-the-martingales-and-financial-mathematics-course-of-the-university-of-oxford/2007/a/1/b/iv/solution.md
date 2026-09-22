<h1 id="a/1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $x\in M$, let $k$ be the unique index such that $g(x)\in B_{n,k}$. Then $f(x)\in A_{n,k}$ and $h_n(f(x))=k2^{-n}$. The chosen interval is open on the left and closed on the right, so

$$
\boxed{0<g(x)-h_n(f(x))\leq2^{-n}.}
$$

This remains correct at dyadic endpoints; changing it to a floor approximation with a non-strict left endpoint would describe a different approximation.

By part (iii), define the finite limit $h(t)=\lim_n h_n(t)$ for every $t\in\mathbb R$. Part (a) makes this limit [Borel measurable](../../../../../../borel-measurable-function.md). Letting $n\to\infty$ in the displayed error bound gives

$$
\boxed{g=h\circ f.}
$$

This is the factorization conclusion of the [Doob-Dynkin lemma](../../../../../../doob-dynkin-lemma.md) under the specified Borel-image hypothesis.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
