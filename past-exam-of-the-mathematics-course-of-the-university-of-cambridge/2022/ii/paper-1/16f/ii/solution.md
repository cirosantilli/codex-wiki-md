<h1 id="16f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $f:X\to A\subseteq Y$ be an order isomorphism onto a down-set, and let $g:Y\to U=X\setminus B$ be an order isomorphism onto the complement of a down-set $B$. Define increasing down-sets

$$
D_0=B,
\qquad D_{n+1}=B\cup g(f(D_n)),
\qquad D=\bigcup_{n\geq0}D_n.
$$

The order assumptions ensure inductively that each $D_n$ is a down-set. Define

$$
h(x)=
\begin{cases}
f(x),&x\in D,\\g^{-1}(x),&x\notin D.
\end{cases}
$$

The usual [Cantor-Schröder-Bernstein theorem](../../../../../../cantor-schroder-bernstein-theorem.md) orbit argument shows that these two pieces partition both domain and codomain bijectively: points generated from $B$ move forward through $f$, while every remaining point lies in $U$ and moves backward through $g$. Each branch preserves order. If $x\in D$ and $x'<x$ then $x'\in D$; hence the only mixed case has $x\notin D<x'\in D$, and the initial/final-segment hypotheses put $h(x)<h(x')$. Thus $h$ is an order isomorphism and

$$
\boxed{X\cong Y}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [16F](../../16f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
