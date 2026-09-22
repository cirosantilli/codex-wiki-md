# Uniform approximation

↑ **Parent:** [Analysis](analysis.md)

Uniform approximation minimizes the [supremum norm](functional-analysis.md#supremum-norm) of the difference between a target [function](function.md) and an approximant.

The error is measured uniformly over the domain using the [supremum norm](functional-analysis.md#supremum-norm). A sequence of approximants whose uniform error tends to zero converges by [uniform convergence](real-analysis.md#uniform-convergence); the optimization problem and the convergence notion are distinct.

**Table of contents**

- [Lebesgue constant of interpolation](#lebesgue-constant-of-interpolation)
  - [Fekete interpolation sites for a continuous function space](#fekete-interpolation-sites-for-a-continuous-function-space)
- [Chebyshev system](#chebyshev-system)
  - [Odd dimension of a periodic Chebyshev system](#odd-dimension-of-a-periodic-chebyshev-system)
  - [Exponential Chebyshev system](#exponential-chebyshev-system)
  - [Determinant criterion for a Chebyshev system](#determinant-criterion-for-a-chebyshev-system)
- [Uniform closure of a function algebra](#uniform-closure-of-a-function-algebra)
- [Integer polynomial approximation away from zero and one](#integer-polynomial-approximation-away-from-zero-and-one)
- [Polynomial approximation](#polynomial-approximation)
  - [Strict polynomial error decrease from nonvanishing derivatives](#strict-polynomial-error-decrease-from-nonvanishing-derivatives)
- [Bernstein inequality for algebraic polynomials](#bernstein-inequality-for-algebraic-polynomials)
  - [Markov inequality for polynomial derivatives](#markov-inequality-for-polynomial-derivatives)
    - [Duffin-Schaeffer polynomial derivative inequality](#duffin-schaeffer-polynomial-derivative-inequality)
      - [Uniqueness of Chebyshev derivative-norming nodes](#uniqueness-of-chebyshev-derivative-norming-nodes)
- [Extension of approximation operators from a dense subspace](#extension-of-approximation-operators-from-a-dense-subspace)
- [Kolmogorov-Arnold representation theorem](#kolmogorov-arnold-representation-theorem)
  - [Whole-plane reduction for continuous superposition](#whole-plane-reduction-for-continuous-superposition)
  - [Grid-separated additive coordinates](#grid-separated-additive-coordinates)
- [Polynomial approximation of an exterior pole on a convex compact set](#polynomial-approximation-of-an-exterior-pole-on-a-convex-compact-set)
  - [Moving an exterior pole to obtain pointwise polynomial approximation](#moving-an-exterior-pole-to-obtain-pointwise-polynomial-approximation)
- [Integer-coefficient polynomial approximation](#integer-coefficient-polynomial-approximation)
- [Second modulus of smoothness](#second-modulus-of-smoothness)
  - [Second-difference integral formula](#second-difference-integral-formula)
- [Uniform step approximation on a compact interval](#uniform-step-approximation-on-a-compact-interval)
- [Best uniform approximation](#best-uniform-approximation)
  - [Cosine substitution for polynomial approximation](#cosine-substitution-for-polynomial-approximation)
  - [Polynomial reproduction error bound](#polynomial-reproduction-error-bound)
  - [Uniqueness of best uniform polynomial approximation](#uniqueness-of-best-uniform-polynomial-approximation)
  - [Kolmogorov criterion for uniform approximation](#kolmogorov-criterion-for-uniform-approximation)
- [Equioscillation theorem](#equioscillation-theorem)
  - [Strict decrease of best polynomial approximation under a derivative sign](#strict-decrease-of-best-polynomial-approximation-under-a-derivative-sign)
  - [Trigonometric Chebyshev alternation theorem](#trigonometric-chebyshev-alternation-theorem)
    - [Positive lacunary trigonometric series](#positive-lacunary-trigonometric-series)
      - [Weierstrass function](#weierstrass-function)
        - [Critical Weierstrass modulus](#critical-weierstrass-modulus)
  - [Positive lacunary Chebyshev series](#positive-lacunary-chebyshev-series)
- [Bernstein's lethargy theorem](#bernstein-s-lethargy-theorem)
  - [Explicit Chebyshev construction for Bernstein lethargy](#explicit-chebyshev-construction-for-bernstein-lethargy)
- [Jackson-type estimate](#jackson-type-estimate)
  - [Multivariable Jackson approximation](#multivariable-jackson-approximation)
  - [First Jackson theorem for periodic approximation](#first-jackson-theorem-for-periodic-approximation)
  - [Jackson kernel](#jackson-kernel)
    - [Jackson operator estimate](#jackson-operator-estimate)
- [Inverse theorem for trigonometric approximation](#inverse-theorem-for-trigonometric-approximation)
  - [Logarithmic cusp with slow trigonometric approximation](#logarithmic-cusp-with-slow-trigonometric-approximation)
  - [Endpoint obstruction to an algebraic inverse approximation theorem](#endpoint-obstruction-to-an-algebraic-inverse-approximation-theorem)
- [Korovkin theorem](#korovkin-theorem)
  - [Quadratic barrier estimate for positive approximation operators](#quadratic-barrier-estimate-for-positive-approximation-operators)
  - [Compact Korovkin test space](#compact-korovkin-test-space)
    - [Periodic Korovkin test set](#periodic-korovkin-test-set)
- [Spline (mathematics)](#spline-mathematics)
  - [Linear spline](#linear-spline)
  - [Spline approximation](#spline-approximation)
    - [Spline quasi-interpolation](#spline-quasi-interpolation)
    - [Box spline](#box-spline)
      - [Unit-direction univariate box spline](#unit-direction-univariate-box-spline)
      - [Quadratic four-direction box spline](#quadratic-four-direction-box-spline)
      - [Twice-smoothed four-direction box spline](#twice-smoothed-four-direction-box-spline)
    - [Quadratic spline](#quadratic-spline)
    - [Spline interpolation](#spline-interpolation)
      - [Spline interpolation operator](#spline-interpolation-operator)
        - [Centered quadratic spline interpolation](#centered-quadratic-spline-interpolation)
        - [B-spline interpolation operator norm](#b-spline-interpolation-operator-norm)
          - [Linear growth of shifted quadratic spline interpolation](#linear-growth-of-shifted-quadratic-spline-interpolation)
    - [Maximum-norm bound for spline projection](#maximum-norm-bound-for-spline-projection)
    - [Regression spline](#regression-spline)
      - [Cubic regression spline](#cubic-regression-spline)
      - [Penalized regression spline](#penalized-regression-spline)
    - [Second derivative roughness penalty](#second-derivative-roughness-penalty)
    - [Spline knot](#spline-knot)
      - [Spline knot sequence](#spline-knot-sequence)
    - [Cubic spline](#cubic-spline)
      - [Natural cubic spline](#natural-cubic-spline)
        - [Natural cubic spline interpolant](#natural-cubic-spline-interpolant)
          - [Spline roughness penalty matrix](#spline-roughness-penalty-matrix)
          - [Minimum roughness property of the natural cubic spline interpolant](#minimum-roughness-property-of-the-natural-cubic-spline-interpolant)
            - [Minimum roughness property with absolutely continuous first derivatives](#minimum-roughness-property-with-absolutely-continuous-first-derivatives)
    - [B-spline](#b-spline)
      - [B-spline differentiation formula](#b-spline-differentiation-formula)
      - [Local linear independence of B-splines](#local-linear-independence-of-b-splines)
      - [Compact-support spline zero count](#compact-support-spline-zero-count)
      - [Quartic treble-knot representation of a quadratic B-spline](#quartic-treble-knot-representation-of-a-quadratic-b-spline)
      - [Non-uniform rational B-spline](#non-uniform-rational-b-spline)
      - [Knot insertion](#knot-insertion)
      - [De Boor's algorithm](#de-boor-s-algorithm)
      - [Unit-integral normalization of a B-spline](#unit-integral-normalization-of-a-b-spline)
      - [Uniform-norm stability of a B-spline basis](#uniform-norm-stability-of-a-b-spline-basis)
        - [Coefficient condition number of a normalized B-spline basis](#coefficient-condition-number-of-a-normalized-b-spline-basis)
        - [Chebyshev spline coefficient and dual norm equality](#chebyshev-spline-coefficient-and-dual-norm-equality)
          - [Optimal spline coefficient interpolation sites](#optimal-spline-coefficient-interpolation-sites)
      - [Subpartition of unity for B-splines](#subpartition-of-unity-for-b-splines)
      - [Simple-knot B-spline regularity](#simple-knot-b-spline-regularity)
      - [Support and Gram bandwidth of B-splines](#support-and-gram-bandwidth-of-b-splines)
      - [Mixed-normalization spline Gram matrix](#mixed-normalization-spline-gram-matrix)
        - [Uniform norm bound for B-spline orthogonal projection](#uniform-norm-bound-for-b-spline-orthogonal-projection)
        - [Linear-spline mixed Gram matrix](#linear-spline-mixed-gram-matrix)
      - [Lee interpolation identity](#lee-interpolation-identity)
      - [Cardinal B-spline](#cardinal-b-spline)
        - [Quintic cardinal spline midpoint collocation](#quintic-cardinal-spline-midpoint-collocation)
        - [Quadratic cardinal B-spline](#quadratic-cardinal-b-spline)
          - [Midpoint quadratic spline collocation](#midpoint-quadratic-spline-collocation)
        - [Cardinal cubic B-spline](#cardinal-cubic-b-spline)
          - [Cubic B-spline Bézier extraction](#cubic-b-spline-bezier-extraction)
          - [Midpoint cubic spline collocation](#midpoint-cubic-spline-collocation)
            - [Exact inverse norm of midpoint cubic spline collocation](#exact-inverse-norm-of-midpoint-cubic-spline-collocation)
      - [Cox-de Boor recursion formula](#cox-de-boor-recursion-formula)
      - [Marsden identity](#marsden-identity)
        - [Monomial B-spline coefficients](#monomial-b-spline-coefficients)
          - [Greville abscissa](#greville-abscissa)
            - [Linear precision at Greville abscissae](#linear-precision-at-greville-abscissae)
        - [Marsden dual functional](#marsden-dual-functional)
          - [De Boor–Fix spline coefficient functional](#de-boor-fix-spline-coefficient-functional)
          - [Normalized Marsden dual functional](#normalized-marsden-dual-functional)
      - [B-spline collocation matrix](#b-spline-collocation-matrix)
        - [Total nonnegativity of B-spline collocation matrices](#total-nonnegativity-of-b-spline-collocation-matrices)
        - [Schoenberg–Whitney theorem](#schoenberg-whitney-theorem)
      - [Schoenberg spline operator](#schoenberg-spline-operator)
        - [Local-support error bound for a Schoenberg spline operator](#local-support-error-bound-for-a-schoenberg-spline-operator)

## Lebesgue constant of interpolation

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

If interpolation at distinct sites $x_i$ in a finite-dimensional space of [continuous functions](calculus.md#continuous-function) is unique, its cardinal functions satisfy $\ell_i(x_j)=\delta_{ij}$. The interpolation [linear map](vector-space.md#linear-map) is $Pf=\sum_if(x_i)\ell_i$ and has [operator norm](continuous-dual-space.md#operator-norm) $\Lambda_{\mathbf x}$ in the [supremum norm](functional-analysis.md#supremum-norm). The upper bound is the [triangle inequality](topological-analysis.md#triangle-inequality). For the reverse bound choose node values to be the signs of the cardinal functions at a point maximizing their absolute sum, and extend those values by a [continuous function](calculus.md#continuous-function) of [norm](functional-analysis.md#norm) one. The [polynomial reproduction error bound](#polynomial-reproduction-error-bound) gives $\|f-Pf\|_\infty\le(1+\Lambda_{\mathbf x})\inf_{s\in\operatorname{range}P}\|f-s\|_\infty$.

### Fekete interpolation sites for a continuous function space

↑ **Parent:** [Lebesgue constant of interpolation](#lebesgue-constant-of-interpolation)

For a real $n$-dimensional [vector space](vector-space.md) of [continuous functions](calculus.md#continuous-function) on a [compact](topology.md#compact-space) [interval](real-analysis.md#interval-mathematics), choose sites maximizing the absolute evaluation [determinant](linear-algebra.md#determinant) in any [basis](vector-space.md#basis). [Linear independence](vector-space.md#linear-independence) ensures some nonzero evaluation [determinant](linear-algebra.md#determinant), so a maximizer exists and has distinct sites. Replacing row $i$ by evaluation at $t$ multiplies the [determinant](linear-algebra.md#determinant) by the cardinal function $\ell_i(t)$. Maximality implies $|\ell_i(t)|\le1$, hence the [Lebesgue constant of interpolation](#lebesgue-constant-of-interpolation) is at most $n$. This gives a useful interpolation set without asserting that determinant maximization minimizes the [Lebesgue constant of interpolation](#lebesgue-constant-of-interpolation).

## Chebyshev system

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

A Chebyshev system on a nondegenerate real interval is a family of $n+1$ real [continuous functions](calculus.md#continuous-function) such that every [linear combination](vector-space.md#linear-combination) with coefficients not all zero has at most $n$ distinct zeros. The condition entails [linear independence](vector-space.md#linear-independence) and unique interpolation at any $n+1$ distinct points. It is a zero-counting hypothesis, not a requirement to count multiplicities.

### Odd dimension of a periodic Chebyshev system

↑ **Parent:** [Chebyshev system](#chebyshev-system)

A [Chebyshev system](#chebyshev-system) of real [continuous functions](calculus.md#continuous-function) on a circle has odd dimension. If its dimension is $d$, take $d$ cyclically ordered evaluation points and move them continuously to the next cyclic permutation without letting points collide. The evaluation [determinant](linear-algebra.md#determinant) stays nonzero, so cannot change sign. The final cyclic row permutation multiplies it by $(-1)^{d-1}$; consequently $d$ must be odd. For example, $1,\cos x,\sin x,\ldots,\cos mx,\sin mx$ has dimension $2m+1$ and the required zero bound.

### Exponential Chebyshev system

↑ **Parent:** [Chebyshev system](#chebyshev-system)

Exponentials with distinct real exponents form a [Chebyshev system](#chebyshev-system) on every nondegenerate real interval. For an inductive proof, multiply a candidate combination by $e^{-\lambda_0x}$. If it has $n+1$ zeros, [Rolle's theorem](calculus.md#rolle-theorem) gives at least $n$ zeros of its derivative, a combination of the $n$ exponentials with exponents $\lambda_i-\lambda_0$, $i>0$. The inductive zero bound forces all those coefficients to vanish. The remaining constant also vanishes, a contradiction.

### Determinant criterion for a Chebyshev system

↑ **Parent:** [Chebyshev system](#chebyshev-system)

A family of $n+1$ real [continuous functions](calculus.md#continuous-function) is a [Chebyshev system](#chebyshev-system) exactly when every evaluation [matrix](vector-space.md#matrix) at $n+1$ distinct points is invertible. A singular evaluation matrix supplies a nonzero coefficient vector whose function vanishes at those points; conversely, a violation of the zero bound supplies such a vector in the [kernel](linear-algebra.md#kernel-of-a-linear-map). This also gives the existence and uniqueness of interpolation from its span.

## Uniform closure of a function algebra

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

For an algebra $A\subseteq C(K)$ on a compact space, its uniform closure consists of functions that are [uniform limits](real-analysis.md#uniform-limit) of sequences from $A$. It is a closed algebra in the [uniform norm](functional-analysis.md#supremum-norm), because addition and multiplication preserve uniform convergence for bounded functions. If it contains every constant and separates points, the [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) makes the closure all of $C(K)$.

## Integer polynomial approximation away from zero and one

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

On $[a,b]\subset(0,1)$, the [uniform closure](#uniform-closure-of-a-function-algebra) of integer-coefficient [polynomials](polynomial.md) contains $1/2$, since $\sum_{j=0}^Nx(1-2x)^j\to1/2$ uniformly. This closure is a ring, so it contains all dyadic constants and then all real constants. It contains $x$ and therefore every real-coefficient polynomial. The [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) makes it all of $C([a,b])$. On an interval including zero this fails, since the value of an integer-coefficient polynomial at zero is an integer.

## Polynomial approximation

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

Polynomial approximation represents a function by [polynomials](polynomial.md) of bounded [polynomial degree](polynomial.md#degree-of-a-polynomial). On a compact real interval, the [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) guarantees [uniform approximation](uniform-approximation.md) of every [continuous function](calculus.md#continuous-function) by such polynomials. The displayed best error quantifies the accuracy available at degree at most $n$.

### Strict polynomial error decrease from nonvanishing derivatives

↑ **Parent:** [Polynomial approximation](#polynomial-approximation)

If $n\ge1$, $f$ is real and $C^n$ on an interval, and $f^{(n)}$ is nowhere zero there, the displayed inequality holds. If the errors were equal, a best degree-at-most-$n-1$ polynomial would also be best at degree $n$. The [Chebyshev alternation theorem](#equioscillation-theorem) and [intermediate value theorem](calculus.md#intermediate-value-theorem) would give $n+1$ zeros of the error. Applying [Rolle's theorem](calculus.md#rolle-theorem) $n$ times would force a zero of $f^{(n)}$, a contradiction. The zero-error case already contradicts $f^{(n)}\ne0$. In particular this proves strict improvement for the [exponential function](calculus.md#exponential-function) at every positive degree step.

## Bernstein inequality for algebraic polynomials

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

For a polynomial of degree at most $n$, this [derivative](calculus.md#derivative) estimate holds for $-1<x<1$. It controls the derivative away from the endpoints. Sampling it at [Chebyshev polynomial](numerical-analysis.md#chebyshev-polynomial) roots supplies the hypotheses of the [Chebyshev nodal derivative comparison](numerical-analysis.md#chebyshev-nodal-derivative-comparison), which controls the missing endpoint regions. The norm is taken on the entire interval, although the displayed pointwise bound concerns its interior.

### Markov inequality for polynomial derivatives

↑ **Parent:** [Bernstein inequality for algebraic polynomials](#bernstein-inequality-for-algebraic-polynomials)

Apply the [Bernstein inequality for algebraic polynomials](#bernstein-inequality-for-algebraic-polynomials) to the central interval $|x|\le\cos(\pi/(2n))$, using $\sin(\pi/(2n))\ge1/n$. On the remaining regions apply the [Chebyshev nodal derivative comparison](numerical-analysis.md#chebyshev-nodal-derivative-comparison) to $p'$. Since $T_n'(\cos\theta)=n\sin(n\theta)/\sin\theta$, the identity expressing $\sin(n\theta)/\sin\theta$ as a sum of $n$ unit complex phases gives $|T_n'|\le n^2$. The endpoint limit is $T_n'(1)=n^2$, so the constant is sharp.

#### Duffin-Schaeffer polynomial derivative inequality

↑ **Parent:** [Markov inequality for polynomial derivatives](#markov-inequality-for-polynomial-derivatives)

If a real degree-at-most-$n$ [polynomial](polynomial.md) has absolute value at most one at every extremum $\cos(j\pi/n)$ of the [Chebyshev polynomial](numerical-analysis.md#chebyshev-polynomial) $T_n$, its $k$th [derivative](calculus.md#derivative) on $[-1,1]$ is bounded by $T_n^{(k)}(1)$, for $1\le k\le n$. This strengthens the [Markov inequality for polynomial derivatives](#markov-inequality-for-polynomial-derivatives) by replacing a bound on the whole interval with these finitely many samples. The node set is rigid, as quantified by [uniqueness of Chebyshev derivative-norming nodes](#uniqueness-of-chebyshev-derivative-norming-nodes).

##### Uniqueness of Chebyshev derivative-norming nodes

↑ **Parent:** [Duffin-Schaeffer polynomial derivative inequality](#duffin-schaeffer-polynomial-derivative-inequality)

For $n\ge1$, any distinct node set in $[-1,1]$ different from the $n+1$ [Chebyshev polynomial](numerical-analysis.md#chebyshev-polynomial) extrema admits one degree-$n$ [polynomial](polynomial.md) $q$, bounded by one at all those nodes, whose every nonconstant derivative violates the corresponding sharp endpoint bound. In decreasing order set $q(t_i)=(-1)^i$. The [endpoint derivative signs of Lagrange cardinal polynomials](numerical-analysis.md#endpoint-derivative-signs-of-lagrange-cardinal-polynomials) give $q^{(k)}(1)=\sum_i|L_i^{(k)}(1)|$. Interpolating $T_n$ on the same nodes shows

$$
q^{(k)}(1)-T_n^{(k)}(1)=\sum_i|L_i^{(k)}(1)|\bigl[1-(-1)^iT_n(t_i)\bigr]>0.
$$

Each term is nonnegative and at least one is positive, because the other node set includes a nonextremal point. Uniqueness is a claim about node sets: permuting the same nodes does not change their norming property.

## Extension of approximation operators from a dense subspace

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

Suppose [linear operators](vector-space.md#linear-operator) $T_n$ on a [normed vector space](functional-analysis.md#normed-vector-space) satisfy $\|T_n\|\le C$ uniformly and $T_np\to p$ on a [dense subspace](topological-vector-space.md#dense-subspace). The displayed [triangle inequality](topological-analysis.md#triangle-inequality) for any element $p$ of that subspace first permits $p$ to approximate $f$, then lets $n$ increase, proving $T_nf\to f$ for every $f$. Applied to the [Bernstein polynomial](functional-analysis.md#bernstein-polynomial), the [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) supplies the dense polynomial subspace and $C=1$.

## Kolmogorov-Arnold representation theorem

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

Every real [continuous function](calculus.md#continuous-function) on a compact square can be represented as $\sum_{q=1}^5G_q(a_q(x)+b_q(y))$, with continuous one-variable functions and fixed inner functions $a_q,b_q$ independent of the represented function. [Grid-separated additive coordinates](#grid-separated-additive-coordinates) give the inner functions. For a residual $r$ of norm $M$, assign $r$ at a sample point divided by three to each separated rectangle image, and continuously interpolate between images. Each point lies in at least three rectangles, so if $k\in\{3,4,5\}$ summands are accurate, the error is at most $[|1-k/3|+(5-k)/3]M+5\eta/3=2M/3+5\eta/3$. Choose oscillation $\eta\le M/10$ to obtain contraction $5/6$. Iteration gives outer functions by [uniform convergence](real-analysis.md#uniform-convergence) of corrections bounded by $M(5/6)^j/3$. [Whole-plane reduction for continuous superposition](#whole-plane-reduction-for-continuous-superposition) removes compactness of the original domain without assuming boundedness of the original function.

### Whole-plane reduction for continuous superposition

↑ **Parent:** [Kolmogorov-Arnold representation theorem](#kolmogorov-arnold-representation-theorem)

For $f\in C(\mathbb R^2)$, choose a positive [continuous function](calculus.md#continuous-function) $A$ with $A(t)\ge(1+t)\max_{x^2+y^2\le t}|f(x,y)|$ for $t\ge0$. Such an $A$ is obtained by piecewise linear interpolation of a sufficiently large increasing sequence. Then $b(x,y)=f(x,y)/A(x^2+y^2)$ tends uniformly to zero at infinity. Transport $b$ to $(0,1)^2$ by $x=\tan(\pi(s-1/2))$ and extend it by zero on the boundary; the extension is continuous. Apply the compact [Kolmogorov-Arnold representation theorem](#kolmogorov-arnold-representation-theorem), then multiply by $A(x^2+y^2)$. Multiplication introduces no additional primitive operation because $uv=[(u+v)^2-(u-v)^2]/4$ uses only addition and continuous one-variable squaring and scaling.

### Grid-separated additive coordinates

↑ **Parent:** [Kolmogorov-Arnold representation theorem](#kolmogorov-arnold-representation-theorem)

For five pairs of [continuous functions](calculus.md#continuous-function) on $[0,1]$, one can arrange that at every arbitrarily fine scale there are closed interval families whose product rectangles cover each point at least three times, and within each family the images under $a_q(x)+b_q(y)$ are mutually disjoint. To see this, put gaps near five shifted fine grids; gap sets for different shifts are disjoint. Each coordinate misses at most one family, so a pair misses at most two. Approximate any prescribed pair of functions by constants on the complementary intervals, interpolating across gaps. Perturb the finitely many constants to avoid all equalities between distinct pair sums. The rectangle images are then separated by a positive distance, a property preserved under sufficiently small uniform perturbations. For each required mesh size this property defines a dense open subset of $C([0,1])^{10}$. The [Baire category theorem](topological-analysis.md#baire-category-theorem) gives a tuple satisfying every scale simultaneously.

## Polynomial approximation of an exterior pole on a convex compact set

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

For a compact [convex set](mathematical-optimization.md#convex-set) $K\subset\mathbb C$ and $\zeta\notin K$, strict separation gives a unit vector $u$ with $\operatorname{Re}(\bar u\zeta)>\max_K\operatorname{Re}(\bar uz)$. Taking $c=-Ru$ for large $R$ makes $q=\max_K|z-c|/|\zeta-c|<1$. The polynomial

$$
p_N(z)=-\frac1{\zeta-c}\sum_{j=0}^N\left(\frac{z-c}{\zeta-c}\right)^j
$$

has uniform error at most $q^{N+1}/(|\zeta-c|(1-q))$. This elementary [geometric series](real-analysis.md#geometric-series) argument proves exterior-pole approximation without a general complex approximation theorem.

### Moving an exterior pole to obtain pointwise polynomial approximation

↑ **Parent:** [Polynomial approximation of an exterior pole on a convex compact set](#polynomial-approximation-of-an-exterior-pole-on-a-convex-compact-set)

Let $z_0$ be a boundary point of a compact convex set and choose exterior points $\zeta_n\to z_0$. Approximate $(z-\zeta_n)^{-1}$ uniformly on the compact set by a polynomial with error at most $1/n$. At each fixed $z\ne z_0$, the reciprocal converges and so does the approximating polynomial. On a boundary accumulating at $z_0$, uniform convergence to the singular reciprocal is impossible because each polynomial is bounded there. This distinguishes [pointwise convergence](real-analysis.md#pointwise-convergence) from [uniform convergence](real-analysis.md#uniform-convergence) without confusing the two norms.

## Integer-coefficient polynomial approximation

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

The [uniform approximation](uniform-approximation.md) closure of the integer-coefficient [polynomials](polynomial.md) on $[0,1]$ consists precisely of the [continuous functions](calculus.md#continuous-function) taking [integer](number-theory.md#integer) values at both endpoints. Necessity follows because evaluations at zero and one are [integers](number-theory.md#integer) and convergent [integer](number-theory.md#integer) sequences are eventually constant. For sufficiency, the [rounded Bernstein polynomial](functional-analysis.md#rounded-bernstein-polynomial) has [integer](number-theory.md#integer) monomial [coefficients](vector-space.md#coefficient) and differs uniformly by a vanishing amount from the [Bernstein polynomial](functional-analysis.md#bernstein-polynomial), which converges uniformly to the target.

## Second modulus of smoothness

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

For a continuous periodic function set

$$
\omega_2(f,h)=\sup_{|u|\leq h}\|f(\cdot+u)-2f+f(\cdot-u)\|_\infty.
$$

It measures smoothness through second differences without requiring a derivative. For $h>0$, factoring the translation difference gives $\omega_2(f,t)\leq(1+t/h)^2\omega_2(f,h)$. The [second-difference integral formula](#second-difference-integral-formula) gives $\omega_2(f,h)\leq h^2\|f''\|_\infty$ for twice continuously differentiable functions.

### Second-difference integral formula

↑ **Parent:** [Second modulus of smoothness](#second-modulus-of-smoothness)

For a twice continuously differentiable function and $h\geq0$, the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) gives

$$
f(x+h)-2f(x)+f(x-h)=\int_{-h}^h(h-|u|)f''(x+u)\,du.
$$

The nonnegative triangular weight has integral $h^2$, so its [supremum norm](functional-analysis.md#supremum-norm) estimate directly controls the [second modulus of smoothness](#second-modulus-of-smoothness).

## Uniform step approximation on a compact interval

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

A [uniformly continuous](topological-analysis.md#uniform-continuity) real [function](function.md) on a closed bounded interval can be approximated uniformly by finite [step functions](measure-theory.md#step-function). Given $\varepsilon>0$, choose a mesh smaller than the uniform-continuity distance and set the approximant equal to a sampled value on each interval. Then the [supremum norm](functional-analysis.md#supremum-norm) of the approximation error is at most $\varepsilon$. If the function has a [Lipschitz bound](real-analysis.md#lipschitz-bound) $L$, a mesh of maximum length $h$ gives the explicit error bound $\|f-g\|_\infty\le Lh$.

## Best uniform approximation

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

Given a family $A$ of approximating [functions](function.md), a best uniform approximation to $f$ is an element $p\in A$ satisfying

$$
\lVert f-p\rVert_\infty=\inf_{q\in A}\lVert f-q\rVert_\infty.
$$

### Cosine substitution for polynomial approximation

↑ **Parent:** [Best uniform approximation](#best-uniform-approximation)

Cosine substitution is an isometry from continuous functions on $[-1,1]$ to even continuous $2\pi$-periodic functions. It satisfies $\omega(\widetilde f,\delta)\le\omega(f,\delta)$ because cosine is [Lipschitz continuous](real-analysis.md#lipschitz-continuity) with constant one. Even degree-at-most-$n$ [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) correspond exactly to algebraic polynomials via $T_j(\cos\theta)=\cos(j\theta)$. Averaging a periodic approximant with its reflection cannot increase its error against an even target, so the algebraic and periodic best errors are equal.

### Polynomial reproduction error bound

↑ **Parent:** [Best uniform approximation](#best-uniform-approximation)

If a bounded [linear map](vector-space.md#linear-map) $P$ reproduces every element of an approximating polynomial space $V$, then $f-Pf=(f-v)-P(f-v)$ for every $v\in V$. The triangle inequality and infimum over $v$ prove the displayed error bound. The same argument works for any linear approximating space, and applies in particular to [de la Vallée Poussin sums](fourier-series.md#de-la-vallee-poussin-sum).

### Uniqueness of best uniform polynomial approximation

↑ **Parent:** [Best uniform approximation](#best-uniform-approximation)

For a fixed degree bound, two best approximating [polynomials](polynomial.md) have a best approximating average. At each active point of that average their errors agree, hence the two polynomials agree. There must be at least two more active points than the degree: otherwise [polynomial interpolation](numerical-analysis.md#polynomial-interpolation) constructs a strictly improving sign-matching perturbation. The difference has too many zeros and must vanish. Finite-dimensional coefficient compactness also gives existence.

### Kolmogorov criterion for uniform approximation

↑ **Parent:** [Best uniform approximation](#best-uniform-approximation)

For real $f$, a candidate $u\in U\subset C(K,\mathbb R)$, and active set $E=\{x:|f(x)-u(x)|=\|f-u\|_\infty\}$, the candidate is best precisely when every $v\in U$ has some $x\in E$ with $(f(x)-u(x))v(x)\leq0$. A direction with strictly matching error signs on the whole active set gives a uniformly improving small perturbation by compactness. Conversely one oppositely signed active value already prevents improvement. This criterion yields the [Chebyshev alternation theorem](#equioscillation-theorem).

## Equioscillation theorem

↑ **Parent:** [Uniform approximation](uniform-approximation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equioscillation_theorem)

A degree-at-most-$m$ polynomial is a best uniform approximation precisely when its error attains alternating extrema of equal magnitude at at least $m+2$ ordered points.

### Strict decrease of best polynomial approximation under a derivative sign

↑ **Parent:** [Equioscillation theorem](#equioscillation-theorem)

For real $f\in C^{n+1}[0,1]$ with positive $(n+1)$st [derivative](calculus.md#derivative), equality of consecutive [best uniform approximation](#best-uniform-approximation) errors would make a best degree-at-most-$n$ [polynomial](polynomial.md) also best at degree $n+1$. The [Chebyshev alternation theorem](#equioscillation-theorem) then supplies $n+3$ alternating extrema of its nonzero error, hence $n+2$ distinct zeros. Repeated [Rolle's theorem](calculus.md#rolle-theorem) forces a zero of the $(n+1)$st derivative of that error, contradicting the assumed sign. The same conclusion holds for a strictly negative derivative by replacing $f$ with $-f$.

### Trigonometric Chebyshev alternation theorem

↑ **Parent:** [Equioscillation theorem](#equioscillation-theorem)

For real [continuous](calculus.md#continuous-function) $2\pi$-periodic $f$, a degree-at-most-$n$ real [trigonometric polynomial](fourier-series.md#trigonometric-polynomial) $p$ is its unique [best uniform approximation](#best-uniform-approximation) exactly when $f-p$ has $2n+2$ alternating extrema of magnitude $\|f-p\|_\infty$ at distinct ordered points in one period. The closing interval around the circle also counts. A strictly improving approximant would force its difference from $p$ to have at least $2n+2$ zeros, whereas a nonzero degree-$n$ [trigonometric polynomial](fourier-series.md#trigonometric-polynomial) has at most $2n$.

#### Positive lacunary trigonometric series

↑ **Parent:** [Trigonometric Chebyshev alternation theorem](#trigonometric-chebyshev-alternation-theorem)

For an odd [integer](number-theory.md#integer) $q\ge3$ and positive summable [coefficients](vector-space.md#coefficient) $a_k$, the [Weierstrass M-test](probability-and-statistics.md#weierstrass-m-test) makes $f(x)=\sum_{k\ge0}a_k\cos(q^kx)$ [continuous](calculus.md#continuous-function). Its partial sum over $q^k\le n$ is the unique [best uniform approximation](#best-uniform-approximation) by degree-at-most-$n$ [trigonometric polynomials](fourier-series.md#trigonometric-polynomial), for $n\ge1$. If $Q$ is the first omitted frequency, at $x_j=j\pi/Q$ every omitted cosine equals $(-1)^j$ because all frequency ratios are odd. Thus the tail attains alternating extrema equal to its coefficient sum at $2Q\ge2n+2$ points. The [trigonometric Chebyshev alternation theorem](#trigonometric-chebyshev-alternation-theorem) proves the formula. For $a_k=r^{-k}$, $r>1$, the largest decay exponent is $\log r/\log q$.

##### Weierstrass function

↑ **Parent:** [Positive lacunary trigonometric series](#positive-lacunary-trigonometric-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weierstrass_function)

A standard [Weierstrass function](#weierstrass-function) is a uniformly convergent lacunary cosine series, here parameterized by $a>1$ and an integer frequency multiplier $b>1$. Its continuity follows from the [Weierstrass M-test](probability-and-statistics.md#weierstrass-m-test). In the range $1<a<b$, its [modulus of continuity](topological-analysis.md#modulus-of-continuity) has the fractional-power scale $\delta^{\log a/\log b}$ for the positive odd-frequency model; the critical case $a=b$ can have the larger scale $\delta\log(1/\delta)$. These examples distinguish small approximation error from ordinary [Lipschitz continuity](real-analysis.md#lipschitz-continuity).

###### Critical Weierstrass modulus

↑ **Parent:** [Weierstrass function](#weierstrass-function)

For $g(x)=\sum_{k\ge0}5^{-k}\cos(5^kx)$, all frequencies satisfy $5^k\equiv1\pmod4$. At $x=\pi/2$, the increment is $-\sum_{k\ge0}5^{-k}\sin(5^kh)$. If $5^m\le1/h<5^{m+1}$, the first $m+1$ terms have $0<5^kh\le1$ and contribute at least $(m+1)h\sin1$, while the remaining tail has magnitude at most $5^{-m}/4\le5h/4$. This proves a lower [modulus of continuity](topological-analysis.md#modulus-of-continuity) bound of order $h\log(1/h)$ for small $h$. The [inverse theorem for trigonometric approximation](#inverse-theorem-for-trigonometric-approximation) supplies the matching upper bound because the [positive lacunary trigonometric series](#positive-lacunary-trigonometric-series) has $E_n(g)\asymp n^{-1}$.

### Positive lacunary Chebyshev series

↑ **Parent:** [Equioscillation theorem](#equioscillation-theorem)

For positive summable coefficients, the [Weierstrass M-test](probability-and-statistics.md#weierstrass-m-test) gives a continuous uniform sum. The partial sum over $3^k\le n$ is the unique [best uniform approximation](#best-uniform-approximation) of degree at most $n$. If $3^K$ is the first omitted frequency, every tail term equals $(-1)^j$ at $x_j=\cos(j\pi/3^K)$ because its frequency ratio is odd. The entire tail therefore attains alternating extrema equal in magnitude to its coefficient sum at more than $n+1$ points. The [Chebyshev alternation theorem](#equioscillation-theorem) proves the assertion, including the empty partial sum at $n=0$.

<h2 id="bernstein-s-lethargy-theorem">Bernstein's lethargy theorem</h2>

↑ **Parent:** [Uniform approximation](uniform-approximation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernstein's_lethargy_theorem)

Bernstein's lethargy theorem says that best approximation errors in nested approximation spaces can tend to zero arbitrarily slowly. For algebraic polynomials on $[-1,1]$, given any decreasing positive sequence $\delta_n\to0$, there is a continuous function $f$ whose best degree-$n$ uniform-approximation error is at least $\delta_n$ for every $n$.

### Explicit Chebyshev construction for Bernstein lethargy

↑ **Parent:** [Bernstein's lethargy theorem](#bernstein-s-lethargy-theorem)

For a strictly decreasing positive sequence $\epsilon_n\to0$, put $a_0=\epsilon_0-\epsilon_1$ and $a_k=\epsilon_{3^{k-1}}-\epsilon_{3^k}$ for $k\ge1$. These are positive with sum $\epsilon_0$. The [positive lacunary Chebyshev series](#positive-lacunary-chebyshev-series) $f_\epsilon=\sum_k a_kT_{3^k}$ has error $\epsilon_0$ at degree zero and error $\epsilon_{3^{K-1}}\ge\epsilon_n$ whenever $3^{K-1}\le n<3^K$. This proves the lower-bound form of [Bernstein's lethargy theorem](#bernstein-s-lethargy-theorem) with an explicit continuous function.

## Jackson-type estimate

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

A Jackson-type estimate bounds an approximation error by a smoothness quantity such as a [modulus of continuity](topological-analysis.md#modulus-of-continuity), with the smoothness evaluated at a scale comparable to the reciprocal of the approximating degree.

### Multivariable Jackson approximation

↑ **Parent:** [Jackson-type estimate](#jackson-type-estimate)

For $p\ge1$ and $f\in C^p(\mathbb T^n)$, there is a real [trigonometric polynomial](fourier-series.md#trigonometric-polynomial) with coordinate frequencies $|k_j|\le N$ whose uniform error is at most $C_{n,p}N^{-p}\|f\|_{C^p}$. One obtains the multivariable statement by applying bounded one-dimensional Jackson approximation operators successively in each coordinate and telescoping their errors. Each operator commutes with differentiation in the other coordinates, and its uniform operator norm is bounded independently of $N$; the total error is bounded by a constant times $N^{-p}\sum_j\|\partial_j^p f\|_\infty$.

### First Jackson theorem for periodic approximation

↑ **Parent:** [Jackson-type estimate](#jackson-type-estimate)

Every continuous $2\pi$-periodic function admits degree-at-most-$n$ [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) with [supremum norm](functional-analysis.md#supremum-norm) error bounded by a universal constant times its [modulus of continuity](topological-analysis.md#modulus-of-continuity) at scale $1/n$, for $n\ge1$. This first-order [Jackson-type estimate](#jackson-type-estimate) transfers to algebraic polynomials through [cosine substitution for polynomial approximation](#cosine-substitution-for-polynomial-approximation).

### Jackson kernel

↑ **Parent:** [Jackson-type estimate](#jackson-type-estimate)

The normalized even kernel

$$
J_n(t)=\frac{3}{2\pi n(2n^2+1)}\left(\frac{\sin(nt/2)}{\sin(t/2)}\right)^4
$$

is nonnegative, has integral one, and is a [trigonometric polynomial](fourier-series.md#trigonometric-polynomial) of degree $2(n-1)$. Its mass is concentrated on a scale $1/n$: $J_n(t)\leq C\min(n,n^{-3}|t|^{-4})$ for $|t|\leq\pi$. This controls a weighted second moment and produces the [Jackson operator estimate](#jackson-operator-estimate).

#### Jackson operator estimate

↑ **Parent:** [Jackson kernel](#jackson-kernel)

For $j_nf(x)=\int_{-\pi}^{\pi}f(x-t)J_n(t)\,dt$, evenness and unit mass reduce the error to an integral of second differences. The [Jackson kernel](#jackson-kernel) bound and the scaling inequality for the [second modulus of smoothness](#second-modulus-of-smoothness) yield $\|j_nf-f\|_\infty\leq C\omega_2(f,1/n)$. Since the degree is $2(n-1)$, a degree-$N$ estimate uses $n=\lfloor N/2\rfloor+1$. For $f\in C^2$ this gives $E_N(f)\leq C'N^{-2}\|f''\|_\infty$.

## Inverse theorem for trigonometric approximation

↑ **Parent:** [Uniform approximation](uniform-approximation.md)

For periodic uniform approximation,

$$
\omega(f,n^{-1})\leq\frac Cn\sum_{\nu=0}^nE_\nu(f).
$$

### Logarithmic cusp with slow trigonometric approximation

↑ **Parent:** [Inverse theorem for trigonometric approximation](#inverse-theorem-for-trigonometric-approximation)

Define $h(x)=|x|\log(e\pi/|x|)$ on $[-\pi,\pi]$, set $h(0)=0$, and extend periodically. Concavity and monotonicity on $[0,\pi]$ give $\omega(h,\delta)=\delta\log(e\pi/\delta)$ for $0<\delta\le\pi$. Its cosine [Fourier coefficients](fourier-series.md#fourier-coefficient) are

$$
a_j=-\frac{2}{\pi j^2}\int_0^{j\pi}\frac{1-\cos u}{u}\,du
=-\frac{2\log j}{\pi j^2}+O(j^{-2}),\qquad j\ge1.
$$

One [integration by parts](calculus.md#integration-by-parts) gives the formula; the remaining integral is $\log j+O(1)$ by the [Dirichlet test](real-analysis.md#dirichlet-test). All these coefficients are nonpositive. The [de la Vallée Poussin sum](fourier-series.md#de-la-vallee-poussin-sum) $V_n=2\sigma_{2n}-\sigma_n$ reproduces degree-at-most-$n$ [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) and has [operator norm](continuous-dual-space.md#operator-norm) at most three. Hence $L_n(f)=f(0)-V_nf(0)$ has norm at most four and annihilates those polynomials. Its weights on coefficients are zero up to $n$, nonnegative thereafter, and one from $2n$ onwards, so $|L_n(h)|\ge\sum_{j\ge2n}|a_j|\gtrsim\log n/n$. Thus $E_n(h)\ge|L_n(h)|/4\gtrsim\log n/n$; the [first Jackson theorem for periodic approximation](#first-jackson-theorem-for-periodic-approximation) proves the matching upper bound. This cusp and the [critical Weierstrass modulus](#critical-weierstrass-modulus) have the same first-modulus order but different best-approximation rates.

### Endpoint obstruction to an algebraic inverse approximation theorem

↑ **Parent:** [Inverse theorem for trigonometric approximation](#inverse-theorem-for-trigonometric-approximation)

The [first Jackson theorem for periodic approximation](#first-jackson-theorem-for-periodic-approximation) applied to $|\sin\theta|$ gives algebraic best error $O(n^{-1})$ for $\sqrt{1-x^2}$. Its ordinary interval [modulus of continuity](topological-analysis.md#modulus-of-continuity) at $1/n$ is at least $\sqrt{2/n-1/n^2}$. Substituting that error rate into the unmodified [inverse theorem for trigonometric approximation](#inverse-theorem-for-trigonometric-approximation) would instead bound the modulus by $O(\log(n+1)/n)$, a contradiction. Algebraic inverse estimates must incorporate the endpoint compression of [cosine substitution for polynomial approximation](#cosine-substitution-for-polynomial-approximation).

## Korovkin theorem

↑ **Parent:** [Uniform approximation](uniform-approximation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Korovkin_theorem)

Uniform convergence of positive linear operators on $1,x,x^2$ implies uniform convergence on every continuous function on a compact interval.

### Quadratic barrier estimate for positive approximation operators

↑ **Parent:** [Korovkin theorem](#korovkin-theorem)

For [positive linear operators on continuous functions](topological-vector-space.md#positive-linear-operator-on-continuous-functions) on $[0,1]$, put $e_j=U_n(x^j)-x^j$. Uniform continuity supplies the barriers $|f(x)-f(t)|\le\varepsilon+\gamma(x-t)^2$. Applying positivity and evaluating at $t$ gives the displayed estimate because $U_n((x-t)^2)(t)=e_2(t)-2te_1(t)+t^2e_0(t)$. The constant $\gamma$ is independent of $t$ and $n$. Thus uniform reproduction of $1,x,x^2$ proves [Korovkin theorem](#korovkin-theorem) convergence on every continuous function; exact reproduction forces the operator to be the identity.

### Compact Korovkin test space

↑ **Parent:** [Korovkin theorem](#korovkin-theorem)

Let $K$ be a [compact Hausdorff space](topology.md#compact-hausdorff-space). A test subspace $H\subset C(K,\mathbb R)$ containing a strictly positive function is sufficient for [uniform convergence](real-analysis.md#uniform-convergence) of [positive linear operators on continuous functions](topological-vector-space.md#positive-linear-operator-on-continuous-functions) if, for each $x\in K$, the only [positive linear functional](continuous-dual-space.md#positive-linear-functional) agreeing with point evaluation on $H$ is that evaluation itself. By the [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem), this is uniqueness of the positive measure with the prescribed moments. Boundedness from the positive test function and the [Banach-Alaoglu theorem](functional-analysis.md#banach-alaoglu-theorem) prove the assertion by compactness. When $1\in H$, nonnegative tests with a unique zero at each prescribed $x$ give a convenient sufficient condition.

#### Periodic Korovkin test set

↑ **Parent:** [Compact Korovkin test space](#compact-korovkin-test-space)

For $2\pi$-periodic [continuous functions](calculus.md#continuous-function), convergence of [positive linear operators on continuous functions](topological-vector-space.md#positive-linear-operator-on-continuous-functions) to the identity on $1,\sin x,\cos x$ implies [uniform convergence](real-analysis.md#uniform-convergence) on every function. Indeed $1-\cos(t-x)$ is nonnegative and has just one zero on the circle, so the [compact Korovkin test space](#compact-korovkin-test-space) criterion applies.

## Spline (mathematics)

↑ **Parent:** [Uniform approximation](uniform-approximation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spline_(mathematics))

A spline is a [piecewise polynomial function](polynomial.md#piecewise-polynomial-function) whose polynomial pieces obey specified smoothness conditions at their joins, called [spline knots](#spline-knot). For example, a cubic spline is cubic on each interval and commonly has two continuous derivatives across interior knots. [Spline approximation](#spline-approximation) and [spline interpolation](#spline-interpolation) use these finite-dimensional function spaces to represent data or approximate functions.

### Linear spline

↑ **Parent:** [Spline (mathematics)](#spline-mathematics)

A [linear spline](#linear-spline) is a continuous [piecewise linear function](function.md#piecewise-linear-function) on a specified [spline knot sequence](#spline-knot-sequence). For uniform integer [spline knots](#spline-knot), the hat basis in the displayed representation interpolates the data $s(i)=c_i$. The [derivative](calculus.md#derivative) is constant on each open span and can jump at a knot. Coinciding neighboring slopes remove a particular jump, but generic data give only $C^0$ regularity.

### Spline approximation

↑ **Parent:** [Spline (mathematics)](#spline-mathematics)

#### Spline quasi-interpolation

↑ **Parent:** [Spline approximation](#spline-approximation)

A [spline](#spline-mathematics) quasi-interpolant synthesizes a [B-spline](#b-spline) expansion from local bounded [linear functionals](linear-algebra.md#linear-functional), instead of solving a global interpolation system. Suppose each functional is bounded by $c_k\|f\|_{C[t_i,t_{i+k}]}$ and the operator reproduces every [spline](#spline-mathematics). On a knot cell $[t_j,t_{j+1}]$, only indices $j+1-k\le i\le j$ contribute. Their [supports](function.md#support) lie in $[t_{j+1-k},t_{j+k}]$, and [subpartition of unity for B-splines](#subpartition-of-unity-for-b-splines) proves local [operator norm](continuous-dual-space.md#operator-norm) at most $c_k$. Reproduction of degree-$k-1$ [polynomials](polynomial.md) and a local [Taylor theorem](calculus.md#taylor-theorem) remainder then give error at most $(1+c_k)(2k-1)^k h^k\|f^{(k)}\|_\infty/k!$, on the basic knot domain with the usual completed boundary [basis](vector-space.md#basis).

#### Box spline

↑ **Parent:** [Spline approximation](#spline-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Box_spline)

For a spanning direction matrix $\Xi=(\xi_1,\ldots,\xi_m)$ in $\mathbb R^d$, the [box spline](#box-spline) is the density of the pushforward of uniform measure on $[0,1]^m$ under $t\mapsto\Xi t$. Equivalently,

$$
\int_{\mathbb R^d}M_\Xi(x)\varphi(x)\,dx=\int_{[0,1]^m}\varphi(\Xi t)\,dt.
$$

Its support is the [zonotope](mathematical-optimization.md#zonotope) $\sum_j[0,1]\xi_j$. It is piecewise polynomial of total degree at most $m-d$. For integer directions, splitting each integration interval in half yields its binary refinement symbol

$$
2^d\prod_{j=1}^m\frac{1+z^{\xi_j}}2,
$$

up to the monomial specifying the choice of origin. If $r$ is the smallest number of directions whose removal leaves a nonspanning set, the usual [box spline](#box-spline) smoothness criterion gives $C^{r-2}$ regularity. Repeated directions increase smoothness while enlarging support.

##### Unit-direction univariate box spline

↑ **Parent:** [Box spline](#box-spline)

The unit-direction univariate [box spline](#box-spline) is the density of the sum of $m$ independent uniform unit-interval coordinates. It is the order-$m$ [Cardinal B-spline](#cardinal-b-spline): its closed support is $[0,m]$, it is strictly positive on the interior, and its [polynomial](polynomial.md) degree is $m-1$. For $m\geq2$ it is $C^{m-2}$, generally not $C^{m-1}$. The recurrence $B_m(x)=\int_0^1B_{m-1}(x-u)du$ proves its support and positivity. Starting with a half-open unit interval, integrating the translate partition recursively proves $\sum_{j\in\mathbb Z}B_m(x-j)=1$. Orthogonal projection onto the unit diagonal rescales support width from $m$ to $\sqrt m$.

##### Quadratic four-direction box spline

↑ **Parent:** [Box spline](#box-spline)

This [box spline](#box-spline) is the density of the image of the uniform unit four-cube under the indicated direction [matrix](vector-space.md#matrix). Its [polynomial](polynomial.md) pieces have total degree $4-2=2$. Removing three directions is necessary to leave a nonspanning set, giving $C^1$ [continuity](calculus.md#continuous-function). Its knot arrangement is a criss-cross triangulation of a square lattice. Its refinement mask is $\frac14(1+z)(1+w)(1+zw)(1+z/w)$, up to the monomial that fixes the origin.

##### Twice-smoothed four-direction box spline

↑ **Parent:** [Box spline](#box-spline)

Take two copies of each direction $(1,0),(0,1),(1,1),(1,-1)$. The resulting [box spline](#box-spline) has total polynomial degree six and $C^4$ continuity: there are eight directions and a rank-deficient remaining set has at most two, so the removal number is six. With a centred origin its support is the [zonotope](mathematical-optimization.md#zonotope)

$$
\{|x|\leq3,\ |y|\leq3,\ |x|+|y|\leq4\}.
$$

Its centred binary symbol is

$$
\frac{(1+z)^2(1+w)^2(1+zw)^2(1+z/w)^2}{64z^3w}.
$$

This symbol factors as $A(z,w)A(zw,z/w)$ with $A=(2+z+z^{-1})(2+w+w^{-1})/8$, giving an efficient [quincunx subdivision](numerical-analysis.md#quincunx-subdivision) implementation. The [box spline](#box-spline) criterion is also described in the primary research paper [4–8 Subdivision](https://cims.nyu.edu/gcl/papers/velho20014s.pdf) by Velho and Zorin.

#### Quadratic spline

↑ **Parent:** [Spline approximation](#spline-approximation)

A quadratic [spline](#spline-mathematics) with simple knots is a continuously differentiable [function](function.md) that is a [polynomial](polynomial.md) of degree at most two between successive knots. Its first [derivative](calculus.md#derivative) is continuous and piecewise linear, while its second [derivative](calculus.md#derivative) is piecewise constant and can jump at knots. Constant tails impose vanishing first derivatives at the outermost knots. Such a spline arises from first-derivative roughness penalization when observations are interval averages, as in the [quadratic smoothing spline for interval averages](nonparametric-statistics.md#quadratic-smoothing-spline-for-interval-averages).

#### Spline interpolation

↑ **Parent:** [Spline approximation](#spline-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spline_interpolation)

Spline interpolation matches prescribed function values at distinct sites by an element of a finite-dimensional spline space. In a [B-spline](#b-spline) basis its existence and uniqueness for all data are equivalent to invertibility of the [B-spline collocation matrix](#b-spline-collocation-matrix). Distinct ordered sites satisfying the [Schoenberg–Whitney theorem](#schoenberg-whitney-theorem) give this condition.

##### Spline interpolation operator

↑ **Parent:** [Spline interpolation](#spline-interpolation)

For a fixed spline space and admissible interpolation sites, this linear operator sends a [continuous function](calculus.md#continuous-function) to its unique interpolating spline. Here $Rf$ is the vector of sampled values and $A$ is the [B-spline collocation matrix](#b-spline-collocation-matrix). It reproduces every spline in its range. Its sensitivity to perturbing the data is quantified by the [B-spline interpolation operator norm](#b-spline-interpolation-operator-norm).

###### Centered quadratic spline interpolation

↑ **Parent:** [Spline interpolation operator](#spline-interpolation-operator)

For unit-spaced order-three [B-splines](#b-spline) sampled at [support](function.md#support) midpoints $i+3/2$, the [B-spline collocation matrix](#b-spline-collocation-matrix) has diagonal $3/4$ and neighboring entries $1/8$. Conjugating by alternating diagonal signs reduces its inverse absolute values to the nonnegative inverse of $\operatorname{tridiag}(-1,6,-1)/8$. With $\tau=3-2\sqrt2$, the absolute row sums are $r_i=2[1-(\tau^i+\tau^{n+1-i})/(1+\tau^{n+1})]$. This follows by solving $6r_i-r_{i-1}-r_{i+1}=8$ with $r_0=r_{n+1}=0$. The maximum occurs at the middle row or rows and tends to two as $n$ grows. Nonnegativity and subpartition of unity of the [B-splines](#b-spline) transfer this bound to the [spline interpolation operator](#spline-interpolation-operator).

###### B-spline interpolation operator norm

↑ **Parent:** [Spline interpolation operator](#spline-interpolation-operator)

For distinct interpolation sites and an invertible [B-spline collocation matrix](#b-spline-collocation-matrix), the interpolant is $P=BA^{-1}R$, where $R$ samples data and $Ba=\sum_i a_iN_i$. Sampling and basis synthesis have [operator norms](continuous-dual-space.md#operator-norm) at most one in the [supremum norm](functional-analysis.md#supremum-norm). For the reverse inequality, realize the signs of a maximal absolute row sum of $A^{-1}$ as values of a continuous function of norm one, and apply [uniform-norm stability of a B-spline basis](#uniform-norm-stability-of-a-b-spline-basis). This yields both displayed bounds.

###### Linear growth of shifted quadratic spline interpolation

↑ **Parent:** [B-spline interpolation operator norm](#b-spline-interpolation-operator-norm)

For the degree-two [Cardinal B-spline](#cardinal-b-spline) basis on knots $1,\ldots,n+3$, sampling at $x_i=i+2$ gives the upper-bidiagonal [B-spline collocation matrix](#b-spline-collocation-matrix) $A=(I+S)/2$, where $S$ is the one-step upper shift. Since $S^n=0$, $A^{-1}=2\sum_{r=0}^{n-1}(-S)^r$ and its maximum absolute row sum is $2n$. The [B-spline interpolation operator norm](#b-spline-interpolation-operator-norm) estimate with the order-three stability constant $d_3=3$ gives the displayed linear upper and lower bounds. The lower bound proves failure of uniform boundedness.

#### Maximum-norm bound for spline projection

↑ **Parent:** [Spline approximation](#spline-approximation)

For the orthogonal [B-spline](#b-spline) projector $P$, the normal equations in the [mixed-normalization spline Gram matrix](#mixed-normalization-spline-gram-matrix) give $Ga=r$, with $r_i=(M_i,f)$. Positivity and unit integral of $M_i$ imply $\|r\|_{\ell^\infty}\leq\|f\|_\infty$. Nonnegativity and subpartition of unity of $N_i$ give $\|\sum_ia_iN_i\|_\infty\leq\|a\|_{\ell^\infty}$. Hence $\|P\|_\infty\leq\|G^{-1}\|_{\ell^\infty}$, where the matrix norm is maximum absolute row sum. The range is the spline space, which lies in $C[0,1]$ only for continuous splines.

#### Regression spline

↑ **Parent:** [Spline approximation](#spline-approximation)

A [regression spline](#regression-spline) fits a [regression function](statistical-learning.md#regression-function) in a finite-dimensional [spline approximation](#spline-approximation) space with selected knots. Evaluating its basis at predictor values gives a [design matrix](linear-regression.md#design-matrix), reducing fitting to regression on basis coefficients.

##### Cubic regression spline

↑ **Parent:** [Regression spline](#regression-spline)

A cubic regression spline represents a mean function in a finite-dimensional space of piecewise cubic functions, with continuity of the function and its first two derivatives at chosen knots. A penalized fit minimizes a residual criterion plus $\lambda\int(f'')^2$, using $\Omega_{jk}=\int B_j''B_k''$. Unlike a full [cubic smoothing spline](nonparametric-statistics.md#cubic-smoothing-spline) with knots at every distinct observation, its knot set can be much smaller. The `mgcv` basis `bs="cr"` uses a penalized natural cubic regression-spline basis with linear tails.

##### Penalized regression spline

↑ **Parent:** [Regression spline](#regression-spline)

A penalized [regression spline](#regression-spline) estimates basis coefficients by minimizing a residual or likelihood criterion plus a curvature penalty. Basis size limits the available complexity; the penalty controls how much of that complexity is used.

#### Second derivative roughness penalty

↑ **Parent:** [Spline approximation](#spline-approximation)

The nonnegative functional $J(g)=\int_a^b(g^{\prime\prime}(x))^2\,dx$. Its [null space](linear-algebra.md#kernel-of-a-linear-map) on $C^2[a,b]$ consists of [affine functions](vector-space.md#affine-function). The [natural cubic spline interpolant](#natural-cubic-spline-interpolant) uniquely minimizes this penalty among functions matching at least two prescribed knot values. It is a squared [second derivative](calculus.md#second-derivative) penalty, not the exact geometric curvature energy of a graph.

#### Spline knot

↑ **Parent:** [Spline approximation](#spline-approximation)

A junction between adjacent [polynomial](polynomial.md) pieces of a [cubic spline](#cubic-spline) or other spline. [Continuity](calculus.md#continuous-function) conditions at these junctions determine which piecewise [polynomial](polynomial.md) functions are splines.

##### Spline knot sequence

↑ **Parent:** [Spline knot](#spline-knot)

A spline knot sequence is a nondecreasing list of [spline knots](#spline-knot), including their multiplicities, that specifies the junctions and smoothness constraints of a spline space. An order-$k$ [B-spline](#b-spline) uses $k+1$ consecutive knot entries. Its support must have positive width, and repeated knots are interpreted by confluent [divided differences](numerical-analysis.md#divided-difference) or their limiting convention.

#### Cubic spline

↑ **Parent:** [Spline approximation](#spline-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cubic_spline)

A cubic spline is a twice continuously differentiable piecewise polynomial of degree at most three whose polynomial pieces meet at specified knots.

##### Natural cubic spline

↑ **Parent:** [Cubic spline](#cubic-spline)

A natural cubic spline is linear beyond its two outer knots, equivalently its second derivative vanishes at those knots.

###### Natural cubic spline interpolant

↑ **Parent:** [Natural cubic spline](#natural-cubic-spline)

For at least two distinct knots $x_1<\cdots<x_n$ and values $v_i$, the unique [natural cubic spline](#natural-cubic-spline) matching those values and linear beyond $x_1,x_n$. Its interpolation map is a [linear map](vector-space.md#linear-map) by uniqueness. Over a larger domain $[a,b]$, the two exterior pieces remain linear. With only one knot, arbitrary slopes of [affine functions](vector-space.md#affine-function) make uniqueness false.

###### Spline roughness penalty matrix

↑ **Parent:** [Natural cubic spline interpolant](#natural-cubic-spline-interpolant)

Let $b_i=N e_i$ be the interpolating cardinal basis and set $\Gamma_{ij}=\int_a^b b_i^{\prime\prime}b_j^{\prime\prime}\,dx$. Linearity gives $J(N\mathbf v)=\mathbf v^T\Gamma\mathbf v$, and this [Gram matrix](linear-algebra.md#gram-matrix) is a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix). Its [null space](linear-algebra.md#kernel-of-a-linear-map) consists precisely of [vectors](vector-space.md#vector) $(\alpha+\beta x_i)_i$, by the null-space statement for the [second derivative roughness penalty](#second-derivative-roughness-penalty). Thus its rank is $n-2$, including the zero [matrix](vector-space.md#matrix) when $n=2$.

###### Minimum roughness property of the natural cubic spline interpolant

↑ **Parent:** [Natural cubic spline interpolant](#natural-cubic-spline-interpolant)

For $g=N\mathbf v$ and any $\widetilde g\in C^2[a,b]$ taking the same values at at least two distinct knots, $J(\widetilde g)=J(g)+J(\widetilde g-g)$. To prove it, set $r=\widetilde g-g$, integrate $g^{\prime\prime}r^{\prime\prime}$ by parts on each [polynomial](polynomial.md) interval and use $g^{(4)}=0$, $r(x_i)=0$, [continuous](calculus.md#continuous-function) $g^{\prime\prime}$ and linear exterior pieces. Boundary terms cancel. Expanding the square proves the identity. Equality forces $r^{\prime\prime}=0$, so $r$ is an [affine function](vector-space.md#affine-function) and its two prescribed zeros make it identically zero.

###### Minimum roughness property with absolutely continuous first derivatives

↑ **Parent:** [Minimum roughness property of the natural cubic spline interpolant](#minimum-roughness-property-of-the-natural-cubic-spline-interpolant)

The [minimum roughness property of the natural cubic spline interpolant](#minimum-roughness-property-of-the-natural-cubic-spline-interpolant) extends to interpolants with an absolutely continuous first derivative and square-integrable [second derivative](calculus.md#second-derivative). For $h=f-g$ vanishing at the knots, integration by parts on each cubic interval gives $\int g''h''=0$: the knot boundary terms cancel by continuity, the exterior terms vanish by natural boundary conditions, and the remaining constant-third-derivative term vanishes because $h$ is zero at the interval endpoints. Expanding the square proves minimality. Equality makes $h$ affine; its zeros at two distinct knots force $h=0$, proving uniqueness. Competitors with infinite roughness cannot improve the finite spline penalty.

#### B-spline

↑ **Parent:** [Spline approximation](#spline-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/B-spline)

A B-spline is a compactly supported piecewise polynomial basis function determined by consecutive knots.

##### B-spline differentiation formula

↑ **Parent:** [B-spline](#b-spline)

For the partition-of-unity normalization, the derivative of a degree-$d$ [B-spline](#b-spline) is the displayed difference of two overlapping degree-$(d-1)$ [B-splines](#b-spline). A zero denominator denotes a term with collapsed support, assigned zero. For simple knots the divided-difference representation $N_{i,d}(t)=(t_{i+d+1}-t_i)[t_i,\ldots,t_{i+d+1}](\tau-t)_+^d$ has the required support, smoothness and integral normalization. Differentiate the truncated power and apply the last-step [divided difference](numerical-analysis.md#divided-difference) recursion to obtain the formula. Repeated-knot versions follow by confluent limits, with one-sided interpretation where necessary.

##### Local linear independence of B-splines

↑ **Parent:** [B-spline](#b-spline)

The $k$ order-$k$ [B-splines](#b-spline) active on a simple-knot cell form a [basis](vector-space.md#basis) of its degree-$k-1$ [polynomials](polynomial.md). To see this from [Marsden's identity](#marsden-identity), use the dual [polynomials](polynomial.md) $\psi_i(y)=\prod_{\ell=1}^{k-1}(y-t_{i+\ell})$. On $t_j<x<t_{j+1}$ the identity is $(y-x)^{k-1}=\sum_{i=j-k+1}^jN_i(x)\psi_i(y)$. Evaluation of the dual [polynomials](polynomial.md) at $t_j,t_{j-1},\ldots,t_{j-k+1}$ gives a triangular [coefficient](vector-space.md#coefficient) [matrix](vector-space.md#matrix) with nonzero diagonal. They are independent, and comparison of [coefficients](vector-space.md#coefficient) of $y$ in the identity gives independence of the active [splines](#spline-mathematics). Consequently a [spline](#spline-mathematics) vanishes on a whole open cell exactly when all its active [coefficients](vector-space.md#coefficient) vanish.

##### Compact-support spline zero count

↑ **Parent:** [B-spline](#b-spline)

Let the real [spline](#spline-mathematics) $s=\sum_{i=p}^qc_iN_i$ have distinct knots, order $k\ge2$, nonzero endpoint [coefficients](vector-space.md#coefficient), and no identically zero knot cell in its [support](function.md#support). It and its first $k-2$ [derivatives](calculus.md#derivative) vanish at both [support](function.md#support) endpoints. If $Z$ is its number of interior distinct zeros, there are initially $Z+2$ zero components. Each differentiation through order $k-2$ increases this count by at least one: a nonzero gap between zero components has an interior extremum, and the two endpoint zeros remain separate. The final [derivative](calculus.md#derivative) is continuous piecewise linear on $q-p+k$ cells, and each cell can meet at most one zero component unless it is identically zero, in which case all its zeros belong to the same component. It therefore has at most $q-p+k$ zero components. Thus $Z+k\le q-p+k$, proving the bound.

##### Quartic treble-knot representation of a quadratic B-spline

↑ **Parent:** [B-spline](#b-spline)

For a uniform quadratic [B-spline](#b-spline) with interior [control points](numerical-analysis.md#control-point) $P_i$, label its $i$th span $[i,i+1]$. A quartic [B-spline](#b-spline) with interior [spline knot sequence](#spline-knot-sequence) $\tau_{3i}=\tau_{3i+1}=\tau_{3i+2}=i$ represents the identical curve when

$$
Q_{3i-1}=\frac{P_{i-1}+3P_i}{4},\quad Q_{3i}=\frac{P_{i-1}+10P_i+P_{i+1}}{12},\quad Q_{3i+1}=\frac{3P_i+P_{i+1}}4.
$$

To verify this, raise each quadratic [Bézier curve](numerical-analysis.md#bezier-curve) span twice by [degree elevation of Bernstein coefficients](functional-analysis.md#degree-elevation-of-bernstein-coefficients). The three interior quartic controls are the displayed points. One additional [knot insertion](#knot-insertion) at each interior knot supplies the shared endpoint as the mean of its two neighboring controls, recovering all five quartic [Bézier curve](numerical-analysis.md#bezier-curve) controls. Thus the knot multiplicity is three, giving $C^1$ joins rather than imposing unwanted extra smoothness.

##### Non-uniform rational B-spline

↑ **Parent:** [B-spline](#b-spline)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-uniform_rational_B-spline)

A [non-uniform rational B-spline](#non-uniform-rational-b-spline) surface is

$$
F(u,v)=\frac{\sum_{i,j}w_{ij}N_{i,p}(u)M_{j,q}(v)P_{ij}}{\sum_{i,j}w_{ij}N_{i,p}(u)M_{j,q}(v)}.
$$

Here the $N_{i,p}$ and $M_{j,q}$ are [B-spline](#b-spline) basis functions for possibly nonuniform [spline knot sequences](#spline-knot-sequence), and the $w_{ij}$ are weights. Positive weights make each evaluated point a [convex combination](mathematical-optimization.md#convex-combination) of the active [control points](numerical-analysis.md#control-point), supplying [bounding volumes](numerical-analysis.md#bounding-volume) for geometric searches. The denominator must remain nonzero for the parametrization to be defined.

##### Knot insertion

↑ **Parent:** [B-spline](#b-spline)

[Knot insertion](#knot-insertion) refines the [spline knot sequence](#spline-knot-sequence) and changes the control points without changing the represented [B-spline](#b-spline). Repeated insertion exposes local [Bézier curves](numerical-analysis.md#bezier-curve) and provides subdivision-based evaluation.

// Target: analysis.bigb

<h5 id="de-boor-s-algorithm">De Boor's algorithm</h5>

↑ **Parent:** [B-spline](#b-spline)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Boor's_algorithm)

For degree $p$, knots $t_i$ and span $[t_k,t_{k+1})$, initialize $d_j^{(0)}=P_{k-p+j}$ for $0\le j\le p$. At level $r$, update $j=p,p-1,\ldots,r$ by $d_j^{(r)}=(1-\alpha_{j,r})d_{j-1}^{(r-1)}+\alpha_{j,r}d_j^{(r-1)}$, where $\alpha_{j,r}=(t-t_{k-p+j})/(t_{k+1+j-r}-t_{k-p+j})$. The point is $d_p^{(p)}$. This evaluates a [B-spline](#b-spline) by local affine combinations.

// Target: analysis.bigb

##### Unit-integral normalization of a B-spline

↑ **Parent:** [B-spline](#b-spline)

For strictly increasing [spline knots](#spline-knot), $M_i(t)=k[t_i,\ldots,t_{i+k}](\cdot-t)_+^{k-1}$ is a nonnegative integral-normalized [B-spline](#b-spline). Integrating the [truncated power function](polynomial.md#truncated-power-function) over its [support](function.md#support) replaces its [spline knot](#spline-knot) value by $(u-t_i)^k/k$. The order-$k$ [divided difference](numerical-analysis.md#divided-difference) of this degree-$k$ [polynomial](polynomial.md) is its [leading coefficient](polynomial.md#leading-coefficient-of-a-polynomial) $1/k$. Multiplying by the prefactor $k$ in $M_i$ gives integral one. The corresponding partition-normalized [B-spline](#b-spline) is $N_i=(t_{i+k}-t_i)M_i/k$.

##### Uniform-norm stability of a B-spline basis

↑ **Parent:** [B-spline](#b-spline)

For a linearly independent partition-normalized [B-spline](#b-spline) basis, equivalence of norms gives a lower coefficient-stability constant. The upper bound follows from the [subpartition of unity for B-splines](#subpartition-of-unity-for-b-splines). A knot-independent stability bound can be chosen depending on spline order. This norm comparison transfers matrix estimates to the [B-spline interpolation operator norm](#b-spline-interpolation-operator-norm).

###### Coefficient condition number of a normalized B-spline basis

↑ **Parent:** [Uniform-norm stability of a B-spline basis](#uniform-norm-stability-of-a-b-spline-basis)

For a nonnegative partition-normalized [B-spline](#b-spline) [basis](vector-space.md#basis), the synthesis [linear map](vector-space.md#linear-map) $Tc=\sum_jc_jN_j$ has [operator norm](continuous-dual-space.md#operator-norm) one. Its [condition number](linear-algebra.md#condition-number) is consequently $\|T^{-1}\|$, with the [supremum norm](functional-analysis.md#supremum-norm) on the [spline](#spline-mathematics) space and the maximum [norm](functional-analysis.md#norm) on its [coefficients](vector-space.md#coefficient). The [uniform-norm stability of a B-spline basis](#uniform-norm-stability-of-a-b-spline-basis) bounds this number independently of the [spline knot sequence](#spline-knot-sequence) when the order is fixed. This is different from the [condition number](linear-algebra.md#condition-number) of a particular sampled [B-spline collocation matrix](#b-spline-collocation-matrix).

###### Chebyshev spline coefficient and dual norm equality

↑ **Parent:** [Uniform-norm stability of a B-spline basis](#uniform-norm-stability-of-a-b-spline-basis)

Suppose $\|s_*\|_\infty=1$ and $s_*(x_j)=(-1)^j$ at increasing sites satisfying the [Schoenberg–Whitney theorem](#schoenberg-whitney-theorem) conditions. For the [B-spline collocation matrix](#b-spline-collocation-matrix) $A$, the coefficient [linear functional](linear-algebra.md#linear-functional) in the [dual basis](linear-algebra.md#dual-basis) is $\mu_i(s)=\sum_j(A^{-1})_{ij}s(x_j)$. Therefore $\|\mu_i\|\leq\sum_j|(A^{-1})_{ij}|$. The [checkerboard inverse of a totally nonnegative matrix](vector-space.md#checkerboard-inverse-of-a-totally-nonnegative-matrix) makes $\mu_i(s_*)=(-1)^i\sum_j|(A^{-1})_{ij}|$, attaining that bound. Since $\mu_i(s_*)=a_i^*$,

$$
|a_i^*|=\|\mu_i\|=\sum_j|(A^{-1})_{ij}|.
$$

The conclusion is an extremal property of an alternating unit-norm [spline](#spline-mathematics), not a claim that every bounded [spline](#spline-mathematics) has these extremal coefficients.

###### Optimal spline coefficient interpolation sites

↑ **Parent:** [Chebyshev spline coefficient and dual norm equality](#chebyshev-spline-coefficient-and-dual-norm-equality)

The equality holds when an alternating unit-norm [spline](#spline-mathematics) $s_*$ has as many ordered extremal sites as the dimension, and those sites satisfy the [Schoenberg–Whitney theorem](#schoenberg-whitney-theorem). For every admissible set, sampling has [operator norm](continuous-dual-space.md#operator-norm) at most one, giving $\kappa(\mathcal S)\le\|A_{\mathbf x}^{-1}\|_\infty$. At the alternating sites the [checkerboard inverse of a totally nonnegative matrix](vector-space.md#checkerboard-inverse-of-a-totally-nonnegative-matrix) identifies each inverse absolute row sum with the magnitude of the corresponding [coefficient](vector-space.md#coefficient) of $s_*$. The [Chebyshev spline coefficient and dual norm equality](#chebyshev-spline-coefficient-and-dual-norm-equality) therefore gives equality. This minimizes amplification into [B-spline](#b-spline) [coefficients](vector-space.md#coefficient); it does not by itself prove optimality for the distinct [Lebesgue constant of interpolation](#lebesgue-constant-of-interpolation).

##### Subpartition of unity for B-splines

↑ **Parent:** [B-spline](#b-spline)

A finite collection of the standard partition-normalized [B-splines](#b-spline) is nonnegative and has sum at most one on the entire real line. Extend the knot sequence in both directions. The full order-one collection sums to one, and summing the [Cox-de Boor recurrence](#cox-de-boor-recursion-formula) preserves that sum because the two coefficients of each lower-order function add to one. The finite collection is a subset. On the basic knot interval the finite sum equals one, also following from [Marsden's identity](#marsden-identity).

##### Simple-knot B-spline regularity

↑ **Parent:** [B-spline](#b-spline)

For distinct increasing knots and $k\ge2$, the explicit [divided difference](numerical-analysis.md#divided-difference) formula writes an order-$k$ [B-spline](#b-spline) as a finite sum of [truncated power functions](polynomial.md#truncated-power-function) of degree $k-1$. It is a [piecewise polynomial function](polynomial.md#piecewise-polynomial-function) and is globally $C^{k-2}$. Below its first knot the order-$k$ [divided difference](numerical-analysis.md#divided-difference) annihilates a degree-$k-1$ polynomial; above its last knot all values vanish. Nonzero first and last pieces give the exact closed support. Order one gives interval indicators instead of continuous splines.

##### Support and Gram bandwidth of B-splines

↑ **Parent:** [B-spline](#b-spline)

An order-$k$ [B-spline](#b-spline) is supported on $[t_i,t_{i+k}]$. Below this interval its truncated-power knot data agree with a degree-$k-1$ polynomial, annihilated by the order-$k$ [divided difference](numerical-analysis.md#divided-difference); above it all data vanish. Therefore its ordinary or mixed [Gram matrix](linear-algebra.md#gram-matrix) has entries zero when $|i-j|\geq k$. The half-bandwidth is $k-1$, and for strictly increasing knots this bound is sharp.

##### Mixed-normalization spline Gram matrix

↑ **Parent:** [B-spline](#b-spline)

For partition-normalized [B-splines](#b-spline) $N_i$ and integral-normalized $M_i=kN_i/(t_{i+k}-t_i)$, let $H_{ij}=(N_i,N_j)$ and $D_{ii}=(t_{i+k}-t_i)/k$. The mixed matrix $G_{ij}=(M_i,N_j)$ equals $D^{-1}H$. It is invertible whenever the splines form a basis and their support widths are positive. It need not be symmetric, unlike the ordinary [Gram matrix](linear-algebra.md#gram-matrix).

###### Uniform norm bound for B-spline orthogonal projection

↑ **Parent:** [Mixed-normalization spline Gram matrix](#mixed-normalization-spline-gram-matrix)

Let nonnegative partition-normalized [B-splines](#b-spline) $N_i$ form a [basis](vector-space.md#basis), with $\sum_iN_i\le1$ on the integration interval and $d_i=\int N_i>0$. The row-normalized mixed [Gram matrix](linear-algebra.md#gram-matrix) is $G_{ij}=\int N_iN_j/d_i$. The [normal equations](statistical-modelling.md#normal-equation) for the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto their [linear span](vector-space.md#linear-span) become $Ga=b$, with $b_i=\int fN_i/d_i$ and $\|b\|_{\ell^\infty}\le\|f\|_\infty$. The [subpartition of unity for B-splines](#subpartition-of-unity-for-b-splines) gives $\|\sum_i a_iN_i\|_\infty\le\|a\|_{\ell^\infty}$ and proves the bound. The ordinary symmetric Gram matrix omits this essential row normalization. The projection maps continuous functions into the spline space, not onto all continuous functions.

###### Linear-spline mixed Gram matrix

↑ **Parent:** [Mixed-normalization spline Gram matrix](#mixed-normalization-spline-gram-matrix)

For the distinct-knot linear [B-spline](#b-spline) hats, let $h_i=t_{i+1}-t_i>0$. The [mixed-normalization spline Gram matrix](#mixed-normalization-spline-gram-matrix) has entries

$$
g_{ii}=\frac23,\quad g_{i,i-1}=\frac{h_i}{3(h_i+h_{i+1})},\quad g_{i,i+1}=\frac{h_{i+1}}{3(h_i+h_{i+1})},\quad g_{ij}=0\quad(|i-j|\ge2).
$$

Only indices in the finite [basis](vector-space.md#basis) are retained. This [matrix](vector-space.md#matrix) has a row [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix) margin at least $1/3$, so the [inverse infinity-norm bound from diagonal dominance](vector-space.md#inverse-infinity-norm-bound-from-diagonal-dominance) gives $\|G^{-1}\|_{\ell^\infty}\le3$. Equidistant [spline knots](#spline-knot) give off-diagonal entries $1/6$. Both pieces of every hat are retained; repeated endpoint [spline knots](#spline-knot) require different boundary formulas.

##### Lee interpolation identity

↑ **Parent:** [B-spline](#b-spline)

For distinct increasing knots, let $\ell_i(\cdot,t)$ interpolate $(\cdot-t)_+^{k-1}$ on $t_i,\ldots,t_{i+k-1}$ and let $\omega_i(x)=\prod_{r=1}^{k-1}(x-t_{i+r})$. Adjacent interpolants share $k-1$ values; their difference is a multiple of $\omega_i$. Its leading coefficient, by the [divided difference](numerical-analysis.md#divided-difference) recurrence, is the order-$k$ [B-spline](#b-spline) $N_i(t)$. Thus $\ell_{i+1}(x,t)-\ell_i(x,t)=\omega_i(x)N_i(t)$. Telescoping proves the [Marsden identity](#marsden-identity). Repeated knots require the well-defined confluent or limiting convention.

##### Cardinal B-spline

↑ **Parent:** [B-spline](#b-spline)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cardinal_B-spline)

A cardinal B-spline is a B-spline whose knots are consecutive integers.

###### Quintic cardinal spline midpoint collocation

↑ **Parent:** [Cardinal B-spline](#cardinal-b-spline)

Sampling consecutive order-six [Cardinal B-splines](#cardinal-b-spline) at their support midpoints gives the displayed finite [B-spline collocation matrix](#b-spline-collocation-matrix). No exterior columns are retained. Its row [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix) margin is at least $(66-2\cdot26-2)/120=1/10$, so the [inverse infinity-norm bound from diagonal dominance](vector-space.md#inverse-infinity-norm-bound-from-diagonal-dominance) gives $\|A^{-1}\|_{\ell^\infty}\le10$. The uniform knot samples are $N_{0,6}(0),\ldots,N_{0,6}(6)=(0,1,26,66,26,1,0)/120$, obtained recursively from the [Cox-de Boor recurrence](#cox-de-boor-recursion-formula).

###### Quadratic cardinal B-spline

↑ **Parent:** [Cardinal B-spline](#cardinal-b-spline)

This degree-two [Cardinal B-spline](#cardinal-b-spline) has three consecutive unit knot intervals as its support. Its first and last polynomial pieces are $(t-i)^2/2$ and $(i+3-t)^2/2$; on the middle interval it equals $3/4-(t-i-3/2)^2$. Its two interior integer values are $1/2$, and its endpoint values are zero. The maximum is $3/4$, emphasizing that partition normalization does not mean unit maximum height.

###### Midpoint quadratic spline collocation

↑ **Parent:** [Quadratic cardinal B-spline](#quadratic-cardinal-b-spline)

Sampling order-three [Cardinal B-splines](#cardinal-b-spline) $N_j$ at $x_i=i+3/2$ gives $N_i(x_i)=3/4$, $N_{i-1}(x_i)=N_{i+1}(x_i)=1/8$, and all other entries zero. The [B-spline collocation matrix](#b-spline-collocation-matrix) therefore has row [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix) margin at least $1/2$, giving inverse [operator norm](continuous-dual-space.md#operator-norm) at most two. More precisely, with $q=3-2\sqrt2$, its absolute inverse row sums are $v_i=2[1-(q^i+q^{n+1-i})/(1+q^{n+1})]$. To see this, change signs by $D_{ii}=(-1)^i$: $DAD$ has negative off-diagonal entries and a nonnegative inverse given by a convergent [Neumann series](banach-algebra.md#neumann-series). Its inverse row sums solve $6v_i-v_{i-1}-v_{i+1}=8$, $v_0=v_{n+1}=0$. Thus $\|A^{-1}\|_\infty=v_{\lfloor(n+1)/2\rfloor}<2$, tending to two as the dimension grows.

###### Cardinal cubic B-spline

↑ **Parent:** [Cardinal B-spline](#cardinal-b-spline)

A cardinal cubic B-spline is a degree-three [Cardinal B-spline](#cardinal-b-spline). At the three interior integer knots, its nonzero normalized values are $1/6$, $4/6$, and $1/6$.

<h6 id="cubic-b-spline-bezier-extraction">Cubic B-spline Bézier extraction</h6>

↑ **Parent:** [Cardinal cubic B-spline](#cardinal-cubic-b-spline)

For the unit-spaced cubic cardinal [B-spline](#b-spline) on $[0,4]$, the four scalar cubic [Bernstein basis](functional-analysis.md#bernstein-basis) coefficient rows are $(0,0,0,1/6)$, $(1/6,1/3,2/3,2/3)$, $(2/3,2/3,1/3,1/6)$ and $(1/6,0,0,0)$. Each row applies on its interval with local parameter in $[0,1]$. They result from the compactly supported $C^2$ truncated-cube combination $\tfrac16\sum_{j=0}^4(-1)^j\binom4j(x-j)_+^3$. Each graph piece is a cubic [Bézier curve](numerical-analysis.md#bezier-curve) with abscissa controls $j,j+1/3,j+2/3,j+1$.

###### Midpoint cubic spline collocation

↑ **Parent:** [Cardinal cubic B-spline](#cardinal-cubic-b-spline)

Sampling consecutive [Cardinal cubic B-splines](#cardinal-cubic-b-spline) at the centers of their supports gives diagonal values $2/3$ and adjacent values $1/6$, with all other values zero. Finite truncation gives the displayed [B-spline collocation matrix](#b-spline-collocation-matrix), including its endpoint rows without wrapping or adding boundary conditions. Its inverse has alternating signs. The [exact inverse norm of midpoint cubic spline collocation](#exact-inverse-norm-of-midpoint-cubic-spline-collocation) is less than three for each finite dimension and approaches three as the dimension grows.

###### Exact inverse norm of midpoint cubic spline collocation

↑ **Parent:** [Midpoint cubic spline collocation](#midpoint-cubic-spline-collocation)

Conjugate the collocation [matrix](vector-space.md#matrix) by the diagonal [matrix](vector-space.md#matrix) with entries $(-1)^i$. The resulting negative-off-diagonal [matrix](vector-space.md#matrix) has a nonnegative inverse, as a convergent [Neumann series](banach-algebra.md#neumann-series) shows. The absolute inverse row sums are therefore the entries of its inverse applied to the all-ones vector. They solve $4u_i-u_{i-1}-u_{i+1}=6$ with $u_0=u_{n+1}=0$, whose solution is displayed. The maximum occurs at the central row or central two rows and equals the inverse [operator norm](continuous-dual-space.md#operator-norm) on $\ell^\infty$. Consequently the associated [spline interpolation operator](#spline-interpolation-operator) has [norm](functional-analysis.md#norm) at most three independently of dimension.

##### Cox-de Boor recursion formula

↑ **Parent:** [B-spline](#b-spline)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cox-de_Boor_recursion_formula)

The Cox-de Boor formula recursively expresses an order-$k$ B-spline using two adjacent order-$(k-1)$ B-splines.

##### Marsden identity

↑ **Parent:** [B-spline](#b-spline)

The Marsden identity expands $(x-t)^{k-1}$ in a B-spline basis with knot-polynomial coefficients.

###### Monomial B-spline coefficients

↑ **Parent:** [Marsden identity](#marsden-identity)

For order $k$ [B-splines](#b-spline), comparison of coefficients in the [Marsden identity](#marsden-identity) gives

$$
t^m=\sum_i\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}}N_i(t),\qquad0\leq m\leq k-1,
$$

on the basic knot interval. Here $e_m$ is the [elementary symmetric polynomial](polynomial.md#elementary-symmetric-polynomial), with $e_0=1$. The $m=0$ case is partition of unity; the $m=1$ coefficients are the [Greville abscissae](#greville-abscissa).

###### Greville abscissa

↑ **Parent:** [Monomial B-spline coefficients](#monomial-b-spline-coefficients)

For an order-$k$ [B-spline](#b-spline) with $k\geq2$, its Greville abscissa is the arithmetic mean of its $k-1$ interior knots. These are precisely the coefficients reproducing the linear function in the [monomial B-spline coefficients](#monomial-b-spline-coefficients) formula. The irregular plural is Greville abscissae.

###### Linear precision at Greville abscissae

↑ **Parent:** [Greville abscissa](#greville-abscissa)

For an open clamped [spline knot sequence](#spline-knot-sequence) and degree $d\ge1$, the [Greville abscissae](#greville-abscissa) $\xi_i=d^{-1}\sum_{r=1}^dt_{i+r}$ reproduce the parameter. The [B-spline differentiation formula](#b-spline-differentiation-formula) gives derivative coefficients $d(\xi_i-\xi_{i-1})/(t_{i+d}-t_i)=1$. Their lower-degree [partition of unity](differential-geometry.md#partition-of-unity) makes the derivative of the weighted sum equal to one. The left endpoint value is the left parameter endpoint, fixing the integration constant to zero. This proves [linear precision](numerical-analysis.md#linear-precision-of-a-geometric-basis) even with unequal knot intervals.

###### Marsden dual functional

↑ **Parent:** [Marsden identity](#marsden-identity)

The Marsden dual functionals extract coefficients in a [B-spline](#b-spline) expansion. If $\psi_i$ is the knot polynomial in the [Marsden identity](#marsden-identity), then on polynomials of degree at most $k-1$ one such functional is

$$
\lambda_i(p)=\frac1{(k-1)!}\sum_{j=0}^{k-1}(-1)^j\psi_i^{(k-1-j)}(x)p^{(j)}(x),
$$

and the right-hand side is independent of $x$.

<h6 id="de-boor-fix-spline-coefficient-functional">De Boor–Fix spline coefficient functional</h6>

↑ **Parent:** [Marsden dual functional](#marsden-dual-functional)

This [linear functional](linear-algebra.md#linear-functional) extracts one [coefficient](vector-space.md#coefficient) of a [B-spline](#b-spline) expansion using local [polynomial](polynomial.md) data. With $\psi_i(x)=\prod_{\ell=1}^{k-1}(x-t_{i+\ell})/(k-1)!$ and a point $\xi$ inside a knot cell in the [support](function.md#support), it is $\sum_{r=0}^{k-1}(-1)^rs^{(r)}(\xi)\psi_i^{(k-1-r)}(\xi)$. The local [polynomial](polynomial.md) identity for the [Marsden dual functional](#marsden-dual-functional) gives the desired [coefficient](vector-space.md#coefficient). Its bounded restriction to the local [spline](#spline-mathematics) space can be extended to continuous data on $[t_i,t_{i+k}]$ by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem), with the same bound. Such extensions supply [spline quasi-interpolation](#spline-quasi-interpolation) [coefficients](vector-space.md#coefficient) without requiring [derivatives](calculus.md#derivative) of the data.

###### Normalized Marsden dual functional

↑ **Parent:** [Marsden dual functional](#marsden-dual-functional)

When the knot polynomial is normalized as $\psi_i(x)=\prod_{\ell=1}^{k-1}(x-t_{i+\ell})/(k-1)!$, the displayed formula has no additional factorial prefactor. Applied to [Marsden's identity](#marsden-identity), it extracts the coefficient of the corresponding [B-spline](#b-spline) in any polynomial of degree at most $k-1$. Differentiating the finite sum makes adjacent terms cancel, proving independence of $x$. For linear polynomials the coefficient is their value at the [Greville abscissa](#greville-abscissa).

##### B-spline collocation matrix

↑ **Parent:** [B-spline](#b-spline)

For B-splines $N_j$ and interpolation sites $x_i$, the B-spline collocation matrix is $A_{ij}=N_j(x_i)$. Its invertibility is the existence-and-uniqueness condition for interpolation in that B-spline basis.

###### Total nonnegativity of B-spline collocation matrices

↑ **Parent:** [B-spline collocation matrix](#b-spline-collocation-matrix)

For increasing sites and an ordered nonnegative normalized [B-spline](#b-spline) basis, the [matrix](vector-space.md#matrix) $A_{ij}=N_j(x_i)$ is a [totally nonnegative matrix](vector-space.md#total-nonnegativity-of-a-matrix). One way to see the minors' signs is [knot insertion](#knot-insertion). Each inserted knot changes coefficients by $b_j=\alpha_j a_j+(1-\alpha_j)a_{j-1}$ with $0\leq\alpha_j\leq1$, using the standard constant endpoint pieces. This is a nonnegative rectangular bidiagonal map, whose minors are nonnegative. Products preserve that property by the [Cauchy–Binet formula](linear-algebra.md#cauchy-binet-formula). Insert each site to full knot multiplicity; a suitable refined coefficient is then the value $s(x_i)$. Thus collocation is an ordered row submatrix of the refinement map, and has nonnegative minors. The strict support conditions $t_i<x_i<t_{i+k}$ give invertibility by the [Schoenberg–Whitney theorem](#schoenberg-whitney-theorem); its inverse has the [checkerboard inverse of a totally nonnegative matrix](vector-space.md#checkerboard-inverse-of-a-totally-nonnegative-matrix) sign pattern.

<h6 id="schoenberg-whitney-theorem">Schoenberg–Whitney theorem</h6>

↑ **Parent:** [B-spline collocation matrix](#b-spline-collocation-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schoenberg–Whitney_theorem)

For increasing interpolation sites $x_i$ and an order-$k$ B-spline basis with knots $t_i$, the [B-spline collocation matrix](#b-spline-collocation-matrix) is invertible exactly when

$$
t_i<x_i<t_{i+k}
$$

for every $i$, equivalently when $N_i(x_i)>0$ for every $i$.

##### Schoenberg spline operator

↑ **Parent:** [B-spline](#b-spline)

A Schoenberg spline operator is a positive quasi-interpolant $\sum_i f(\tau_i)N_i$ with each sample point inside the corresponding B-spline support.

###### Local-support error bound for a Schoenberg spline operator

↑ **Parent:** [Schoenberg spline operator](#schoenberg-spline-operator)

For nonnegative partition-normalized order-$k$ [B-splines](#b-spline), let $Vf(t)=\sum_i f(\tau_i)N_i(t)$ with each sample point inside $[t_i,t_{i+k}]$. If $N_i(t)$ is nonzero, both $t$ and $\tau_i$ lie in an interval of length at most $k|\Delta|$. Their function values differ by at most the [modulus of continuity](topological-analysis.md#modulus-of-continuity) at that length. Summing with nonnegative weights of total one proves the displayed bound. With fixed order and vanishing maximum knot gap, [uniform continuity](topological-analysis.md#uniform-continuity) gives [uniform convergence](real-analysis.md#uniform-convergence). The same argument works for bounded piecewise-continuous outputs if full interior knot multiplicities are allowed; their individual continuity should not then be asserted.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (9)

- [Integer-coefficient polynomial approximation](#integer-coefficient-polynomial-approximation)
- [Lattice approximation from two-point approximation](functional-analysis.md#lattice-approximation-from-two-point-approximation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-61.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#2f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#2f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-64.md#1/i/solution)
- [Polynomial approximation](#polynomial-approximation)
- [Positive linear operator on continuous functions](topological-vector-space.md#positive-linear-operator-on-continuous-functions)
