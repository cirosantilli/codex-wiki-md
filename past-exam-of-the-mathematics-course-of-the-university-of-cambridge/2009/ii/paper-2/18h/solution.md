<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

For the first [polynomial](../../../../../polynomial-split.md), put $\alpha=\sqrt{1+\sqrt{26}}$ and $\beta=5i/\alpha$, so that $\beta^2=1-\sqrt{26}$. The roots are $\pm\alpha,\pm\beta$, and

$$
\boxed{K=\mathbb Q(\alpha,i),\qquad G\cong D_4\text{ of order }8.}
$$

To justify the degree, a rational quadratic factorization would have the form $(x^2+ux+v)(x^2-ux+w)$. The vanishing linear coefficient implies either $u=0$ or $v=w$. The former requires $v,w=-1\pm\sqrt{26}$, not rational, while the latter requires $v^2=-25$, also impossible over $\mathbb Q$. There is no rational root, since its square would have to be $1\pm\sqrt{26}$, so the [polynomial](../../../../../polynomial-split.md) is irreducible. The real field $\mathbb Q(\alpha)$ has degree four and does not contain $i$, giving degree eight after adjoining it. The group acts transitively on the four roots while preserving their two opposite pairs, so is contained in the square's [dihedral group](../../../../../dihedral-group.md) of order eight; the degree makes it the full group.

For the second [polynomial](../../../../../polynomial-split.md), choose $\alpha=\sqrt3+i\sqrt2$ and $\beta=\sqrt3-i\sqrt2$. Then $\alpha^2=1+2i\sqrt6$, $\beta^2=1-2i\sqrt6$ and $\alpha\beta=5$. Its four roots generate

$$
\boxed{K=\mathbb Q(\sqrt3,\sqrt{-2}),\qquad G\cong C_2\times C_2.}
$$

Indeed $\alpha+\beta=2\sqrt3$ and $\alpha-\beta=2\sqrt{-2}$ recover both generators. The real quadratic field $\mathbb Q(\sqrt3)$ cannot contain $\sqrt{-2}$, so the degree is four. Independent changes of the two square-root signs give all four [automorphisms](../../../../../automorphism.md).

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
