<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $A$ be a three-dimensional [vector space](../../../../vector-space-split.md) with [basis](../../../../basis.md) $p,q,z$. Define a [bilinear map](../../../../bilinear-map.md) $\bullet:A\times A\to A$ by

$$
p\bullet q=z,\qquad q\bullet p=-z,
$$

with all other products of [basis vectors](../../../../basis-vector.md) zero. Equivalently,

$$
(ap+bq+cz)\bullet(a'p+b'q+c'z)=(ab'-ba')z.
$$

Every product belongs to $kz$, and every product with an element of $kz$ is zero. Hence both $(u\bullet v)\bullet w$ and $u\bullet(v\bullet w)$ vanish for every $u,v,w\in A$. This proves [associativity](../../../../associative-property.md), so $A$ is an [associative algebra](../../../../associative-algebra-split.md). The product is an [alternating multilinear map](../../../../alternating-multilinear-map.md), and each nested product in the [Jacobi identity](../../../../jacobi-identity.md) is zero, so the same product is a [Lie bracket](../../../../lie-bracket.md). It is nonzero because $p\bullet q=z\ne0$.

There is no multiplicative [identity element](../../../../identity-element.md): any candidate $1_A$ would satisfy $1_A\bullet z=0$, whereas an [identity element](../../../../identity-element.md) would require $1_A\bullet z=z$. Thus

$$
\boxed{A=kp\oplus kq\oplus kz,\quad p\bullet q=z=-q\bullet p,\quad A^2=kz,\quad A^3=0.}
$$

This is an [associative Lie product](../../../../associative-lie-product.md); its underlying [Lie algebra](../../../../lie-algebra-split.md) is the [Heisenberg Lie algebra](../../../../heisenberg-lie-algebra.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
