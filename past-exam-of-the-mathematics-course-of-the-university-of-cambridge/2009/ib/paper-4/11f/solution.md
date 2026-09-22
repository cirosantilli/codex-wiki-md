<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Prove the [submodule theorem for free modules over a principal ideal domain](../../../../../submodule-theorem-for-free-modules-over-a-principal-ideal-domain.md) by induction on the rank of $R^n$. For a submodule $N$, project onto its first coordinate. The image is an ideal $aR$. If $a=0$, then $N$ is a submodule of $R^{n-1}$ and induction applies. Otherwise choose $v\in N$ projecting to $a$. Every $w\in N$ has first coordinate $ra$ and hence $w-rv$ lies in the projection kernel. The domain property shows $Rv$ meets that kernel only at zero. Thus

$$
N=Rv\oplus\ker(\text{first-coordinate projection}|_N),
$$

and the kernel is a [free module](../../../../../free-module.md) by induction. This proves that $N$ is free, of rank at most $n$.

To prove [free modules are projective](../../../../../free-modules-are-projective.md), choose a basis $(e_\lambda)$ of a free module $P$. For the given surjection $f$, choose $m_\lambda\in M$ with $f(m_\lambda)=g(e_\lambda)$ and extend $e_\lambda\mapsto m_\lambda$ linearly. Finite support of basis expansions makes the resulting [module homomorphism](../../../../../module-homomorphism.md) well defined, and $f\circ h=g$.

Finally, take a finite generating set of a [projective module](../../../../../projective-module.md) $P$ to obtain a surjection $\pi:R^n\to P$. Projectivity applied to $\operatorname{id}_P$ gives a section $s:P\to R^n$ with $\pi s=\operatorname{id}_P$. Thus $s$ is injective and identifies $P$ with a submodule of $R^n$. The proved [submodule theorem for free modules over a principal ideal domain](../../../../../submodule-theorem-for-free-modules-over-a-principal-ideal-domain.md) shows that **every finitely generated projective module over a principal ideal domain is free**.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
