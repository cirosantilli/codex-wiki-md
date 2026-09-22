<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**Commuting inverse.** Assume $I-M$ is invertible, as required by the displayed inverse. Multiplication gives

$$
(I+M)(I-M)=I-M^2=(I-M)(I+M).
$$

Multiply on both sides by $(I-M)^{-1}$ to obtain

$$
\boxed{(I+M)(I-M)^{-1}=(I-M)^{-1}(I+M).}
$$

More generally, a [matrix](../../../../matrix.md) commuting with an invertible [matrix](../../../../matrix.md) also commutes with its inverse.

**Orthogonality.** For a real [skew-symmetric matrix](../../../../skew-symmetric-matrix.md) $A$, $x^TAx=0$. If $(I-A)x=0$ for a real [vector](../../../../vector.md) $x$, multiply by $x^T$ to obtain $\|x\|^2=0$. Thus $I-A$ is invertible; the same argument applies to $I+A$. For the [Cayley transform of a real skew-symmetric matrix](../../../../cayley-transform-of-a-real-skew-symmetric-matrix.md),

$$
N=(I+A)(I-A)^{-1},\qquad N^T=(I+A)^{-1}(I-A).
$$

The factors commute by the first result, so

$$
N^TN=(I+A)^{-1}(I-A)(I+A)(I-A)^{-1}=I.
$$

Therefore $\boxed{N\text{ is an orthogonal matrix}.}$

**Eigenvector mapping.** If $Av=av$, then $(I-A)^{-1}v=(1-a)^{-1}v$. Consequently

$$
\boxed{Nv=\frac{1+a}{1-a}v.}
$$

The denominator cannot vanish. In fact the [eigenvalues](../../../../eigenvalue.md) of a real [skew-symmetric matrix](../../../../skew-symmetric-matrix.md) are purely imaginary: $v^\dagger Av$ is the negative of its complex conjugate, so $a=-\overline a$. For $a=i\beta$ the corresponding [eigenvalue](../../../../eigenvalue.md) of $N$ is $(1+i\beta)/(1-i\beta)=e^{2i\arctan\beta}$, consistent with [orthogonality](../../../../orthogonal-vectors.md).

**Spectrum in three dimensions.** Let $Q$ be any real three-by-three [orthogonal matrix](../../../../orthogonal-matrix.md). For a complex [eigenvector](../../../../eigenvector.md) $v$, $\|Qv\|=\|v\|$ implies $|\lambda|=1$. A real cubic [characteristic polynomial](../../../../characteristic-polynomial.md) has a real root, necessarily $+1$ or $-1$. Any nonreal roots form a complex-conjugate pair of unit modulus. If all three roots are real, two of the three signs agree and can be grouped as a pair with angle zero or $\pi$. Thus in every case the [eigenvalues](../../../../eigenvalue.md) can be written

$$
\boxed{e^{i\alpha},\quad e^{-i\alpha},\quad\varepsilon,\qquad\alpha\in\mathbb R,\quad\varepsilon\in\{1,-1\}.}
$$

Their product is $\varepsilon=\det Q$.

**Determinant and fixed axis for the Cayley transform.** Since $A^T=-A$,

$$
\det(I+A)=\det((I+A)^T)=\det(I-A),
$$

so $\boxed{\det N=1}$. This determinant argument works in every dimension. In dimension three the preceding spectrum result then guarantees an [eigenvector](../../../../eigenvector.md) with $Nx=x$. Set $z=(I-A)^{-1}x$. The fixed-vector equation says $(I+A)z=(I-A)z$, so $Az=0$ and $x=(I-A)z=z$. Hence

$$
\boxed{Ax=0\text{ for a nonzero real direction }x.}
$$

This is the axis fixed by the three-dimensional [rotation](../../../../rotation-mathematics.md). Equivalently, a real odd-dimensional [skew-symmetric matrix](../../../../skew-symmetric-matrix.md) has zero [determinant](../../../../determinant.md), because $\det A=\det A^T=\det(-A)=-\det A$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
