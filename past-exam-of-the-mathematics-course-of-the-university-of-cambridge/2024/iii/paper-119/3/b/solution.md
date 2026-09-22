<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $[A,B]$ be the set of arbitrary-join-preserving maps $A\to B$, ordered pointwise. Pointwise joins remain join-preserving because the two joins may be interchanged:

$$
\left(\bigvee_i f_i\right)\left(\bigvee_j a_j\right)
=\bigvee_{i,j}f_i(a_j).
$$

Precomposition and postcomposition preserve these joins, so $(A,B)\mapsto[A,B]$ is the required $\mathbf{CSLat}$-valued hom functor.

Sending $f:A\to B$ to its right adjoint gives

$$
[B^*,A^*]\cong[A,B].
$$

It is order-preserving because taking a right adjoint reverses pointwise order once, while the order on $A^*$ reverses it again.

A join map $\chi_a:A\to2$ is associated with $a\in A$ by

$$
\chi_a(x)=0\Longleftrightarrow x\leq a.
$$

Every join map to $2$ is of this form, and $a\mapsto\chi_a$ identifies $A^*$ with $[A,2]$. Finally, a map $A\to[B,C]$ is a function $A\times B\to C$ preserving arbitrary joins separately in each variable. Swapping the variables gives naturally

$$
\boxed{[A,[B,C]]\cong[B,[A,C]].}
$$

The assumed expression of $C$ as a limit of copies of $2$ reduces the verification to the preceding $2$-valued description.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
