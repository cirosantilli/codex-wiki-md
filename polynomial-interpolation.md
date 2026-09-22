# Polynomial interpolation

↑ **Parent:** [Interpolation](interpolation-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_interpolation)

[Polynomial interpolation](polynomial-interpolation.md) constructs a [polynomial](polynomial-split.md) that passes exactly through prescribed data. Given $n+1$ distinct [interpolation nodes](interpolation-node.md) $x_0,\ldots,x_n$ and values $y_0,\ldots,y_n$, there is exactly one [interpolation polynomial](interpolation-polynomial.md) $p_n$ of [polynomial degree](degree-of-a-polynomial.md) at most $n$ with $p_n(x_i)=y_i$ for every $i$. The values may be samples $y_i=f(x_i)$ of a [function](function-split.md), but no knowledge of that [function](function-split.md) between the [interpolation nodes](interpolation-node.md) is needed to construct $p_n$. The [Lagrange polynomial](lagrange-polynomial.md) and [Newton polynomial](newton-polynomial.md) are two representations of this same answer.[Toby A. Driscoll and Richard J. Braun, Fundamentals of Numerical Computation, §9.1, Theorems 9.1.1–9.1.2](https://fncbook.com/polynomial/)

For example, the three data points $(0,1),(1,2),(2,5)$ give the [quadratic polynomial](quadratic-polynomial.md)

$$
p_2(x)=x^2+1,\qquad p_2(0)=1,\quad p_2(1)=2,\quad p_2(2)=5.
$$

Thus [polynomial interpolation](polynomial-interpolation.md) supplies $p_2(1/2)=5/4$ as an intermediate value. Whether this approximates an unknown underlying [function](function-split.md) well is a separate question about [polynomial interpolation error](polynomial-interpolation-error.md).

Both hypotheses in the uniqueness statement matter. The [Lagrange cardinal polynomials](lagrange-cardinal-polynomial.md) prove existence constructively. If two [polynomials](polynomial-split.md) of [polynomial degree](degree-of-a-polynomial.md) at most $n$ fit the data, their difference has $n+1$ distinct [roots of a polynomial](root-of-a-polynomial.md), so it must be zero. Repeated [interpolation nodes](interpolation-node.md) with conflicting values have no solution, and repeated equal values provide no additional independent condition; prescribed [derivatives](derivative.md) instead lead to [Hermite interpolation](hermite-interpolation.md). Without the [polynomial degree](degree-of-a-polynomial.md) restriction there are infinitely many solutions:

$$
p(x)=p_n(x)+q(x)\prod_{i=0}^n(x-x_i),
$$

where $q$ is any [polynomial](polynomial-split.md). By the [factor theorem](factor-theorem.md), this describes every [polynomial](polynomial-split.md) fitting the same data. In the example, $x^2+1+c\,x(x-1)(x-2)$ fits for every $c$, but at $x=1/2$ its value is $5/4+3c/8$; exact agreement at the three [interpolation nodes](interpolation-node.md) alone says nothing about that intermediate value.

The usefulness of [polynomial interpolation](polynomial-interpolation.md) is that data become an explicit [function](function-split.md) whose values, [derivatives](derivative.md), and [integrals](integral-split.md) can be calculated. Differentiating or integrating the [Lagrange cardinal polynomials](lagrange-cardinal-polynomial.md) produces [differentiation weights from nodal evaluations](differentiation-weights-from-nodal-evaluations.md) or a [quadrature rule](quadrature-rule.md). Exact passage through observations is the defining constraint. In [polynomial regression](polynomial-regression.md), [linear least squares](linear-least-squares.md) instead chooses a [polynomial degree](degree-of-a-polynomial.md) and minimizes a sum of squared residuals, generally without passing through every observation. Interpolating noisy values reproduces their errors at the [interpolation nodes](interpolation-node.md) and can amplify them between [interpolation nodes](interpolation-node.md); [polynomial interpolation](polynomial-interpolation.md) does not itself smooth measurement noise. A [linear least squares](linear-least-squares.md) problem with $n+1$ distinct [interpolation nodes](interpolation-node.md) and [polynomial degree](degree-of-a-polynomial.md) at most $n$ does happen to attain zero residual at the same [interpolation polynomial](interpolation-polynomial.md).

**Table of contents**

- [Newton forward interpolation](newton-forward-interpolation.md)
- [Interpolation polynomial](interpolation-polynomial.md)
- [Interpolation nodes from best uniform approximation](interpolation-nodes-from-best-uniform-approximation.md)
- [Interpolation node](interpolation-node.md)
  - [Chebyshev-Lobatto node](chebyshev-lobatto-node.md)
- [Runge's phenomenon](runge-s-phenomenon.md)
- [Lagrange polynomial](lagrange-polynomial.md)
  - [Differentiation weights from nodal evaluations](differentiation-weights-from-nodal-evaluations.md)
  - [Discrete minimax interpolation on ordered nodes](discrete-minimax-interpolation-on-ordered-nodes.md)
  - [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md)
    - [Endpoint derivative signs of Lagrange cardinal polynomials](endpoint-derivative-signs-of-lagrange-cardinal-polynomials.md)
    - [Nodal derivative norm from Lagrange cardinal polynomials](nodal-derivative-norm-from-lagrange-cardinal-polynomials.md)
  - [Barycentric interpolation formula](barycentric-interpolation-formula.md)
- [Divided difference](divided-difference.md)
  - [Divided difference table](divided-difference-table.md)
  - [Symmetry of divided differences](symmetry-of-divided-differences.md)
  - [Omitted-node identities for divided differences](omitted-node-identities-for-divided-differences.md)
  - [Exponential divided difference](exponential-divided-difference.md)
  - [Leibniz rule for divided differences](leibniz-rule-for-divided-differences.md)
  - [Newton polynomial](newton-polynomial.md)
    - [Node order in Newton interpolation](node-order-in-newton-interpolation.md)

## ↑ Ancestors (6)

1. [Interpolation](interpolation-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (41)

- [Barycentric interpolation formula](barycentric-interpolation-formula.md)
- [Bernstein approximation of a corner](bernstein-approximation-of-a-corner.md)
- [Chebyshev-Lobatto node](chebyshev-lobatto-node.md)
- [Chebyshev polynomial](chebyshev-polynomial.md)
- [Conjugate-spectrum proof of Cartan solvability](conjugate-spectrum-proof-of-cartan-solvability.md)
- [Cubic exactness of Simpson's rule](cubic-exactness-of-simpson-s-rule.md)
- [Dual basis](dual-basis.md)
- [Finite field](finite-field.md)
- [Gaussian quadrature](gaussian-quadrature.md)
- [Interpolant](interpolant.md)
- [Interpolation](interpolation-split.md)
- [Newton polynomial](newton-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/6b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-69/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-3/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/18c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/3i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/6b/a/solution.md)
- [Polynomial](polynomial-split.md)
- [Polynomial evaluation](polynomial-evaluation.md)
- [Polynomial interpolation](polynomial-interpolation.md)
- [Remainder of polynomial division](remainder-of-polynomial-division.md)
- [Repeated eigenvalues in the Cayley-Hamilton theorem](repeated-eigenvalues-in-the-cayley-hamilton-theorem.md)
- [Runge's phenomenon](runge-s-phenomenon.md)
- [Shamir's secret sharing](shamir-s-secret-sharing.md)
- [Simpson's rule](simpson-s-rule.md)
- [Spectral projection of a diagonalizable matrix](spectral-projection-of-a-diagonalizable-matrix.md)
- [Symmetry of divided differences](symmetry-of-divided-differences.md)
- [Trace orthogonality nilpotence lemma](trace-orthogonality-nilpotence-lemma.md)
- [Uniqueness of best uniform polynomial approximation](uniqueness-of-best-uniform-polynomial-approximation.md)
