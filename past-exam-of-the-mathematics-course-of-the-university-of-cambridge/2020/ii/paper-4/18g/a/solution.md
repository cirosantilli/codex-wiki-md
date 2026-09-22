<h1 id="18g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $f(x)=a\prod_{i=1}^n(x-\alpha_i)$. Its [polynomial discriminant](../../../../../../polynomial-discriminant.md) is

$$
\Delta(f)=a^{2n-2}\prod_{i<j}(\alpha_i-\alpha_j)^2
=(-1)^{n(n-1)/2}a^{n-2}\operatorname{Res}(f,f').
$$

The squared [Vandermonde determinant](../../../../../../vandermonde-determinant.md) is a symmetric polynomial in the roots. By the [Fundamental theorem of symmetric polynomials](../../../../../../fundamental-theorem-of-symmetric-polynomials.md), it is a polynomial in their elementary symmetric functions, which are the coefficients of $f$ by [Vieta formulas](../../../../../../vieta-formulas.md); hence $\Delta(f)\in K$. Equivalently, the [resultant](../../../../../../resultant.md) formula puts it directly in $K$.

For $f=x^4+rx+s$, a resultant calculation with $f'=4x^3+r$ gives

$$
\boxed{\Delta(f)=256s^3-27r^4}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18G](../../18g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
