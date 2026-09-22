<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

For

$$
A=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in GL_2(F),
$$

define its action on the [projective line](../../../../../projective-line.md) $F\cup\{\infty\}$ by the [Möbius transformation](../../../../../mobius-transformation.md)

$$
A\cdot x=\frac{ax+b}{cx+d},
$$

with the usual conventions when the denominator vanishes or $x=\infty$. [Matrix](../../../../../matrix.md) multiplication agrees with composition, so this is a [group action](../../../../../group-action.md). If $A$ fixes every projective point, then it fixes $0$ and $\infty$, forcing $b=c=0$, and fixing $1$ then gives $a=d$. Thus the kernel consists exactly of the nonzero [scalar](../../../../../scalar.md) [matrices](../../../../../matrix.md) $Z$. The induced [group homomorphism](../../../../../group-homomorphism.md)

$$
\phi:GL_2(F)/Z\longrightarrow S_{q+1}
$$

is therefore injective. This is the [projective general linear group action on the projective line](../../../../../projective-general-linear-group-action-on-the-projective-line.md).

For $F=\mathbb F_4$,

$$
|GL_2(\mathbb F_4)|
=(4^2-1)(4^2-4)=15\cdot12=180.
$$

The [scalar](../../../../../scalar.md) [subgroup](../../../../../subgroup.md) has order $|Z|=3$, so

$$
|G|=60.
$$

The four classes represented by

$$
\begin{pmatrix}1&b\\0&1\end{pmatrix},
\qquad b\in\mathbb F_4,
$$

form a [subgroup](../../../../../subgroup.md) $P$ of order four, hence a [Sylow subgroup](../../../../../sylow-subgroup.md) for the prime two. Its action is translation $x\mapsto x+b$ on $\mathbb F_4$ and fixes $\infty$. For $b\ne0$, characteristic two makes this permutation a product of two disjoint transpositions on the four finite points. It is therefore even, and

$$
\boxed{\phi(P)\leq A_5}.
$$

This realizes the [Sylow 2-subgroup of PGL2 over F4](../../../../../sylow-2-subgroup-of-pgl2-over-f4.md).

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
