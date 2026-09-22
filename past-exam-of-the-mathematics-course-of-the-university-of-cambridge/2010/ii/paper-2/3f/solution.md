<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Let $v=T(0)$ and $B(x)=T(x)-v$. The [Euclidean isometry](../../../../../euclidean-isometry.md) $B$ fixes the origin and preserves norms. The [polarization identity](../../../../../polarization-identity.md) therefore gives $\langle Bx,By\rangle=\langle x,y\rangle$. In particular, $B e_1,B e_2$ are an [orthonormal basis](../../../../../orthonormal-basis.md). The coefficients of $Bx$ in this basis are $\langle Bx,B e_j\rangle=x_j$, so $Bx=x_1B e_1+x_2B e_2$. Thus $B$ is a [linear map](../../../../../linear-map.md) represented by an [orthogonal matrix](../../../../../orthogonal-matrix.md), and **$T(x)=Bx+v$.** Conversely, every such map preserves distances because $\|B(x-y)\|=\|x-y\|$.

When $\det B=-1$, the real [eigenvalues](../../../../../eigenvalue.md) of the two-dimensional [orthogonal matrix](../../../../../orthogonal-matrix.md) are $1,-1$. Choose corresponding unit [eigenvectors](../../../../../eigenvector.md) $e,n$, and write $v=ae+bn$. In these coordinates $T(s,t)=(s+a,-t+b)$. This is reflection in the line $t=b/2$, followed by translation $ae$ along that line. **It is a [Euclidean reflection](../../../../../reflection-mathematics.md) if $a=0$, and a [glide reflection](../../../../../glide-reflection.md) if $a\ne0$.**

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
