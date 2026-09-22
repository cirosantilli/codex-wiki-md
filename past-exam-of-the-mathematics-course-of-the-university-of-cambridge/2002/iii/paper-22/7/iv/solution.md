<h1 id="7/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First prove the hinted statement. Let $U\subseteq y_n$ be the domain of a partial presheaf map $\phi:U\to y_{n+1}$. If $U$ is nonempty, take a section $f:m\to n$ in $U(m)$ and write $g=\phi_m(f):m\to n+1$. Hypothesis (c) supplies $h,k:m+1\to m$ with $fh=fk$ but $gh\ne gk$. Because $U$ is a subpresheaf, both restrictions belong to $U(m+1)$; naturality gives

$$
gh=\phi_{m+1}(fh)=\phi_{m+1}(fk)=gk,
$$

a contradiction. Therefore **every such partial map has empty domain**.

Now suppose a presheaf map $y_n\to A_{n+1}$ existed. Pull back the [monomorphism](../../../../../../monomorphism.md) $y_{n+1}\hookrightarrow A_{n+1}$ along it. Its unit image is dense by the preceding plus-construction argument, and density is stable under pullback, so the resulting domain $U\subseteq y_n$ is dense. It gives exactly a partial map $U\to y_{n+1}$ of the prohibited kind. Such a domain cannot be empty: at the section $1_n$ of $y_n(n)$, density would otherwise require the empty [sieve on a category](../../../../../../sieve-category-theory.md) to cover. Thus there is no map $y_n\to A_{n+1}$.

Any sheaf map $A_n\to A_{n+1}$, composed with $y_n\hookrightarrow A_n$, would be such a presheaf map. Hence

$$
\boxed{\operatorname{Hom}_{\operatorname{Sh}(C,J)}(A_n,A_{n+1})=\varnothing.}
$$

The stronger intermediate statement also says $A_{n+1}(n)=\varnothing$, by the Yoneda correspondence. It will be useful for the last clause.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [7](../../7.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
