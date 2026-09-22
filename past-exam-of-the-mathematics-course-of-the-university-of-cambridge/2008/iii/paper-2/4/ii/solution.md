<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $R=\langle\!\langle r_j:j\in J\rangle\!\rangle_F$ and let $\pi:F\to G_0=F/R$ be the quotient [group homomorphism](../../../../../../group-homomorphism.md). The subgroup in the question is exactly the [fiber product of groups](../../../../../../fiber-product-of-groups.md)

$$
\boxed{H=\{(u,v)\in F\times F:\pi(u)=\pi(v)\}.}
$$

Every specified generator belongs to the right-hand side, so one inclusion is immediate. For the reverse inclusion, diagonal generator pairs produce $(u,u)$ for every $u\in F$. Also

$$
(u,u)^{-1}(1,r_j)(u,u)=(1,u^{-1}r_ju),
$$

so their products and inverses produce $(1,r)$ for every $r\in R$. If $\pi(u)=\pi(v)$, then $u^{-1}v\in R$ and $(u,v)=(u,u)(1,u^{-1}v)\in H$, proving equality.

In particular $\boxed{(1,w)\in H\Longleftrightarrow w\in R\Longleftrightarrow w=1\text{ in }G_0}$. Constructing the input pair $(1,w)$ is effective, so a solution of the [membership problem for a subgroup](../../../../../../membership-problem-for-a-subgroup.md) $H\le F\times F$ would solve the insoluble [word problem for a group](../../../../../../word-problem-for-groups.md) in $G_0$. **The subgroup membership problem is therefore undecidable.** This is the [Mihailova subgroup](../../../../../../mihailova-subgroup.md) construction; its finite generating set follows from the finiteness of $X,J$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
