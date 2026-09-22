# Lagrange polynomial

↑ **Parent:** [Polynomial interpolation](polynomial-interpolation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange_polynomial)

The [Lagrange polynomial](lagrange-polynomial.md) writes the [interpolation polynomial](interpolation-polynomial.md) as a [linear combination](linear-combination.md) of [Lagrange cardinal polynomials](lagrange-cardinal-polynomial.md). Each one selects a single [interpolation node](interpolation-node.md), so the data values themselves become the coefficients:

$$
p_n(x)=\sum_{i=0}^n y_i\ell_i(x),\qquad
\ell_i(x)=\prod_{\substack{0\leq j\leq n\\j\ne i}}\frac{x-x_j}{x_i-x_j}.
$$

Distinct [interpolation nodes](interpolation-node.md) make every denominator nonzero. At $x_j$, all terms vanish except $y_j\ell_j(x_j)=y_j$. This gives an explicit construction without solving for [monomial](monomial.md) coefficients. The elegance of the [Lagrange polynomial](lagrange-polynomial.md) is that it builds all constraints into the [basis](basis.md), leaving no equations to solve for the data values.

For $(x_0,x_1,x_2)=(0,1,2)$ and $(y_0,y_1,y_2)=(1,2,5)$, substitution gives

$$
p_2(x)=\frac{(x-1)(x-2)}2-2x(x-2)+\frac{5x(x-1)}2=x^2+1.
$$

At $x=1/2$, the [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md) values are $3/8,3/4,-1/8$, so $p_2(1/2)=3/8+2(3/4)+5(-1/8)=5/4$. A negative [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md) value is allowed: these weights sum to one but need not be [probabilities](probability.md).

The product form is especially useful for deriving [differentiation weights from nodal evaluations](differentiation-weights-from-nodal-evaluations.md) and [quadrature rules](quadrature-rule.md). For repeated numerical evaluation, the [barycentric interpolation formula](barycentric-interpolation-formula.md) reorganizes the same [Lagrange polynomial](lagrange-polynomial.md) into precomputed weights and sums; it avoids evaluating every full product at every argument.

**Table of contents**

- [Differentiation weights from nodal evaluations](differentiation-weights-from-nodal-evaluations.md)
- [Discrete minimax interpolation on ordered nodes](discrete-minimax-interpolation-on-ordered-nodes.md)
- [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md)
  - [Endpoint derivative signs of Lagrange cardinal polynomials](endpoint-derivative-signs-of-lagrange-cardinal-polynomials.md)
  - [Nodal derivative norm from Lagrange cardinal polynomials](nodal-derivative-norm-from-lagrange-cardinal-polynomials.md)
- [Barycentric interpolation formula](barycentric-interpolation-formula.md)

## ↑ Ancestors (7)

1. [Polynomial interpolation](polynomial-interpolation.md)
2. [Interpolation](interpolation.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Barycentric interpolation formula](barycentric-interpolation-formula.md)
- [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md)
- [Lagrange polynomial](lagrange-polynomial.md)
- [Newton-Cotes closed quadrature](newton-cotes-closed-quadrature.md)
- [Newton polynomial](newton-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/14b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/2/solution.md)
- [Polynomial interpolation](polynomial-interpolation.md)
