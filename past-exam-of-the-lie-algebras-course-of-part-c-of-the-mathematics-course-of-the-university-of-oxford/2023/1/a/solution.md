<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since the [general linear Lie algebra](../../../../general-linear-lie-algebra.md) $\mathfrak{gl}_1(k)$ has zero [Lie bracket](../../../../lie-bracket.md), identify it with $kz$. A [central extension of a Lie algebra](../../../../central-extension-of-a-lie-algebra.md) is a [short exact sequence](../../../../short-exact-sequence.md)

$$
0\longrightarrow kz\xrightarrow{\iota}\widetilde{\mathfrak g}\xrightarrow{\pi}\mathfrak g\longrightarrow0
$$

of [Lie algebra homomorphisms](../../../../lie-algebra-homomorphism.md) with $\iota(kz)$ contained in the [center of a Lie algebra](../../../../center-of-a-lie-algebra.md) $Z(\widetilde{\mathfrak g})$. Thus $\pi$ is surjective, its [kernel](../../../../kernel-of-a-linear-map-split.md) is precisely the indicated line, and that line commutes with all of $\widetilde{\mathfrak g}$.

Choose a [linear map](../../../../linear-map.md) $s:\mathfrak g\to\widetilde{\mathfrak g}$ with $\pi s=\operatorname{id}$. Such a section exists by lifting a [basis](../../../../basis.md). Identify $\widetilde{\mathfrak g}$ with the [direct sum of vector spaces](../../../../direct-sum.md) $\mathfrak g\oplus kz$ by $(x,tz)\mapsto s(x)+t\iota(z)$. The difference $[s(x),s(y)]-s([x,y])$ belongs to the [kernel](../../../../kernel-of-a-linear-map-split.md) of $\pi$, so there is a unique [bilinear map](../../../../bilinear-map.md) $\alpha:\mathfrak g\times\mathfrak g\to k$ such that

$$
[s(x),s(y)]-s([x,y])=\alpha(x,y)\iota(z).
$$

It is an [alternating bilinear form](../../../../alternating-bilinear-form.md): $\alpha(x,x)=0$, equivalently $\alpha(x,y)=-\alpha(y,x)$ in [characteristic zero](../../../../characteristic-zero.md). Taking the central component of the [Jacobi identity](../../../../jacobi-identity.md) gives the [Lie algebra two-cocycle](../../../../lie-algebra-two-cocycle.md) condition

$$
\alpha([x,y],w)+\alpha([y,w],x)+\alpha([w,x],y)=0\qquad(x,y,w\in\mathfrak g).
$$

Conversely, any [alternating bilinear form](../../../../alternating-bilinear-form.md) satisfying this identity defines a [Lie algebra](../../../../lie-algebra-split.md) by

$$
\boxed{[(x,tz),(y,uz)]=([x,y],\alpha(x,y)z).}
$$

Indeed its [Lie bracket](../../../../lie-bracket.md) is an [alternating multilinear map](../../../../alternating-multilinear-map.md) and a [bilinear map](../../../../bilinear-map.md), and the two components of its [Jacobi identity](../../../../jacobi-identity.md) are respectively the [Jacobi identity](../../../../jacobi-identity.md) in $\mathfrak g$ and the displayed [Lie algebra two-cocycle](../../../../lie-algebra-two-cocycle.md) condition. The line $kz$ is central, and projection to $\mathfrak g$ gives the required [central extension of a Lie algebra](../../../../central-extension-of-a-lie-algebra.md).

For later use, replacing $s$ by $s'(x)=s(x)+t(x)\iota(z)$, where $t\in\mathfrak g^*$ is in the [dual space](../../../../dual-space-split.md), changes the [Lie algebra two-cocycle](../../../../lie-algebra-two-cocycle.md) to

$$
\boxed{\alpha'(x,y)=\alpha(x,y)-t([x,y]).}
$$

Thus changes of section add a [Lie algebra two-coboundary](../../../../lie-algebra-two-coboundary.md), up to the conventional sign. A section that is a [Lie algebra homomorphism](../../../../lie-algebra-homomorphism.md) has $\alpha'=0$ and gives a [direct sum of Lie algebras](../../../../direct-sum-of-lie-algebras.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the lie algebras course of Part C of the mathematics course of the University of Oxford](../../../split.md)
5. [Lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
