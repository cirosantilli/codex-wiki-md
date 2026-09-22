<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a [pointed category](../../../../../pointed-category.md), a [normal monomorphism](../../../../../normal-monomorphism.md) is a monomorphism that is the [kernel in a category](../../../../../kernel-in-a-category.md) of some morphism. Suppose $m:M\hookrightarrow A$ is the kernel of $f:A\to B$, and let $q:A\to Q$ be the [cokernel in a category](../../../../../cokernel-in-a-category.md) of $m$. Since $fm=0$, there is a unique $\bar f:Q\to B$ with $f=\bar f q$. If $qx=0$, then $fx=\bar f qx=0$, so the universal property of $m=\ker f$ factors $x$ uniquely through $m$. Therefore $m=\ker q=\ker(\operatorname{coker}m)$. The converse is immediate: if $m$ is the kernel of its cokernel, it is the kernel of a morphism and hence normal.

An [abelian category](../../../../../abelian-category.md) is an [additive category](../../../../../additive-category.md) with kernels and cokernels in which every monomorphism is normal and every epimorphism is a [conormal epimorphism](../../../../../conormal-epimorphism.md). Finite [biproducts](../../../../../biproduct.md) and kernels give finite limits. The [image and coimage in an abelian category](../../../../../image-and-coimage-in-an-abelian-category.md) give every $f:A\to B$ the canonical factorization

$$
A\twoheadrightarrow\operatorname{coim}f
\xrightarrow{\sim}\operatorname{im}f
\hookrightarrow B,
$$

and the middle map is an isomorphism. The first map is a cokernel and therefore a regular epimorphism. Every epimorphism in an abelian category is the cokernel of its kernel, and epimorphisms are stable under pullback; consequently regular epimorphisms are pullback-stable. This proves that [every abelian category is regular](../../../../../every-abelian-category-is-regular.md).

Define the [additive indexing category for chain complexes](../../../../../additive-indexing-category-for-chain-complexes.md) $\mathbf Z$ as follows. Its objects are the integers and

$$
\mathbf Z(n,p)=
\begin{cases}
\mathbb Z,&p=n\text{ or }p=n-1,\\
0,&\text{otherwise}.
\end{cases}
$$

Let the generator of $\mathbf Z(n,n)$ be $1_n$ and the generator of $\mathbf Z(n,n-1)$ be $\partial_n$. Composition is bilinear, the $1_n$ are identities, and

$$
\partial_{n-1}\partial_n=0
$$

because the target hom-group $\mathbf Z(n,n-2)$ is zero. An [additive functor](../../../../../additive-functor.md) $C:\mathbf Z\to\mathcal A$ chooses objects $C_n=C(n)$ and differentials $d_n=C(\partial_n)$ satisfying $d_{n-1}d_n=0$, hence a [complex in an abelian category](../../../../../complex-in-an-abelian-category.md). Conversely every chain complex defines this unique additive functor.

For self-duality, put $Z_n=\ker d_n$, $B_n=\operatorname{im}d_{n+1}$, and let $q:C_n\to Q_n=\operatorname{coker}d_{n+1}$. Since $d_nd_{n+1}=0$, there is a unique $\bar d_n:Q_n\to C_{n-1}$ with $\bar d_nq=d_n$. The image-to-kernel factorization gives a canonical isomorphism

$$
H_n(C_\bullet)
=\operatorname{coker}(B_n\hookrightarrow Z_n)
\cong\ker(\bar d_n:Q_n\to C_{n-1}).
$$

Passing to the [opposite category](../../../../../opposite-category.md) exchanges kernels with cokernels and images with coimages. The usual construction in $\mathcal A^{\mathrm{op}}$ is therefore the expression on the right, which is canonically the original [homology object](../../../../../homology-object.md). This proves the [self-duality of homology](../../../../../self-duality-of-homology.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
