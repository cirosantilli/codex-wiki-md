<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Define the [autoregressive polynomial](../../../../../autoregressive-polynomial.md) $\Phi(z)=1-\sum_{k=1}^p\phi_kz^k$ and the [moving-average polynomial](../../../../../moving-average-polynomial.md) $\Theta(z)=1+\sum_{k=1}^q\theta_kz^k$. The standard [causality and invertibility root criteria for an ARMA model](../../../../../causality-and-invertibility-root-criteria-for-an-arma-model.md) are

$$
\boxed{\Phi(z)\ne0\text{ and }\Theta(z)\ne0\quad\text{for every }|z|\leq1.}
$$

In the usual minimal [autoregressive moving-average model](../../../../../autoregressive-moving-average-model.md), the two polynomials have no common roots. Under that convention, these are the necessary and sufficient root conditions for a causal and invertible representation with the given noise. Without minimality they remain sufficient; shared factors must be considered before claiming necessity.

To see why the conditions work, both ratios $C(z)=\Theta(z)/\Phi(z)$ and $D(z)=\Phi(z)/\Theta(z)$ are analytic on a disc of radius greater than one. Their [power series](../../../../../power-series.md) coefficients therefore decay geometrically and are absolutely summable. The [backshift operator](../../../../../backshift-operator.md) $BX_t=X_{t-1}$ then gives a well-defined mean-square convergent [causal time-series representation](../../../../../causal-time-series-representation.md)

$$
X_t=C(B)\epsilon_t=\sum_{j\geq0}c_j\epsilon_{t-j}.
$$

Filtering [white noise](../../../../../white-noise.md) by these fixed coefficients gives a [weakly stationary process](../../../../../weakly-stationary-process.md). The identity $\Phi(B)C(B)=\Theta(B)$ verifies the original equation. Multiplication by the absolutely summable inverse of $\Phi(B)$ also shows uniqueness among finite-variance stationary solutions. Similarly $D(B)X_t=\epsilon_t$ gives the [invertible time-series representation](../../../../../invertible-time-series-representation.md).

Comparing coefficients in $\Phi(z)C(z)=\Theta(z)$ derives the first of the [ARMA coefficient recursions](../../../../../arma-coefficient-recursions.md):

$$
\boxed{c_j=\theta_j+\sum_{k=1}^p\phi_kc_{j-k}\quad(j\geq0).}
$$

Here $c_j=0$ for negative $j$, $\theta_0=1$, and $\theta_j=0$ for $j>q$, so in particular $c_0=1$. For the inverse filter, compare coefficients in $\Theta(z)D(z)=\Phi(z)$. With $a_0=1$, $a_j=-\phi_j$ for $1\leq j\leq p$, $a_j=0$ for $j>p$, and $d_j=0$ for negative indices, this gives

$$
\boxed{d_j=a_j-\sum_{k=1}^q\theta_kd_{j-k}\quad(j\geq0),\qquad d_0=1.}
$$

The minus sign in the inverse recursion comes from moving the nonconstant moving-average terms to the other side.

For the first-order model, the standard uncancelled conditions are $|\phi|<1$ and $|\theta|<1$. The geometric [power series](../../../../../power-series.md) expansions give

$$
\frac{1+\theta z}{1-\phi z}=1+(\phi+\theta)\sum_{j\geq1}\phi^{j-1}z^j,\qquad\frac{1-\phi z}{1+\theta z}=1-(\phi+\theta)\sum_{j\geq1}(-\theta)^{j-1}z^j.
$$

Thus the [ARMA(1,1) causal and inverse coefficients](../../../../../arma-1-1-causal-and-inverse-coefficients.md) are

$$
\boxed{c_0=d_0=1,\qquad c_j=(\phi+\theta)\phi^{j-1},\qquad d_j=-(\phi+\theta)(-\theta)^{j-1}\quad(j\geq1).}
$$

At $j=1$ these give $c_1=\phi+\theta$ and $d_1=-(\phi+\theta)$, including zero-valued parameters without any negative powers. If $\theta=-\phi$, the filtered process reduces to $X_t=\epsilon_t$ and all later coefficients vanish. This [common factor cancellation in an ARMA model](../../../../../common-factor-cancellation-in-an-arma-model.md) is why the root inequalities should not be advertised as necessary for every nonminimal parameterization. The stated inequalities still ensure uniqueness for the original equation as well as the desired causal and invertible filters.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
