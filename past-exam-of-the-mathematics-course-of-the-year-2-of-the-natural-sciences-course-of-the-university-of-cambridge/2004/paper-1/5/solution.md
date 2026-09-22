<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A real [orthogonal matrix](../../../../orthogonal-matrix.md) satisfies $Q^TQ=I$; a complex [unitary matrix](../../../../unitary-matrix.md) satisfies $U^\dagger U=I$. Their columns are orthonormal in the corresponding real or complex [inner product](../../../../inner-product-split.md).

Adopt the convention that a [complex inner product](../../../../hermitian-inner-product.md) is linear in its second argument, conjugate symmetric, and positive definite: $\langle u,u\rangle\geq0$, with equality exactly when $u=0$. Conjugate symmetry and second-argument linearity then imply antilinearity in the first:

$$
\langle\alpha u_1+\beta u_2,v\rangle=\overline{\langle v,\alpha u_1+\beta u_2\rangle}=\overline{\alpha\langle v,u_1\rangle+\beta\langle v,u_2\rangle}=\bar\alpha\langle u_1,v\rangle+\bar\beta\langle u_2,v\rangle.
$$

For the specified real symmetric matrix use $b=a^2$. Its upper block is the [outer product](../../../../outer-product.md) $(1,a)^T(1,a)$, so it has one zero eigenvalue and one eigenvalue $1+a^2$. A complete [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) is

$$
\boxed{\lambda_0=0,\quad v_0=\frac{(-a,1,0)^T}{\sqrt{1+a^2}};\qquad \lambda_+=1+a^2=1+b,\quad v_+=\frac{(1,a,0)^T}{\sqrt{1+a^2}};\qquad \lambda_c=c,\quad v_c=(0,0,1)^T.}
$$

If $c=1+b$, the last two eigenvalues coincide and their [eigenspace](../../../../eigenspace.md) is the span of $v_+,v_c$; every nonzero vector in that span is an eigenvector. Since $c>0$, the zero eigenspace remains one-dimensional.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
