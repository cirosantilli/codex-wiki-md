# Interpolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interpolation)

Interpolation constructs a [function](function.md) agreeing exactly with prescribed values at sample points. The resulting function is an [interpolant](#interpolant). Choosing a family determines how missing values are filled: [polynomial interpolation](#polynomial-interpolation) selects a [polynomial](polynomial.md), while [linear interpolation](function.md#linear-interpolation) joins adjacent samples by straight segments. The [McShane extension theorem](real-analysis.md#mcshane-extension-theorem) instead permits any [Lipschitz function](real-analysis.md#lipschitz-continuity) with a specified bound and provides envelopes controlling all allowed choices.

**Table of contents**

- [Extrapolation](#extrapolation)
- [Interpolant](#interpolant)
- [Polynomial interpolation](#polynomial-interpolation)
  - [Newton forward interpolation](#newton-forward-interpolation)
  - [Interpolation polynomial](#interpolation-polynomial)
  - [Interpolation nodes from best uniform approximation](#interpolation-nodes-from-best-uniform-approximation)
  - [Interpolation node](#interpolation-node)
    - [Chebyshev-Lobatto node](#chebyshev-lobatto-node)
  - [Runge's phenomenon](#runge-s-phenomenon)
  - [Lagrange polynomial](#lagrange-polynomial)
    - [Differentiation weights from nodal evaluations](#differentiation-weights-from-nodal-evaluations)
    - [Discrete minimax interpolation on ordered nodes](#discrete-minimax-interpolation-on-ordered-nodes)
    - [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial)
      - [Endpoint derivative signs of Lagrange cardinal polynomials](#endpoint-derivative-signs-of-lagrange-cardinal-polynomials)
      - [Nodal derivative norm from Lagrange cardinal polynomials](#nodal-derivative-norm-from-lagrange-cardinal-polynomials)
    - [Barycentric interpolation formula](#barycentric-interpolation-formula)
  - [Divided difference](#divided-difference)
    - [Divided difference table](#divided-difference-table)
    - [Symmetry of divided differences](#symmetry-of-divided-differences)
    - [Omitted-node identities for divided differences](#omitted-node-identities-for-divided-differences)
    - [Exponential divided difference](#exponential-divided-difference)
    - [Leibniz rule for divided differences](#leibniz-rule-for-divided-differences)
    - [Newton polynomial](#newton-polynomial)
      - [Node order in Newton interpolation](#node-order-in-newton-interpolation)

## Extrapolation

↑ **Parent:** [Interpolation](interpolation.md)

Estimating values beyond the range of the supplied sample points. For two distinct points $P,Q$, the [affine combination](geometry-and-topology.md#affine-combination) $(1-t)P+tQ$ lies beyond an endpoint of their [line segment](convex-set.md#line-segment) when $t<0$ or $t>1$. The construction specifies an extension of the chosen model; it does not show that an unknown underlying [function](function.md) follows that extension.

## Interpolant

↑ **Parent:** [Interpolation](interpolation.md)

An interpolant is a [function](function.md) satisfying the prescribed sample conditions $g(x_i)=y_i$. It agrees with the data exactly, but need not agree with an unknown underlying function between samples. The [polynomial interpolation](#polynomial-interpolation) example shows that a family or a [polynomial degree](polynomial.md#degree-of-a-polynomial) restriction can supply uniqueness; the [McShane extension theorem](real-analysis.md#mcshane-extension-theorem) shows a useful nonunique alternative.

## Polynomial interpolation

↑ **Parent:** [Interpolation](interpolation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_interpolation)

[Polynomial interpolation](#polynomial-interpolation) constructs a [polynomial](polynomial.md) that passes exactly through prescribed data. Given $n+1$ distinct [interpolation nodes](#interpolation-node) $x_0,\ldots,x_n$ and values $y_0,\ldots,y_n$, there is exactly one [interpolation polynomial](#interpolation-polynomial) $p_n$ of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$ with $p_n(x_i)=y_i$ for every $i$. The values may be samples $y_i=f(x_i)$ of a [function](function.md), but no knowledge of that [function](function.md) between the [interpolation nodes](#interpolation-node) is needed to construct $p_n$. The [Lagrange polynomial](#lagrange-polynomial) and [Newton polynomial](#newton-polynomial) are two representations of this same answer.[Toby A. Driscoll and Richard J. Braun, Fundamentals of Numerical Computation, §9.1, Theorems 9.1.1–9.1.2](https://fncbook.com/polynomial/)

For example, the three data points $(0,1),(1,2),(2,5)$ give the [quadratic polynomial](polynomial.md#quadratic-polynomial)

$$
p_2(x)=x^2+1,\qquad p_2(0)=1,\quad p_2(1)=2,\quad p_2(2)=5.
$$

Thus [polynomial interpolation](#polynomial-interpolation) supplies $p_2(1/2)=5/4$ as an intermediate value. Whether this approximates an unknown underlying [function](function.md) well is a separate question about [polynomial interpolation error](algebra.md#polynomial-interpolation-error).

Both hypotheses in the uniqueness statement matter. The [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial) prove existence constructively. If two [polynomials](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$ fit the data, their difference has $n+1$ distinct [roots of a polynomial](polynomial.md#root-of-a-polynomial), so it must be zero. Repeated [interpolation nodes](#interpolation-node) with conflicting values have no solution, and repeated equal values provide no additional independent condition; prescribed [derivatives](calculus.md#derivative) instead lead to [Hermite interpolation](algebra.md#hermite-interpolation). Without the [polynomial degree](polynomial.md#degree-of-a-polynomial) restriction there are infinitely many solutions:

$$
p(x)=p_n(x)+q(x)\prod_{i=0}^n(x-x_i),
$$

where $q$ is any [polynomial](polynomial.md). By the [factor theorem](polynomial.md#factor-theorem), this describes every [polynomial](polynomial.md) fitting the same data. In the example, $x^2+1+c\,x(x-1)(x-2)$ fits for every $c$, but at $x=1/2$ its value is $5/4+3c/8$; exact agreement at the three [interpolation nodes](#interpolation-node) alone says nothing about that intermediate value.

The usefulness of [polynomial interpolation](#polynomial-interpolation) is that data become an explicit [function](function.md) whose values, [derivatives](calculus.md#derivative), and [integrals](integral.md) can be calculated. Differentiating or integrating the [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial) produces [differentiation weights from nodal evaluations](#differentiation-weights-from-nodal-evaluations) or a [quadrature rule](numerical-integration.md#quadrature-rule). Exact passage through observations is the defining constraint. In [polynomial regression](linear-regression.md#polynomial-regression), [linear least squares](probability-and-statistics.md#linear-least-squares) instead chooses a [polynomial degree](polynomial.md#degree-of-a-polynomial) and minimizes a sum of squared residuals, generally without passing through every observation. Interpolating noisy values reproduces their errors at the [interpolation nodes](#interpolation-node) and can amplify them between [interpolation nodes](#interpolation-node); [polynomial interpolation](#polynomial-interpolation) does not itself smooth measurement noise. A [linear least squares](probability-and-statistics.md#linear-least-squares) problem with $n+1$ distinct [interpolation nodes](#interpolation-node) and [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$ does happen to attain zero residual at the same [interpolation polynomial](#interpolation-polynomial).

### Newton forward interpolation

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

For equally spaced nodes $x_0,x_0+h,\ldots,x_0+dh$, write $t=(x-x_0)/h$. The interpolating [polynomial](polynomial.md) is $P(x)=\sum_{j=0}^d\binom tj\Delta_h^j f(x_0)$. A table of [forward differences](finite-difference.md#forward-difference) supplies its coefficients; for a [polynomial](polynomial.md) of degree at most $d$, the formula reproduces the function exactly.

### Interpolation polynomial

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

An interpolation polynomial for distinct nodes $x_0,\ldots,x_n$ and prescribed values $y_0,\ldots,y_n$ is a [polynomial](polynomial.md) $p$ satisfying $p(x_i)=y_i$. There is a unique such [polynomial](polynomial.md) of degree at most $n$: the [Lagrange interpolation polynomial](#lagrange-polynomial) constructs it explicitly, and uniqueness follows because a nonzero degree-at-most-$n$ difference cannot have $n+1$ distinct roots. [Newton interpolation polynomials](#newton-polynomial) express the same object using [divided differences](#divided-difference).

### Interpolation nodes from best uniform approximation

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

For a real [continuous function](calculus.md#continuous-function) on a compact interval, choose its [best uniform approximation](uniform-approximation.md#best-uniform-approximation) $p_n^*$ of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$. If its error is nonzero, the [Chebyshev alternation theorem](uniform-approximation.md#equioscillation-theorem) supplies $n+2$ ordered alternating extrema. The [intermediate value theorem](calculus.md#intermediate-value-theorem) gives a zero of $f-p_n^*$ in each intervening interval. At these $n+1$ distinct points, the [polynomial interpolant](#lagrange-polynomial) is exactly $p_n^*$. If the best error is zero, arbitrary distinct nodes suffice. The [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) shows that these function-dependent interpolants converge uniformly. The nodes depend on the target function; the conclusion does not provide one universal node sequence for every continuous target.

### Interpolation node

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

An [interpolation node](#interpolation-node) is an argument value $x_i$ at which an [interpolation polynomial](#interpolation-polynomial) must take a prescribed value $y_i$. The [interpolation nodes](#interpolation-node) specify where the constraints apply; the values specify how high the graph must pass there. In the three-point example, the [interpolation nodes](#interpolation-node) are $0,1,2$, while the prescribed values are $1,2,5$. Changing the [interpolation nodes](#interpolation-node) changes the [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial) and the [polynomial interpolation error](algebra.md#polynomial-interpolation-error), even if their number stays fixed.

#### Chebyshev-Lobatto node

↑ **Parent:** [Interpolation node](#interpolation-node)

For $n\geq1$, the $n+1$ [Chebyshev-Lobatto nodes](#chebyshev-lobatto-node) are the [extrema](mathematical-optimization.md#maximum-and-minimum) of the [Chebyshev polynomial](numerical-analysis.md#chebyshev-polynomial) $T_n$ on $[-1,1]$, including both endpoints: $T_n(x_k)=(-1)^k$. Imagine $n+1$ equally spaced angles on a [semicircle](topology.md#semicircle) and project their points onto the horizontal axis. The [interpolation nodes](#interpolation-node) crowd near $-1$ and $1$ because equal angular steps have smaller horizontal projections there. Reversing the order gives the same set. These are distinct from the [roots of a polynomial](polynomial.md#root-of-a-polynomial) $\cos((2k+1)\pi/(2n+2))$ of $T_{n+1}$, which omit the endpoints. Driscoll and Braun call this endpoint-including family Chebyshev points of the second kind or Chebyshev extreme points.[Driscoll and Braun, Fundamentals of Numerical Computation, §9.3.2, equation 9.3.2](https://fncbook.com/python/stability-1/)

On an interval $[a,b]$, use $x_k=(a+b)/2+(b-a)\cos(k\pi/n)/2$. The [Runge phenomenon](#runge-s-phenomenon) example compares [polynomial interpolation](#polynomial-interpolation) at eleven [Chebyshev-Lobatto nodes](#chebyshev-lobatto-node) with eleven equally spaced [interpolation nodes](#interpolation-node). The distinction matters whenever sampling locations are a choice rather than fixed observations.

<h3 id="runge-s-phenomenon">Runge's phenomenon</h3>

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Runge's_phenomenon)

The [Runge phenomenon](#runge-s-phenomenon) is the failure of increasing-degree [polynomial interpolation](#polynomial-interpolation) at equally spaced [interpolation nodes](#interpolation-node) to converge to some smooth target [functions](function.md), with large oscillations near the ends of the interval. It is a property of the approximation problem, and can occur even with exact arithmetic. A numerically stable evaluation method cannot remove it. Endpoint clustering, as in [Chebyshev-Lobatto nodes](#chebyshev-lobatto-node), changes the approximation problem and can greatly improve it.[Driscoll and Braun, Fundamentals of Numerical Computation, §9.3.1–9.3.2](https://fncbook.com/python/stability-1/)

Take $f(x)=1/(1+25x^2)$ on $[-1,1]$ and [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $10$. Use either $x_k=-1+k/5$ or $x_k=\cos(k\pi/10)$ for $k=0,\ldots,10$. Each [interpolation polynomial](#interpolation-polynomial) passes through all eleven of its own samples, yet the first has severe endpoint oscillations and the second stays much closer to the target [function](function.md). Evaluating both by the [barycentric interpolation formula](#barycentric-interpolation-formula) on $20{,}001$ equally spaced points, including the endpoints, gives sampled maximum absolute errors of approximately $1.915659$ and $0.132197$, respectively: about a $14.49$-fold reduction. These are maxima over the stated grid, not certified maxima over the continuous interval. The generator separately checks exact reproduction of all stored nodal values.

<a id="image-degree-10-interpolation-of-the-runge-function-at-equally-spaced-and-chebyshev-lobatto-nodes-with-absolute-errors"></a>
![](interpolation-node-placement.png)

**[Figure 1](#image-degree-10-interpolation-of-the-runge-function-at-equally-spaced-and-chebyshev-lobatto-nodes-with-absolute-errors). Degree-10 interpolation of the Runge function at equally spaced and Chebyshev-Lobatto nodes, with absolute errors**.

The [polynomial interpolation error](algebra.md#polynomial-interpolation-error) formula explains why [interpolation nodes](#interpolation-node) enter the analysis. If $f$ has $n+1$ continuous [derivatives](calculus.md#derivative) on an interval containing $x$ and all the [interpolation nodes](#interpolation-node), then for a suitable $\xi_x$ in that interval,

$$
f(x)-p_n(x)=\frac{f^{(n+1)}(\xi_x)}{(n+1)!}\prod_{i=0}^n(x-x_i).
$$

At an [interpolation node](#interpolation-node) the error is zero directly. Away from the [interpolation nodes](#interpolation-node), both the product and the high-order [derivative](calculus.md#derivative) matter. A short proof applies [Rolle's theorem](calculus.md#rolle-theorem) repeatedly to $f(t)-p_n(t)-[f(x)-p_n(x)]\prod_i(t-x_i)/\prod_i(x-x_i)$, which vanishes at $n+2$ distinct points.[Driscoll and Braun, Fundamentals of Numerical Computation, §9.1.2, Theorem 9.1.3](https://fncbook.com/polynomial/)

The successful comparison here does not assert that [Chebyshev-Lobatto nodes](#chebyshev-lobatto-node) solve every approximation problem for every [function](function.md). The [derivatives](calculus.md#derivative), the [polynomial degree](polynomial.md#degree-of-a-polynomial), and measurement errors still matter. The [Lebesgue constant of interpolation](uniform-approximation.md#lebesgue-constant-of-interpolation) measures worst-case amplification of nodal errors, while the [polynomial reproduction error bound](uniform-approximation.md#polynomial-reproduction-error-bound) relates interpolation to the [best uniform approximation](uniform-approximation.md#best-uniform-approximation) available at that [polynomial degree](polynomial.md#degree-of-a-polynomial).

### Lagrange polynomial

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange_polynomial)

The [Lagrange polynomial](#lagrange-polynomial) writes the [interpolation polynomial](#interpolation-polynomial) as a [linear combination](vector-space.md#linear-combination) of [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial). Each one selects a single [interpolation node](#interpolation-node), so the data values themselves become the coefficients:

$$
p_n(x)=\sum_{i=0}^n y_i\ell_i(x),\qquad
\ell_i(x)=\prod_{\substack{0\leq j\leq n\\j\ne i}}\frac{x-x_j}{x_i-x_j}.
$$

Distinct [interpolation nodes](#interpolation-node) make every denominator nonzero. At $x_j$, all terms vanish except $y_j\ell_j(x_j)=y_j$. This gives an explicit construction without solving for [monomial](polynomial.md#monomial) coefficients. The elegance of the [Lagrange polynomial](#lagrange-polynomial) is that it builds all constraints into the [basis](vector-space.md#basis), leaving no equations to solve for the data values.

For $(x_0,x_1,x_2)=(0,1,2)$ and $(y_0,y_1,y_2)=(1,2,5)$, substitution gives

$$
p_2(x)=\frac{(x-1)(x-2)}2-2x(x-2)+\frac{5x(x-1)}2=x^2+1.
$$

At $x=1/2$, the [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) values are $3/8,3/4,-1/8$, so $p_2(1/2)=3/8+2(3/4)+5(-1/8)=5/4$. A negative [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) value is allowed: these weights sum to one but need not be [probabilities](probability-theory.md#probability).

The product form is especially useful for deriving [differentiation weights from nodal evaluations](#differentiation-weights-from-nodal-evaluations) and [quadrature rules](numerical-integration.md#quadrature-rule). For repeated numerical evaluation, the [barycentric interpolation formula](#barycentric-interpolation-formula) reorganizes the same [Lagrange polynomial](#lagrange-polynomial) into precomputed weights and sums; it avoids evaluating every full product at every argument.

#### Differentiation weights from nodal evaluations

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

At distinct nodes $a_0,\ldots,a_n$, the [Lagrange interpolation polynomial](#lagrange-polynomial) has basis $\ell_j(x)=\prod_{i\ne j}(x-a_i)/(a_j-a_i)$. Differentiating its exact expression for a polynomial of degree at most $n$ gives the displayed weights. Their uniqueness follows because the nodal evaluations form a basis of the [dual space](dual-space.md) of that polynomial space.

#### Discrete minimax interpolation on ordered nodes

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

For $n+2$ increasingly ordered nodes $y_j$, let $r_j$ be their [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial), $t=\sum f(y_j)r_j$, and $r=\sum(-1)^jr_j$. The leading coefficient of $r_j$ has sign $(-1)^{n+2-j}$, so all summands in the leading coefficient of $r$ have the same nonzero sign. There is a unique $\lambda$ canceling degree $n+1$ in $t-\lambda r$. Its errors at the nodes are $\lambda(-1)^j$, and a better degree-at-most-$n$ approximation would have a difference polynomial with at least $n+1$ roots. Thus it minimizes the maximum node error. Increasing order matters: for the permutation $(0,1/3,1,2/3)$ the alternating interpolant is already the quadratic $-1+9x(1-x)$, so the leading-coefficient assertion for $n=2$ fails.

#### Lagrange cardinal polynomial

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

For distinct [interpolation nodes](#interpolation-node) $x_0,\ldots,x_n$, the [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) $\ell_i$ has value one at its own [interpolation node](#interpolation-node) and zero at every other [interpolation node](#interpolation-node):

$$
\ell_i(x)=\prod_{j\ne i}\frac{x-x_j}{x_i-x_j},\qquad
\ell_i(x_j)=\delta_{ij}=
\begin{cases}1,&i=j,\\0,&i\ne j.\end{cases}
$$

Here $\delta_{ij}$ is the [Kronecker delta](multilinear-algebra.md#kronecker-delta). These [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial) form a [basis](vector-space.md#basis) of the [vector space](vector-space.md) of [polynomials](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$: every such [polynomial](polynomial.md) has the unique expansion $p(x)=\sum_i p(x_i)\ell_i(x)$. The nodal evaluation [linear functionals](dual-space.md#linear-functional) $E_j(p)=p(x_j)$ form the [dual basis](dual-space.md#dual-basis), since $E_j(\ell_i)=\delta_{ij}$.

For the [interpolation nodes](#interpolation-node) $0,1,2$, the three [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial) are

$$
\ell_0(x)=\frac{(x-1)(x-2)}2,\qquad
\ell_1(x)=-x(x-2),\qquad
\ell_2(x)=\frac{x(x-1)}2.
$$

Their values on the [interpolation nodes](#interpolation-node) are the rows of the [identity matrix](vector-space.md#identity-matrix). In the figure, each colored curve passes through its own unit-height marker and through zero at the other two [interpolation nodes](#interpolation-node). Multiplying the curves by the data $1,2,5$ and adding gives the [Lagrange polynomial](#lagrange-polynomial) $x^2+1$.

<a id="image-lagrange-cardinal-polynomials-at-nodes-0-1-2-and-their-weighted-sum-interpolating-values-1-2-5"></a>
![](lagrange-interpolation-cardinals.png)

**[Figure 2](#image-lagrange-cardinal-polynomials-at-nodes-0-1-2-and-their-weighted-sum-interpolating-values-1-2-5). Lagrange cardinal polynomials at nodes 0, 1, 2 and their weighted sum interpolating values 1, 2, 5**.

Since the constant [polynomial](polynomial.md) one interpolates data values all equal to one, uniqueness gives $\sum_i\ell_i(x)=1$. Nevertheless, $\ell_2(1/2)=-1/8$, so [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial) need not stay between zero and one. If a single data value $y_i$ changes by $\varepsilon$, the [interpolation polynomial](#interpolation-polynomial) changes by exactly $\varepsilon\ell_i(x)$. Thus a [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) describes how one observation influences the entire graph, and $\sum_i|\ell_i(x)|$ controls the worst amplification of simultaneous data errors at $x$; its maximum is the [Lebesgue constant of interpolation](uniform-approximation.md#lebesgue-constant-of-interpolation).

##### Endpoint derivative signs of Lagrange cardinal polynomials

↑ **Parent:** [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial)

At decreasing distinct [interpolation nodes](#interpolation-node) $1\ge t_0>\cdots>t_n\ge-1$, the [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) $L_i(x)=\prod_{j\ne i}(x-t_j)/\prod_{j\ne i}(t_i-t_j)$ has denominator sign $(-1)^i$. For $1\le k\le n$, its numerator's $k$th [derivative](calculus.md#derivative) at one is $k!$ times a sum of products of $n-k$ nonnegative factors $1-t_j$. At most one factor vanishes, and at least one product avoids it, so that sum is strictly positive. The same alternating nodal signs therefore maximize every endpoint derivative simultaneously.

##### Nodal derivative norm from Lagrange cardinal polynomials

↑ **Parent:** [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial)

At distinct [interpolation nodes](#interpolation-node), differentiating [Lagrange interpolation](#lagrange-polynomial) gives $p^{(k)}(x)=\sum_i p(t_i)\ell_i^{(k)}(x)$. The [triangle inequality](topological-analysis.md#triangle-inequality) gives the displayed upper bound, attained by prescribing each nodal value to be the sign of the corresponding [derivative](calculus.md#derivative) weight. For increasingly ordered real nodes, the [Markov interlacing lemma](polynomial.md#markov-interlacing-lemma) and [monotonicity of polynomial critical points in their roots](polynomial.md#monotonicity-of-polynomial-critical-points-in-their-roots) imply that $(-1)^i\ell_i^{(k)}(x)$ has at most one sign change, ignoring zero weights. Thus an extremizer has alternating nodal signs with at most one reversal of that alternating pattern. This reduces a choice among $2^{n+1}$ sign patterns to $n+1$ candidate [polynomials](polynomial.md).

#### Barycentric interpolation formula

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

The [barycentric interpolation formula](#barycentric-interpolation-formula) evaluates the same [Lagrange polynomial](#lagrange-polynomial) using weights that depend only on the distinct [interpolation nodes](#interpolation-node):

$$
w_i=\frac1{\prod_{j\ne i}(x_i-x_j)},\qquad
p_n(x)=\frac{\displaystyle\sum_{i=0}^n\frac{w_i y_i}{x-x_i}}
{\displaystyle\sum_{i=0}^n\frac{w_i}{x-x_i}},\qquad x\ne x_i.
$$

At $x=x_i$, return $y_i$ directly, before dividing; the formula has [removable singularities](isolated-singularity.md#removable-singularity) at the [interpolation nodes](#interpolation-node). Multiplying every $w_i$ by the same nonzero constant leaves the answer unchanged. Driscoll and Braun derive this formula as a more efficient, numerically stable way to evaluate [polynomial interpolation](#polynomial-interpolation).[Driscoll and Braun, Fundamentals of Numerical Computation, §9.2, Theorem 9.2.1 and Algorithm 9.2.1](https://fncbook.com/barycentric/)

For the [interpolation nodes](#interpolation-node) $0,1,2$, the weights are $(1/2,-1,1/2)$, or equivalently $(1,-2,1)$. With data $(1,2,5)$, at $x=1/2$ the denominator using the latter weights is $2+4-2/3=16/3$ and the numerator is $2+8-10/3=20/3$, giving $p_2(1/2)=5/4$ again. For eleven [interpolation nodes](#interpolation-node) in the [Runge phenomenon](#runge-s-phenomenon) figure, the generator computes the weights by the direct products above and returns stored values exactly at every [interpolation node](#interpolation-node).

The direct products require $O(n^2)$ [arithmetic operations](numerical-analysis.md#arithmetic-operation) once; each subsequent value uses $O(n)$ [arithmetic operations](numerical-analysis.md#arithmetic-operation). Here $O$ denotes [Big O notation](real-analysis.md#big-o-notation). At large [polynomial degree](polynomial.md#degree-of-a-polynomial) or on poorly scaled intervals, forming these products can exceed the range of [floating-point arithmetic](floating-point-arithmetic.md); normalization or specialized weight formulas may be needed. Stable evaluation also cannot cure sensitivity intrinsic to the chosen [interpolation nodes](#interpolation-node), measured by the [Lebesgue constant of interpolation](uniform-approximation.md#lebesgue-constant-of-interpolation), or the approximation failure in the [Runge phenomenon](#runge-s-phenomenon).

### Divided difference

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divided_difference)

For $k+1$ distinct [interpolation nodes](#interpolation-node), the [divided difference](#divided-difference) $f[x_0,\ldots,x_k]$ is the coefficient of $x^k$ in the [interpolation polynomial](#interpolation-polynomial) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $k$ through those [interpolation nodes](#interpolation-node). It is the [leading coefficient](polynomial.md#leading-coefficient-of-a-polynomial) when that [polynomial degree](polynomial.md#degree-of-a-polynomial) is exactly $k$, and zero when it is smaller. Explicitly,

$$
f[x_0,\ldots,x_k]
=\sum_{j=0}^k\frac{f(x_j)}
{\prod_{i\ne j}(x_j-x_i)}.
$$

starting with $f[x_i]=f(x_i)$. The [divided differences](#divided-difference) obey the recurrence

$$
f[x_0,\ldots,x_k]
=\frac{f[x_1,\ldots,x_k]-f[x_0,\ldots,x_{k-1}]}
{x_k-x_0}.
$$

For data $f(0)=1$, $f(1)=2$, $f(2)=5$, the first [divided differences](#divided-difference) are $f[0,1]=(2-1)/(1-0)=1$ and $f[1,2]=(5-2)/(2-1)=3$. The second [divided difference](#divided-difference) is $f[0,1,2]=(3-1)/(2-0)=1$, the [leading coefficient](polynomial.md#leading-coefficient-of-a-polynomial) of $x^2+1$. The first [divided difference](#divided-difference) is the slope of a [secant line](euclidean-geometry.md#secant-line); higher [divided differences](#divided-difference) supply successive coefficients for the [Newton polynomial](#newton-polynomial).

#### Divided difference table

↑ **Parent:** [Divided difference](#divided-difference)

A [divided difference table](#divided-difference-table) arranges [divided differences](#divided-difference) by starting [interpolation node](#interpolation-node) $i$ and order $k$. Its base column is $D_{i,0}=f(x_i)$; every later entry uses two neighboring entries from the previous column:

$$
D_{i,k}=\frac{D_{i+1,k-1}-D_{i,k-1}}{x_{i+k}-x_i},\qquad
1\leq k\leq n,\quad 0\leq i\leq n-k.
$$

The denominator spans all $k+1$ [interpolation nodes](#interpolation-node) of that entry, even though the numerator uses adjacent table entries. The [interpolation nodes](#interpolation-node) must be distinct; they need not be equally spaced or sorted.[NIST Digital Library of Mathematical Functions; §3.3(iii), equation 3.3.34: initial values and divided-difference recurrence for distinct nodes](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/3-3-interpolation)

Take the [polynomial](polynomial.md) $f(x)=x^3-2x+1$ at the [interpolation nodes](#interpolation-node) $(-1,0,2,3)$, giving values $(2,1,5,22)$. Its [divided difference table](#divided-difference-table) is

$$
\begin{array}{c|r|r|r|r}
x_i&D_{i,0}&D_{i,1}&D_{i,2}&D_{i,3}\\\hline
-1&2&-1&1&1\\
0&1&2&5&\\
2&5&17&&\\
3&22&&&
\end{array}
$$

The first [divided differences](#divided-difference) are $(1-2)/(0+1)=-1$, $(5-1)/(2-0)=2$, and $(22-5)/(3-2)=17$. The second [divided differences](#divided-difference) use the wider spans: $(2+1)/(2+1)=1$ and $(17-2)/(3-0)=5$. The third [divided difference](#divided-difference) is $(5-1)/(3+1)=1$. Reading the top row gives the [Newton polynomial](#newton-polynomial) coefficients $(2,-1,1,1)$, rather than all the entries in any one column.

The resulting [Newton polynomial](#newton-polynomial) grows through four partial [interpolants](#interpolant):

$$
\begin{aligned}
p_0(x)&=2,\\
p_1(x)&=2-(x+1)=1-x,\\
p_2(x)&=2-(x+1)+(x+1)x=x^2+1,\\
p_3(x)&=2-(x+1)+(x+1)x+(x+1)x(x-2)=x^3-2x+1.
\end{aligned}
$$

At $x=2$, $p_1(2)=-1$ misses $f(2)=5$ by $6$; the correction $(x+1)x$ supplies exactly $6$ there and vanishes at the earlier [interpolation nodes](#interpolation-node) $-1,0$. At $x=3$, $p_2(3)=10$ misses $f(3)=22$ by $12$; the correction $(x+1)x(x-2)$ supplies exactly $12$ there and vanishes at all three earlier [interpolation nodes](#interpolation-node). Each added term therefore preserves the previous agreements while satisfying the next one.

<a id="image-divided-difference-triangle-and-successive-newton-interpolants-for-the-constructed-polynomial-x-cubed-minus-2x-plus-1"></a>
![](divided-difference-triangle-newton-stages.png)

**[Figure 3](#image-divided-difference-triangle-and-successive-newton-interpolants-for-the-constructed-polynomial-x-cubed-minus-2x-plus-1). Divided-difference triangle and successive Newton interpolants for the constructed polynomial x cubed minus 2x plus 1**.

For $n+1$ [interpolation nodes](#interpolation-node), the triangle contains $n+(n-1)+\cdots+1=n(n+1)/2$ recurrence steps. Once the top row is known, nested evaluation of the [Newton polynomial](#newton-polynomial) uses only $n$ multiplications and $n$ additions per argument. The triangle organizes the work; the factors explain why the construction works.

#### Symmetry of divided differences

↑ **Parent:** [Divided difference](#divided-difference)

A [divided difference](#divided-difference) depends on the chosen [interpolation nodes](#interpolation-node) and their data, but is unchanged by any [permutation](combinatorics.md#permutation) $\sigma$ of those same [interpolation nodes](#interpolation-node). The explicit [sum](arithmetic.md#sum) in [divided difference](#divided-difference) makes this visible: a [permutation](combinatorics.md#permutation) merely rearranges its summands.[NIST Digital Library of Mathematical Functions; §3.3(iii), equation 3.3.35: symmetric explicit expression](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/3-3-interpolation)

There is also a short explanation using [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial). The [coefficient](vector-space.md#coefficient) of $x^k$ in the $j$th [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) is $1/\prod_{i\ne j}(x_j-x_i)$. Taking that [coefficient](vector-space.md#coefficient) in their weighted [sum](arithmetic.md#sum) gives exactly the explicit [divided difference](#divided-difference) formula. Since [polynomial interpolation](#polynomial-interpolation) has a unique answer for a fixed set of distinct [interpolation nodes](#interpolation-node), this [coefficient](vector-space.md#coefficient) cannot depend on their ordering. If the [interpolation polynomial](#interpolation-polynomial) has [polynomial degree](polynomial.md#degree-of-a-polynomial) below $k$, the [coefficient](vector-space.md#coefficient) is zero.

For the four-point example in [divided difference table](#divided-difference-table), every ordering gives third [divided difference](#divided-difference) $1$. This does not make every [Newton polynomial](#newton-polynomial) coefficient invariant: $f[-1,0]=-1$ whereas $f[3,2]=17$, because these use different pairs of [interpolation nodes](#interpolation-node). Even at second order, $f[-1,0,2]=1$ and $f[3,2,0]=5$ use different triples. The [node order in Newton interpolation](#node-order-in-newton-interpolation) determines which subsets occur along the top row.

#### Omitted-node identities for divided differences

↑ **Parent:** [Divided difference](#divided-difference)

For distinct [interpolation nodes](#interpolation-node), write $D_i$ for the [divided difference](#divided-difference) with $x_i$ omitted. Symmetry and the divided-difference recurrence give the displayed identity. Consequently, for $0<i<n$,

$$
D_i=\frac{x_i-x_0}{x_n-x_0}D_n+\frac{x_n-x_i}{x_n-x_0}D_0.
$$

The identity is algebraic and does not require the nodes to be ordered; the coefficients need not be nonnegative.

#### Exponential divided difference

↑ **Parent:** [Divided difference](#divided-difference)

The displayed integral is $(e^{t\beta}-e^{t\gamma})/(\beta-\gamma)$ for distinct exponents and $te^{t\gamma}$ when they coincide. The latter is the continuous limit, so a zero denominator is a removable singularity. This quantity appears in [variation-of-constants formula](functional-analysis.md#variation-of-constants-formula) estimates of [matrix](vector-space.md#matrix) evolution and avoids omitting an equal-exponent case.

#### Leibniz rule for divided differences

↑ **Parent:** [Divided difference](#divided-difference)

For $h=fg$,

$$
h[t_0,\ldots,t_k]=\sum_{m=0}^kf[t_0,\ldots,t_m]g[t_m,\ldots,t_k].
$$

#### Newton polynomial

↑ **Parent:** [Divided difference](#divided-difference)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton_polynomial)

The [Newton polynomial](#newton-polynomial) expresses the [interpolation polynomial](#interpolation-polynomial) in products that successively vanish at all previously used [interpolation nodes](#interpolation-node). With $y_i=f(x_i)$, the coefficients are [divided differences](#divided-difference):

$$
p_n(x)=f(x_0)+\sum_{k=1}^nf[x_0,\ldots,x_k]
\prod_{i=0}^{k-1}(x-x_i).
$$

A triangular [divided difference](#divided-difference) table computes all its coefficients using exactly $n(n+1)/2$ divisions. The [Newton polynomial](#newton-polynomial) and the [Lagrange polynomial](#lagrange-polynomial) have the same [polynomial degree](polynomial.md#degree-of-a-polynomial) bound and the same nodal values, hence are equal by uniqueness of [polynomial interpolation](#polynomial-interpolation).

For $f(0)=1$, $f(1)=2$, $f(2)=5$, the complete [divided difference](#divided-difference) table is

$$
\begin{array}{c|r|r|r}
x_i&f[x_i]&f[x_i,x_{i+1}]&f[x_i,x_{i+1},x_{i+2}]\\\hline
0&1&1&1\\
1&2&3&\\
2&5&&
\end{array}
$$

The first [divided differences](#divided-difference) are $1$ and $3$, and their [divided difference](#divided-difference) is $(3-1)/(2-0)=1$. Reading the top entries gives

$$
p_2(x)=1+1(x-0)+1(x-0)(x-1)=1+x+x(x-1)=x^2+1.
$$

The initial term fits $(0,1)$; adding $x$ also fits $(1,2)$; adding $x(x-1)$ fits $(2,5)$ while leaving the first two data values unchanged. This is the practical beauty of the [Newton polynomial](#newton-polynomial): each new correction respects all previous interpolation constraints.

If a new distinct [interpolation node](#interpolation-node) $x_{n+1}$ with value $y_{n+1}$ arrives, append one term:

$$
p_{n+1}(x)=p_n(x)+c\prod_{i=0}^n(x-x_i),\qquad
c=\frac{y_{n+1}-p_n(x_{n+1})}{\prod_{i=0}^n(x_{n+1}-x_i)}.
$$

For example, appending $(3,11)$ to the three-point data gives $c=(11-10)/(3\cdot2\cdot1)=1/6$, hence $p_3(x)=x^2+1+x(x-1)(x-2)/6$. Changing the order of the [interpolation nodes](#interpolation-node) changes the [Newton polynomial](#newton-polynomial) coefficients and products, but not the final [interpolation polynomial](#interpolation-polynomial) in exact arithmetic.

The products also permit nested evaluation analogous to [Horner's method](polynomial.md#horner-s-method). If $a_k=f[x_0,\ldots,x_k]$, start with $b_n=a_n$ and work backwards by $b_k=a_k+(x-x_k)b_{k+1}$; the answer is $b_0$. The three-point example becomes $1+x[1+(x-1)]$, needing two multiplications for each evaluation. This organization is useful when adding observations incrementally or evaluating a stored [Newton polynomial](#newton-polynomial) many times; the [Runge phenomenon](#runge-s-phenomenon) still depends on the [interpolation nodes](#interpolation-node) rather than on which representation is used.

To justify the update formula, its added [product](arithmetic.md#product-of-numbers) vanishes at every previous [interpolation node](#interpolation-node). Choosing $c$ by the new residual forces agreement at $x_{n+1}$, so uniqueness of [polynomial interpolation](#polynomial-interpolation) identifies the result. For $n\geq0$, $p_n$ has [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$, and the added [product](arithmetic.md#product-of-numbers) has [leading coefficient](polynomial.md#leading-coefficient-of-a-polynomial) one. Thus the new [coefficient](vector-space.md#coefficient) $c$ is exactly $f[x_0,\ldots,x_{n+1}]$. The initial state is $p_0(x)=f(x_0)$, with the [empty product](arithmetic.md#empty-product) interpreted as one.[NIST Digital Library of Mathematical Functions; §3.3(iv), equation 3.3.38 and the following new-point update paragraph](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/3-3-interpolation)

Appending $(4,57)$ to the four-point example in [divided difference table](#divided-difference-table) leaves the [Newton polynomial](#newton-polynomial) unchanged: $p_3(4)=57$, so the new fourth [divided difference](#divided-difference) is zero. If the appended value is instead $58$, the new [coefficient](vector-space.md#coefficient) is

$$
c=\frac{58-57}{(4+1)\cdot4\cdot(4-2)\cdot(4-3)}=\frac1{40},\qquad
p_4(x)=x^3-2x+1+\frac{(x+1)x(x-2)(x-3)}{40}.
$$

This [polynomial](polynomial.md) still takes values $2,1,5,22$ at the original [interpolation nodes](#interpolation-node), and now takes value $58$ at $4$. A zero update is a valid completed step: adding another exact sample of the original [polynomial](polynomial.md) need not increase the [polynomial degree](polynomial.md#degree-of-a-polynomial).

##### Node order in Newton interpolation

↑ **Parent:** [Newton polynomial](#newton-polynomial)

Reordering the [interpolation nodes](#interpolation-node) changes the successive subsets used for the [divided differences](#divided-difference) and the factors of the [Newton polynomial](#newton-polynomial). The final [interpolation polynomial](#interpolation-polynomial) remains unchanged in exact arithmetic. For $f(x)=x^3-2x+1$, reversing $(-1,0,2,3)$ gives $(3,2,0,-1)$ and values $(22,5,1,2)$. The successive [divided difference](#divided-difference) columns are now

$$
\begin{aligned}
D_{i,1}&:\quad 17,\ 2,\ -1,\\
D_{i,2}&:\quad 5,\ 1,\\
D_{i,3}&:\quad 1.
\end{aligned}
$$

For example, the first second [divided difference](#divided-difference) is $(2-17)/(0-3)=5$. The top row becomes $(22,17,5,1)$, giving

$$
\begin{aligned}
q_0(x)&=22,\\
q_1(x)&=22+17(x-3)=17x-29,\\
q_2(x)&=22+17(x-3)+5(x-3)(x-2)=5x^2-8x+1,\\
q_3(x)&=22+17(x-3)+5(x-3)(x-2)+(x-3)(x-2)x\\
&=x^3-2x+1=p_3(x).
\end{aligned}
$$

The earlier partial [interpolants](#interpolant) differ because they fit different subsets: $p_2$ fits $-1,0,2$, whereas $q_2$ fits $3,2,0$. The highest [divided difference](#divided-difference) is invariant because both complete top rows finish with the same set of four [interpolation nodes](#interpolation-node); this is [symmetry of divided differences](#symmetry-of-divided-differences).

<a id="image-reversing-the-interpolation-nodes-changes-the-newton-construction-but-gives-the-same-final-polynomial"></a>
![](newton-interpolation-node-order.png)

**[Figure 4](#image-reversing-the-interpolation-nodes-changes-the-newton-construction-but-gives-the-same-final-polynomial). Reversing the interpolation nodes changes the Newton construction but gives the same final polynomial**.

This distinction is useful when checking a [divided difference table](#divided-difference-table): permuting all the [interpolation nodes](#interpolation-node) must preserve its final [divided difference](#divided-difference), even though the intermediate entries change. It also explains why data can be appended in their arrival order. In [floating-point arithmetic](floating-point-arithmetic.md), the subtractions and divisions may accumulate different rounding errors in different orders; exact invariance describes the mathematical [polynomial](polynomial.md), rather than guaranteeing bit-for-bit equality of numerical results.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (15)

- [Affine combination](geometry-and-topology.md#affine-combination)
- [Chaikin subdivision](computer-aided-geometric-design.md#chaikin-subdivision)
- [Control point](computer-aided-geometric-design.md#control-point)
- [Control-point influence on a curve](computer-aided-geometric-design.md#control-point-influence-on-a-curve)
- [Exposure-averaged light curve](astrophysics.md#exposure-averaged-light-curve)
- [Image registration](inverse-problem.md#image-registration)
- [Lipschitz continuity](real-analysis.md#lipschitz-continuity)
- [Periodic extension of a finite sequence](discrete-fourier-transform.md#periodic-extension-of-a-finite-sequence)
- [Photopic luminous efficiency function](optics.md#photopic-luminous-efficiency-function)
- [Raster graphics](computer-graphics.md#raster-graphics)
- [Raster sampling and reconstruction](computer-graphics.md#raster-sampling-and-reconstruction)
- [Stirling formula](real-analysis.md#stirling-formula)
- [Subdivision curve](computer-aided-geometric-design.md#subdivision-curve)
- [Thermocouple reference function](thermoelectric-effect.md#thermocouple-reference-function)
- [Vector graphics](computer-graphics.md#vector-graphics)
