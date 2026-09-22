<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [semidirect product of a Lie algebra and a module](../../../../semidirect-product-of-a-lie-algebra-and-a-module.md)

$$
L=\mathfrak{sl}_2(k)\ltimes k^2,\qquad[(X,u),(Y,v)]=([X,Y],Xv-Yu),
$$

where $k^2$ is the [defining representation](../../../../defining-representation-of-a-matrix-lie-algebra.md) of the [sl2 Lie algebra](../../../../sl2-lie-algebra.md). To see directly that this is a [Lie algebra](../../../../lie-algebra-split.md), realize $(X,u)$ as the block [matrix](../../../../matrix.md) $\left(\begin{smallmatrix}X&u\\0&0\end{smallmatrix}\right)$. These [matrices](../../../../matrix.md) are closed under the [operator commutator](../../../../operator-commutator.md), whose [Jacobi identity](../../../../jacobi-identity.md) holds in every [associative algebra](../../../../associative-algebra-split.md).

Using the standard [sl2 triple](../../../../sl2-triple.md) $e,h,f$, its [Lie brackets](../../../../lie-bracket.md) show $[\mathfrak{sl}_2,\mathfrak{sl}_2]=\mathfrak{sl}_2$: indeed $h=[e,f]$, $e=[h,e]/2$, and $f=-[h,f]/2$. Also $h=\operatorname{diag}(1,-1)$ is invertible on $k^2$. For any $u\in k^2$, put $v=h^{-1}u$; then

$$
[(h,0),(0,v)]=(0,u).
$$

It follows that the [derived algebra](../../../../derived-algebra.md) contains both $\mathfrak{sl}_2\oplus0$ and $0\oplus k^2$, so $[L,L]=L$: this is a [perfect Lie algebra](../../../../perfect-lie-algebra.md).

However, $0\oplus k^2$ is a nonzero [ideal of a Lie algebra](../../../../ideal-of-a-lie-algebra.md) with zero [Lie bracket](../../../../lie-bracket.md). It is therefore a [solvable Lie algebra](../../../../solvable-lie-algebra.md) and is contained in the [solvable radical](../../../../radical-of-a-lie-algebra.md) of $L$. A [semisimple Lie algebra](../../../../semisimple-lie-algebra-split.md) has zero [solvable radical](../../../../radical-of-a-lie-algebra.md), so

$$
\boxed{[L,L]=L,\qquad0\ne k^2\subseteq\operatorname{rad}L,\qquad\dim L=5.}
$$

This illustrates the [perfect semidirect product criterion](../../../../perfect-semidirect-product-criterion.md): the [Lie brackets](../../../../lie-bracket.md) internal to the first summand generate it, while its action generates the second summand.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
