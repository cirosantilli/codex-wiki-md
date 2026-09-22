<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The multiplication gives $v_1=1_A$ and $v_2^2+3v_2+2v_1=0$. Since $v_1,v_2$ form a [basis](../../../../../basis.md),

$$
A\cong\mathbb C[t]/((t+1)(t+2))\cong\mathbb C\times\mathbb C
$$

by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md). Thus there are exactly **two nonisomorphic simple [modules](../../../../../module-mathematics.md)**, both one-dimensional. With basis vectors $s_{-1},s_{-2}$ their actions are

$$
\boxed{v_1s_{-1}=s_{-1},\quad v_2s_{-1}=-s_{-1};\qquad v_1s_{-2}=s_{-2},\quad v_2s_{-2}=-2s_{-2}.}
$$

The two orthogonal primitive [idempotents](../../../../../idempotent.md) are $e_{-1}=2v_1+v_2$ and $e_{-2}=-v_1-v_2$. They sum to $v_1$ and span the two simple ideals. Consequently the regular [module](../../../../../module-mathematics.md) splits as $A=\mathbb Ce_{-1}\oplus\mathbb Ce_{-2}$, so **$A$ is semisimple**.

Its complete list of [composition series](../../../../../composition-series.md) is

$$
\boxed{0<\mathbb C(2v_1+v_2)<A,\qquad0<\mathbb C(v_1+v_2)<A.}
$$

Indeed every proper nonzero submodule has dimension one and is an invariant line for multiplication by $v_2$. The matrix $\begin{pmatrix}0&-2\\1&-3\end{pmatrix}$ has the two distinct eigenvalues $-1,-2$, so these are exactly its two invariant lines.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the algebra course of the University of Oxford](../../../../split.md)
6. [Algebra course of the University of Oxford](../../../../../algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
