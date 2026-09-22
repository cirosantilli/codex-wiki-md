<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

An extension of $A$ by $B$ is a [short exact sequence](../../../../short-exact-sequence.md) $1\to A\to G\to B\to1$. It splits if the quotient map has a homomorphic section. Equivalently the embedded $A$ has a subgroup complement isomorphic to $B$, and $G$ is the corresponding [semidirect product](../../../../semidirect-product.md).

For $t\notin K$ and $a\in K$, both $t$ and $ta$ lie outside $K$, so $t^2=(ta)^2=1$. It follows that $tat=a^{-1}$, and $t=t^{-1}$ gives the claimed [conjugation](../../../../conjugation.md) identity. [Conjugation](../../../../conjugation.md) is an [automorphism](../../../../automorphism.md) of $K$, so inversion is an [automorphism](../../../../automorphism.md) there. Comparing the image of $ab$ with the product of the images gives $b^{-1}a^{-1}=a^{-1}b^{-1}$. Therefore **$K$ is abelian**.

Conversely inversion is an [automorphism](../../../../automorphism.md) of any [abelian group](../../../../abelian-group.md) $A$, of order dividing two. Form the [semidirect product](../../../../semidirect-product.md) $G=A\rtimes C_2$ with multiplication

$$
(a,\varepsilon)(b,\delta)=(ab^{(-1)^\varepsilon},\varepsilon+\delta),\qquad\varepsilon,\delta\in\mathbb Z/2.
$$

For completeness associativity follows because $b\mapsto b^{(-1)^\varepsilon}$ is an [automorphism](../../../../automorphism.md) and these automorphisms compose according to addition modulo two; $(1,0)$ is the identity and inverses follow from this formula. The subgroup $H=A\times\{0\}$ is normal with quotient $C_2$, and every outside element satisfies $(a,1)^2=(aa^{-1},0)=1$. Thus **the [generalized dihedral group](../../../../generalized-dihedral-group.md) supplies the required extension**, including when $A$ is infinite or has elements of order two.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
