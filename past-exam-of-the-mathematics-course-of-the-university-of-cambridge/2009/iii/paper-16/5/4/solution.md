<h1 id="5/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**True: every integer occurs.** The simple-connectivity assumptions in parts 1 and 2 are local to those statements and are not imposed here. For a connected closed oriented four-manifold, [Poincare duality](../../../../../../poincare-duality.md) gives

$$
\chi(M)=1-b_1+b_2-b_3+1=2-2b_1+b_2,
$$

since $b_3=b_1$. This expression has no fixed sign or parity.

Use $\chi(\mathbb{CP}^2)=3$, from its three even-dimensional cells, and $\chi(S^1\times S^3)=0$, by [Euler characteristic of a product](../../../../../../euler-characteristic-of-a-product.md). The [Euler characteristic of a connected sum](../../../../../../euler-characteristic-of-a-connected-sum.md) in dimension four is

$$
\chi(A\#B)=\chi(A)+\chi(B)-2.
$$

It follows either by [Mayer–Vietoris sequence](../../../../../../mayer-vietoris-sequence.md) after deleting balls, or by the intermediate-degree cohomology splitting and the single top and bottom generators. Therefore a [connected sum](../../../../../../connected-sum-of-oriented-manifolds.md) of $r$ projective planes and $s$ copies of $S^1\times S^3$ has

$$
\chi=2+r-2s.
$$

Given an integer $h$, choose an integer $s\geq\max\{0,\lceil(2-h)/2\rceil\}$ and put $r=h-2+2s\geq0$. This produces a connected closed oriented four-manifold of [Euler characteristic](../../../../../../euler-characteristic.md) $h$. When $r=s=0$, use $S^4$. Thus

$$
\boxed{\{\chi(M):M\text{ connected, closed, oriented, }\dim M=4\}=\mathbb Z.}
$$

If simple connectivity were added, the possible values would instead satisfy $\chi=2+b_2\geq2$. This distinction is recorded in [Euler characteristics of closed oriented four-manifolds](../../../../../../euler-characteristics-of-closed-oriented-four-manifolds.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
