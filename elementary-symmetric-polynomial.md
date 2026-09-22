# Elementary symmetric polynomial

↑ **Parent:** [Polynomial](polynomial-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elementary_symmetric_polynomial)

The $k$th elementary symmetric polynomial adds every product obtained by choosing $k$ distinct positions from $x_1,\ldots,x_n$:

$$
e_k(x_1,\ldots,x_n)=\sum_{1\leq i_1<\cdots<i_k\leq n}x_{i_1}\cdots x_{i_k}.
$$

The conventions are $e_0=1$ and $e_k=0$ for $k>n$. The positions must be distinct, but their values may coincide. Each [permutation](permutation.md) of the variables merely rearranges the summands, so this is a [symmetric polynomial](symmetric-polynomial.md).

For $x_1=1$, $x_2=2$, $x_3=3$, we obtain $e_1=1+2+3=6$, $e_2=1\cdot2+1\cdot3+2\cdot3=11$, and $e_3=1\cdot2\cdot3=6$. Expanding the product gives

$$
\boxed{(z-1)(z-2)(z-3)=z^3-6z^2+11z-6}.
$$

In general, $\prod_{i=1}^n(z-x_i)=z^n-e_1z^{n-1}+e_2z^{n-2}-\cdots+(-1)^ne_n$. Thus the [coefficients](coefficient.md) of a [monic polynomial](monic-polynomial.md) collect [elementary symmetric polynomials](elementary-symmetric-polynomial.md) of its [roots of a polynomial](root-of-a-polynomial.md), with alternating signs. These are the [Vieta formulas](vieta-s-formulas.md).[NIST Digital Library of Mathematical Functions; §1.11(ii), equation 1.11.10](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

<a id="image-choosing-one-two-or-three-root-positions-gives-the-coefficients-of-a-cubic"></a>
![](elementary-symmetric-root-products.png)

**[Figure 9](#image-choosing-one-two-or-three-root-positions-gives-the-coefficients-of-a-cubic). Choosing one, two, or three root positions gives the coefficients of a cubic**. For the stipulated roots $1,2,3$, node values add to $e_1=6$, edge products add to $e_2=11$, and the product of all three positions is $e_3=6$. These [elementary symmetric polynomials](elementary-symmetric-polynomial.md) enter the [monic polynomial](monic-polynomial.md) with alternating signs. The graph is an original illustration of the exact finite calculation.

**Table of contents**

- [Elementary symmetric sum](elementary-symmetric-sum.md)
- [Fundamental theorem of symmetric polynomials](fundamental-theorem-of-symmetric-polynomials.md)
- [Newton's identities](newton-s-identities.md)
  - [Root power-sum recurrence](root-power-sum-recurrence.md)
  - [Characteristic polynomial from traces of powers](characteristic-polynomial-from-traces-of-powers.md)
  - [Root sensitivity in power-sum reconstruction](root-sensitivity-in-power-sum-reconstruction.md)
  - [Newton identities in positive characteristic](newton-identities-in-positive-characteristic.md)

## ↑ Ancestors (5)

1. [Polynomial](polynomial-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Elementary symmetric polynomial](elementary-symmetric-polynomial.md)
- [Exact tied-set conditional likelihood](exact-tied-set-conditional-likelihood.md)
- [Explicit multistep methods cannot be A-stable](explicit-multistep-methods-cannot-be-a-stable.md)
- [Monomial B-spline coefficients](monomial-b-spline-coefficients.md)
- [Newton identities in positive characteristic](newton-identities-in-positive-characteristic.md)
- [Newton's identities](newton-s-identities.md)
- [1 Algebraic and Analytic Methods](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-3/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/17f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-125/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-136/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-142/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-142/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-142/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-312/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-318/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-101/3/b/solution.md)
- [Repeated roots in Vieta's formulas](repeated-roots-in-vieta-s-formulas.md)
- [Representation ring of an odd-dimensional special orthogonal group](representation-ring-of-an-odd-dimensional-special-orthogonal-group.md)
- [Symmetric-coordinate identity for elliptic-curve addition](symmetric-coordinate-identity-for-elliptic-curve-addition.md)
- [Symmetric polynomial](symmetric-polynomial.md)
- [Vieta formulas for a cubic](vieta-formulas-for-a-cubic.md)
- [Vieta's formulas](vieta-s-formulas.md)
