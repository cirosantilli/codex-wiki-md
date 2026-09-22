<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [finite abelian group](../../../../../../finite-abelian-group.md) additively. A [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) is a [group homomorphism](../../../../../../group-homomorphism.md) $\chi:G\to\{z:|z|=1\}$. We first prove that there are exactly $|G|$ such [characters of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md), without assuming a structure theorem.

Use [extension of a character across a cyclic quotient](../../../../../../extension-of-a-character-across-a-cyclic-quotient.md). Given a [subgroup](../../../../../../subgroup.md) $H$ and $a\notin H$, let $k$ be the least positive integer with $ka\in H$. The [subgroup](../../../../../../subgroup.md) $K=H+\langle a\rangle$ has $k$ cosets of $H$. If $\phi$ is a [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) on $H$, choose any of the $k$ roots $\lambda^k=\phi(ka)$ and define

$$
\widetilde\phi(h+ja)=\phi(h)\lambda^j.
$$

This is well-defined: two representations differ by an integer multiple of $ka$, and the root equation exactly cancels that difference. It is a [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md), and every extension arises from one of the $k$ choices of $\lambda$. Build a chain from the trivial [subgroup](../../../../../../subgroup.md) to $G$ by adjoining elements. The [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) count multiplies by the same factor as the [subgroup](../../../../../../subgroup.md) order at every step, so $|\widehat G|=|G|$.

For a nontrivial [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) $\eta$, choose $a$ with $\eta(a)\ne1$. Translating the group sum shows

$$
\sum_{x\in G}\eta(x)
=\eta(a)\sum_{x\in G}\eta(x),
$$

so the sum is zero. Applied to $\chi\overline\psi$, this proves

$$
\sum_{x\in G}\chi(x)\overline{\psi(x)}
=\begin{cases}|G|,&\chi=\psi,\\0,&\chi\ne\psi.\end{cases}
$$

The $|G|$ [orthogonal](../../../../../../orthogonal-vectors.md) nonzero [characters of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) therefore form a [basis](../../../../../../basis.md) of all complex [functions](../../../../../../function-split.md) on $G$, a [vector space](../../../../../../vector-space-split.md) of [dimension](../../../../../../dimension-vector-space.md) $|G|$.

With the unnormalized [Fourier coefficients](../../../../../../fourier-coefficient.md) $\widehat f(\chi)=\sum_{x\in G}f(x)\overline{\chi(x)}$, expansion in that basis gives the [Fourier inversion on a finite group](../../../../../../fourier-inversion-on-a-finite-group.md)

$$
\boxed{f(x)=\frac1{|G|}\sum_{\chi\in\widehat G}\widehat f(\chi)\chi(x).}
$$

Under a normalized forward-transform convention the prefactor would instead be one. Thus the unspecified constant is determined by the convention, and the inversion itself follows directly from [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) counting and [orthogonality](../../../../../../orthogonal-vectors.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
