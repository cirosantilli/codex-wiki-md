<h1 id="18i/solution">Solution</h1>

↑ **Parent:** [18I](../18i.md)

The elementary symmetric functions are

$$
e_r(x_1,\ldots,x_n)=\sum_{1\leq i_1<\cdots<i_r\leq n}x_{i_1}\cdots x_{i_r}.
$$

The [Fundamental theorem of symmetric polynomials](../../../../../fundamental-theorem-of-symmetric-polynomials.md) says that every symmetric polynomial is uniquely a polynomial in $e_1,\ldots,e_n$.

If $r_1,\ldots,r_n$ are the roots of a monic polynomial, its [discriminant](../../../../../polynomial-discriminant.md) is

$$
\operatorname{Disc}(f)=\prod_{i<j}(r_i-r_j)^2.
$$

This is symmetric in the roots, hence the theorem and Vieta's formulas express it polynomially in the coefficients. Equivalently,

$$
\operatorname{Disc}(f)=(-1)^{n(n-1)/2}\operatorname{Res}(f,f').
$$

For $x^5+q$ this gives

$$
\boxed{\operatorname{Disc}(x^5+q)=5^5q^4=3125q^4}.
$$

For $f=x^5+px^2+q$, a repeated root solves $f=f'=0$. Elimination gives

$$
\boxed{\operatorname{Disc}(f)=q(108p^5+3125q^3)}.
$$

**Thus the discriminant vanishes exactly when $q=0$ or $108p^5+3125q^3=0$.**

## ↑ Ancestors (10)

1. [18I](../18i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
