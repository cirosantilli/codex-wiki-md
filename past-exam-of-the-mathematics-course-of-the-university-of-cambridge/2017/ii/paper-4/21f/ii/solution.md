<h1 id="21f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $A=T^*T$. Then $A^*=T^*T$ and $(x,Ax)=\|Tx\|^2\geq0$, with the [inner product](../../../../../../inner-product.md) linear in its second argument as required by the later SVD formula. For nonreal $\lambda$, self-adjointness gives $\|(A-\lambda I)x\|\geq|\operatorname{Im}\lambda|\|x\|$. For $\lambda=-a<0$, positivity gives $\|(A+aI)x\|\geq a\|x\|$. These bounds give injectivity and closed range. The range is dense because its [orthogonal complement](../../../../../../orthogonal-complement.md) is the kernel of the adjoint, to which the same bound applies. Thus the range is all of $H$ and the inverse is bounded in either case. Consequently

$$
\boxed{A=T^*T\text{ is self-adjoint},\qquad\sigma(A)\subseteq[0,\infty).}
$$

If $T$ is compact, composition of the [compact operator](../../../../../../compact-operator-split.md) $T$ with bounded $T^*$ is compact, so $T^*T$ is compact too.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [21F](../../21f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
