<h1 id="37e/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Krylov subspace](../../../../../../../krylov-subspace.md) is $K_m(A,v)=\operatorname{span}\{v,Av,\ldots,A^{m-1}v\}$. Let $s$ be the first index for which $A^s v$ depends linearly on $v,\ldots,A^{s-1}v$. Such an index exists with $1\leq s\leq n$, since $v\ne0$ and any $n+1$ vectors are dependent. The first $s$ vectors are independent. The relation for $A^sv$ shows that their span is invariant under $A$: multiplying any generator by $A$ stays in that span. Repeated multiplication makes every higher power stay there too. Therefore

$$
\boxed{\dim K_m=m\ (m\leq s),\qquad\dim K_m=s\ (m>s).}
$$

Once a [Krylov subspace](../../../../../../../krylov-subspace.md) stops growing, it cannot resume growth.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [37E](../../../37e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
