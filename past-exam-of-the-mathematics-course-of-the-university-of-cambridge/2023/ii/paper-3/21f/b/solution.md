<h1 id="21f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
A=\bigcap_{n=1}^\infty U_n
$$

with each $U_n$ open. The closed sets $A$ and $X\setminus U_n$ are disjoint. By the [Urysohn lemma](../../../../../../urysohn-s-lemma.md), choose a continuous $f_n:X\to[0,1]$ with

$$
f_n=0\text{ on }A,
\qquad
f_n=1\text{ on }X\setminus U_n.
$$

The uniformly convergent series

$$
f(x)=\sum_{n=1}^\infty2^{-n}f_n(x)
$$

defines a continuous map to $[0,1]$. It vanishes on $A$. If $x\notin A$, then $x\notin U_n$ for some $n$, so $f_n(x)=1$ and $f(x)>0$. Thus

$$
\boxed{f^{-1}(0)=A,}
$$

which is the [closed G-delta set as a zero set](../../../../../../closed-g-delta-set-as-a-zero-set.md) construction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21F](../../21f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
