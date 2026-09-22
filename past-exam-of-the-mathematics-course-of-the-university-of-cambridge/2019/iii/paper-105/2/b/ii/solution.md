<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the product [Hilbert space](../../../../../../../hilbert-space-split.md) $H=H_0^1(U)\times H^1(U)$ define

$$
B((u,w),(v,z))
=\int_U\bigl(Du\mathbin\cdot Dv+uv+wv+Dw\mathbin\cdot Dz+wz-3uz\bigr)
$$

and

$$
F(v,z)=\int_U(fv+gz).
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) makes $B$ and $F$ bounded. On the diagonal,

$$
B((u,w),(u,w))
=\|Du\|_2^2+\|Dw\|_2^2+\|u-w\|_2^2.
$$

The [Poincaré inequality](../../../../../../../poincare-inequality.md) controls $\|u\|_2$ by $\|Du\|_2$, and

$$
\|w\|_2\leq\|w-u\|_2+\|u\|_2.
$$

The displayed diagonal value therefore controls the full product $H^1$ norm, so $B$ is [coercive](../../../../../../../coercive-bilinear-form.md). The [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md) now gives exactly one pair $(u,w)\in H$ satisfying the weak identities. Hence **a unique weak solution exists for every $f,g\in L^2(U)$**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
