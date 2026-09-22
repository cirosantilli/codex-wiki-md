<h1 id="39a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the active block have size $m$. Using a stored skew triangle, the product $Dv$ costs $m(m-1)$ scalar multiplications: two for each unordered off-diagonal pair. Updating its stored triangle with $vw^T-wv^T$ costs another $m(m-1)$ products. Reflector construction, scalings and the active column take only $O(m)$ additional products. Summing over $m=n-1,\ldots,2$ gives

$$
\boxed{\text{skew-symmetric cost}=\frac23n^3+O(n^2)\text{ products}}.
$$

For a symmetric block, an optimized matrix-vector calculation costs $m^2$ products, and the symmetric rank-two update of one triangle costs $m(m+1)$ products. The additional scalar $v^TDv$ and its correction to the update [vector](../../../../../../vector.md) cost only $O(m)$ per step. Thus

$$
\boxed{\text{symmetric cost}=\frac23n^3+O(n^2)\text{ products}}.
$$

The leading terms are the same under the requested product-count convention. Skew symmetry removes the diagonal work and the scalar correction, giving lower-order savings, not a factor-of-two leading advantage over an already symmetry-aware implementation. Counting additions as well would change the reported flop constants; it is not the convention requested here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
