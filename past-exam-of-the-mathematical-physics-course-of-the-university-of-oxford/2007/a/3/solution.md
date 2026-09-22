<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\Psi\ne0$ and take the reduced [positive operator](../../../../positive-operator.md) $\rho_1=\operatorname{Tr}_2|\Psi\rangle\langle\Psi|$. Choose orthonormal [eigenvectors](../../../../eigenvector.md) $\xi_j$ for its positive [eigenvalues](../../../../eigenvalue.md) $\lambda_j$. Define

$$
v_j=(\langle\xi_j|\otimes I)\Psi,\qquad c_j=\sqrt{\lambda_j},\qquad\eta_j=v_j/c_j.
$$

The defining identity of the [partial trace](../../../../partial-trace.md) gives $\langle v_i,v_j\rangle=\lambda_j\delta_{ij}$, so the $\eta_j$ are orthonormal. Expansion in a full eigenbasis of $\rho_1$ yields $\Psi=\sum_j\xi_j\otimes v_j$; zero-[eigenvalue](../../../../eigenvalue.md) terms have zero squared norm and contribute nothing. Thus

$$
\boxed{\Psi=\sum_jc_j|\xi_j\rangle|\eta_j\rangle,\qquad c_j>0.}
$$

The zero vector has the empty decomposition. Unit [normalization](../../../../normalization.md) would give $\sum_jc_j^2=1$, but no [normalization](../../../../normalization.md) is needed for the theorem itself.

For the given vector, the [coefficient matrix](../../../../coefficient-matrix.md) is $M=\bigl(\begin{smallmatrix}1&0\\0&1\\1&1\end{smallmatrix}\bigr)$. Its second reduced operator is $M^*M=\bigl(\begin{smallmatrix}2&1\\1&2\end{smallmatrix}\bigr)$, whose [eigenvalues](../../../../eigenvalue.md) are $3,1$ and [eigenvectors](../../../../eigenvector.md) $\eta_+=(E_1+E_2)/\sqrt2$, $\eta_-=(E_1-E_2)/\sqrt2$. The corresponding normalized first-factor vectors are

$$
\xi_+=\frac{e_1+e_2+2e_3}{\sqrt6},\qquad\xi_-=\frac{e_1-e_2}{\sqrt2}.
$$

Their norms are one and their [inner product](../../../../inner-product-split.md) is zero. Hence

$$
\boxed{\psi=\sqrt3\,|\xi_+\rangle|\eta_+\rangle+|\xi_-\rangle|\eta_-\rangle.}
$$

Expanding the two terms returns the original three contributions. The vector has squared norm $4$; if a normalized state is wanted, divide by two and the [Schmidt coefficients](../../../../schmidt-coefficient.md) become $\sqrt3/2$ and $1/2$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematical physics course of the University of Oxford](../../../split.md)
5. [Mathematical physics course of the University of Oxford](../../../../mathematical-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
