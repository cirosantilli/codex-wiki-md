<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Clifford algebra](../../../../../../clifford-algebra.md) relation implies

$$
[C(a)C(b),C(v)]=2(b,v)C(a)-2(a,v)C(b).
$$

Indeed move $C(v)$ past $C(b)$ and then past $C(a)$ using the two anticommutator identities; the three-generator products cancel.

Since all $C(w)$ are [self-adjoint](../../../../../../self-adjoint-operator.md),

$$
\pi(T)^*+\pi(T)=\frac14\sum_i\bigl(C(e_i)C(Te_i)+C(Te_i)C(e_i)\bigr)
=\frac12\sum_i(e_i,Te_i)I=0.
$$

Each scalar vanishes because $T$ is [skew-adjoint](../../../../../../skew-adjoint-generator.md). This proves $\boxed{\pi(T)^*=-\pi(T)}$.

For the requested [commutator](../../../../../../commutator.md), the first identity gives

$$
[\pi(T),C(v)]=\frac12\sum_i\bigl((e_i,v)C(Te_i)-(Te_i,v)C(e_i)\bigr).
$$

The first sum is $C(Tv)$ by the [orthonormal basis](../../../../../../orthonormal-basis.md) expansion of $v$. For the second, the [skew-adjoint](../../../../../../skew-adjoint-generator.md) property gives $\sum_i(Te_i,v)e_i=-Tv$. By real linearity of $C$, the difference is therefore

$$
\boxed{[\pi(T),C(v)]=\tfrac12(C(Tv)-C(-Tv))=C(Tv).}
$$

This calculation explains the factor $1/4$: it makes infinitesimal rotations of $V$ act correctly on its Clifford generators.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
