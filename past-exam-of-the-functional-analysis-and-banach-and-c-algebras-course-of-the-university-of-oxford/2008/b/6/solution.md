<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [spectrum of an element](../../../../spectrum-of-an-element.md) is $\sigma_A(a)=\{\lambda\in\mathbb C:a-\lambda1_A\text{ is not invertible in }A\}$. A [Normal element of a C-star algebra](../../../../normal-element-of-a-c-star-algebra.md) satisfies $a^*a=aa^*$.

For a [Hermitian C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) $h$, the [C-star identity](../../../../c-star-identity.md) gives $\|h^2\|=\|h\|^2$. For normal $a$, commutation gives

$$
\|a^2\|^2=\|(a^*)^2a^2\|=\|(a^*a)^2\|=\|a^*a\|^2=\|a\|^4.
$$

All powers remain normal, so induction yields $\|a^{2^k}\|=\|a\|^{2^k}$. Taking the spectral-radius limit along these powers gives

$$
\boxed{\nu_A(a)=\|a\|\quad\text{for normal }a.}
$$

Let $\varphi:A\to B$ be a [C-star homomorphism](../../../../c-star-homomorphism.md), without assuming continuity or preservation of the ambient unit. Put $p=\varphi(1_A)$, a [projection in a C-star algebra](../../../../projection-in-a-c-star-algebra.md). If $p=0$, then $\varphi=0$. Otherwise its image lies in the unital corner $pBp$ and it is unital as a map into that corner. An inverse in $A$ maps to an inverse in the corner, so $\sigma_{pBp}(\varphi(b))\subseteq\sigma_A(b)$. Apply this to the normal element $b=a^*a$ and use the [C-star identity](../../../../c-star-identity.md) in both algebras:

$$
\|\varphi(a)\|^2=\|\varphi(a^*a)\|=\nu_{pBp}(\varphi(a^*a))\leq\nu_A(a^*a)=\|a^*a\|=\|a\|^2.
$$

Thus **every [C-star homomorphism](../../../../c-star-homomorphism.md) is [norm](../../../../norm.md) non-increasing**, including nonunital maps.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
