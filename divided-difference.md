# Divided difference

↑ **Parent:** [Polynomial interpolation](polynomial-interpolation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divided_difference)

For $k+1$ distinct [interpolation nodes](interpolation-node.md), the [divided difference](divided-difference.md) $f[x_0,\ldots,x_k]$ is the coefficient of $x^k$ in the [interpolation polynomial](interpolation-polynomial.md) of [polynomial degree](degree-of-a-polynomial.md) at most $k$ through those [interpolation nodes](interpolation-node.md). It is the [leading coefficient](leading-coefficient-of-a-polynomial.md) when that [polynomial degree](degree-of-a-polynomial.md) is exactly $k$, and zero when it is smaller. Explicitly,

$$
f[x_0,\ldots,x_k]
=\sum_{j=0}^k\frac{f(x_j)}
{\prod_{i\ne j}(x_j-x_i)}.
$$

starting with $f[x_i]=f(x_i)$. The [divided differences](divided-difference.md) obey the recurrence

$$
f[x_0,\ldots,x_k]
=\frac{f[x_1,\ldots,x_k]-f[x_0,\ldots,x_{k-1}]}
{x_k-x_0}.
$$

For data $f(0)=1$, $f(1)=2$, $f(2)=5$, the first [divided differences](divided-difference.md) are $f[0,1]=(2-1)/(1-0)=1$ and $f[1,2]=(5-2)/(2-1)=3$. The second [divided difference](divided-difference.md) is $f[0,1,2]=(3-1)/(2-0)=1$, the [leading coefficient](leading-coefficient-of-a-polynomial.md) of $x^2+1$. The first [divided difference](divided-difference.md) is the slope of a [secant line](secant-line.md); higher [divided differences](divided-difference.md) supply successive coefficients for the [Newton polynomial](newton-polynomial.md).

**Table of contents**

- [Divided difference table](divided-difference-table.md)
- [Symmetry of divided differences](symmetry-of-divided-differences.md)
- [Omitted-node identities for divided differences](omitted-node-identities-for-divided-differences.md)
- [Exponential divided difference](exponential-divided-difference.md)
- [Leibniz rule for divided differences](leibniz-rule-for-divided-differences.md)
- [Newton polynomial](newton-polynomial.md)
  - [Node order in Newton interpolation](node-order-in-newton-interpolation.md)

## ↑ Ancestors (7)

1. [Polynomial interpolation](polynomial-interpolation.md)
2. [Interpolation](interpolation-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (40)

- [B-spline differentiation formula](b-spline-differentiation-formula.md)
- [Divided difference](divided-difference.md)
- [Divided difference table](divided-difference-table.md)
- [Interpolation polynomial](interpolation-polynomial.md)
- [Lee interpolation identity](lee-interpolation-identity.md)
- [Newton polynomial](newton-polynomial.md)
- [Node order in Newton interpolation](node-order-in-newton-interpolation.md)
- [Omitted-node identities for divided differences](omitted-node-identities-for-divided-differences.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-56/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/14b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/14b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/14b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-61/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-69/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-61/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/6/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/6b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-318/5/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-318/3/a/solution.md)
- [Simple-knot B-spline regularity](simple-knot-b-spline-regularity.md)
- [Spline knot sequence](spline-knot-sequence.md)
- [Support and Gram bandwidth of B-splines](support-and-gram-bandwidth-of-b-splines.md)
- [Symmetry of divided differences](symmetry-of-divided-differences.md)
- [Truncated power function](truncated-power-function.md)
- [Unit-integral normalization of a B-spline](unit-integral-normalization-of-a-b-spline.md)
