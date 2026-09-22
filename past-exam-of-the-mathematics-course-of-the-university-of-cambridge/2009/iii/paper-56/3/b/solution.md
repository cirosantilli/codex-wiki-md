<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Frobenius theorem](../../../../../../frobenius-theorem.md) says that [hypersurface orthogonality](../../../../../../hypersurface-orthogonality.md) of the nonzero covector $U_a$ is equivalent to $U_{[a}\nabla_bU_{c]}=0$, or locally $U_a=h\nabla_aS$ for some nonzero $h$. This immediately makes the screen projection of $\nabla_{[b}U_{a]}$ zero, since its antisymmetric part is a wedge product with $\nabla S$, which is proportional to $U$. Thus hypersurface orthogonality gives zero [null twist](../../../../../../null-twist.md).

For the converse, put $B_{ab}=\nabla_bU_a$. Nullness gives $U^aB_{ab}=\tfrac12\nabla_b(U^2)=0$, and the affine geodesic equation gives $B_{ab}U^b=0$. Resolve both tensor slots in the basis consisting of $U,N$ and the screen. These two identities exclude covector factors of $N$. Consequently

$$
B_{[ab]}=\widehat\omega_{ab}+U_{[a}q_{b]}
$$

for some covector $q$. If $\widehat\omega=0$, wedging this identity with $U$ makes $U_{[a}\nabla_bU_{c]}=0$. Applying [Frobenius theorem](../../../../../../frobenius-theorem.md) completes the proof:

$$
\boxed{\widehat\omega_{ab}=0\iff\text{the null geodesic congruence is hypersurface-orthogonal}.}
$$

This is the [null twist vanishes exactly for hypersurface-orthogonal geodesics](../../../../../../null-twist-vanishes-exactly-for-hypersurface-orthogonal-geodesics.md) criterion; the geodesic assumption ensures that the screen criterion implies the full Frobenius condition. The resulting hypersurfaces are null, and the congruence follows their null generators.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
