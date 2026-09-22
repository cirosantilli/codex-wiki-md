<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the [complex inner product](../../../../hermitian-inner-product.md) $\langle a,b\rangle=\sum_j\overline{a_j}b_j=a^\dagger b$, conjugate-linear in its first argument. For $a\ne0$, put $c=\langle a,b\rangle/\langle a,a\rangle$. Positivity gives

$$
0\leq\|b-ca\|^2=\|b\|^2-\frac{|\langle a,b\rangle|^2}{\|a\|^2}.
$$

Hence the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) is $|\langle a,b\rangle|\leq\|a\|\|b\|$. If $a=0$ it is immediate; equality holds precisely when the two [vectors](../../../../vector.md) are [linearly dependent](../../../../linear-dependence.md).

For a [unitary matrix](../../../../unitary-matrix.md), $U^\dagger U=I$, so $\|Ua\|^2=a^\dagger U^\dagger Ua=\|a\|^2$. If $Uv=\lambda v$ with a nonzero [eigenvector](../../../../eigenvector.md), this implies $|\lambda|\|v\|=\|v\|$. Thus every [eigenvalue](../../../../eigenvalue.md) satisfies

$$
\boxed{|\lambda|=1.}
$$

For the one-parameter family, expand unitarity to first order: $(I+tA^\dagger+O(t^2))(I+tA+O(t^2))=I$, so $A^\dagger+A=0$. Thus $A$ is a [skew-Hermitian matrix](../../../../skew-hermitian-matrix.md), an element of the [unitary Lie algebra](../../../../unitary-lie-algebra.md). If $Av=\mu v$, then $v^\dagger Av=\mu\|v\|^2$, whereas complex conjugation gives $(v^\dagger Av)^*=v^\dagger A^\dagger v=-v^\dagger Av$. Consequently $\overline\mu=-\mu$, proving that every [eigenvalue](../../../../eigenvalue.md) of $A$ is purely imaginary, with zero permitted.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
