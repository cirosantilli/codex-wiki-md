<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $G=M^{-1}N$. Subtracting the exact equation $Mx=Nx+b$ from the iteration gives $e_{\ell+1}=Ge_\ell$, where $e_\ell=x-x^{(\ell)}$. Hence $e_\ell=G^\ell e_0$. Also

$$
\det(N-\lambda M)=\det(M)\det(G-\lambda I),
$$

so the stated scalars are precisely the [eigenvalues](../../../../eigenvalue.md) of the [iteration matrix](../../../../iteration-matrix.md) $G$.

The [spectral radius criterion for matrix powers](../../../../spectral-radius-criterion-for-matrix-powers.md) states that $G^\ell\to0$ if and only if all its [eigenvalues](../../../../eigenvalue.md) have modulus strictly less than one. Applying that theorem gives $e_\ell\to0$ for every initial vector. Therefore $\boxed{x^{(\ell)}\to A^{-1}b}$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
