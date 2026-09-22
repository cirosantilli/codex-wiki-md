<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

State the characteristic convention explicitly: for real $\alpha,\beta$, define the [theta function with characteristics](../../../../../../theta-function-with-characteristics.md) by

$$
\boxed{\theta[\alpha,\beta](z,\tau)=\sum_{n\in\mathbb Z}\exp\bigl(\pi i(n+\alpha)^2\tau+2\pi i(n+\alpha)(z+\beta)\bigr),\qquad\operatorname{Im}\tau>0.}
$$

Binary subscripts $\vartheta_{ab}$ often denote this function with $(\alpha,\beta)=(a/2,b/2)$, $a,b\in\{0,1\}$. On compact subsets of the $(z,\tau)$ domain, a summand and any derivative are bounded by a polynomial in $|n|$ times $e^{-c n^2+C|n|}$. Normal convergence therefore gives an entire function of $z$, holomorphic dependence on $\tau$, and legitimate termwise differentiation. In particular the [heat equation for theta functions with characteristics](../../../../../../heat-equation-for-theta-functions-with-characteristics.md) is

$$
\boxed{4\pi i\,\partial_\tau\theta=\partial_z^2\theta.}
$$

Characteristics are defined modulo integers with a phase: $\theta[\alpha+1,\beta]=\theta[\alpha,\beta]$ and $\theta[\alpha,\beta+1]=e^{2\pi i\alpha}\theta[\alpha,\beta]$. Shifting the summation index proves the spatial quasi-periods

$$
\theta(z+1)=e^{2\pi i\alpha}\theta(z),\qquad
\theta(z+\tau)=e^{-\pi i\tau-2\pi i(z+\beta)}\theta(z).
$$

These multipliers describe a degree-one [line bundle](../../../../../../line-bundle.md) on the [complex torus](../../../../../../complex-torus.md) with periods $1,\tau$, rather than an ordinary elliptic function. The logarithmic derivative is unchanged under one and decreases by $2\pi i$ under tau. Pairing opposite sides of a fundamental cell therefore makes its contour integral $2\pi i$. The [argument principle](../../../../../../argument-principle.md) counts exactly one zero in a cell, with multiplicity.

The characteristic function is a translate of the unshifted theta function:

$$
\theta[\alpha,\beta](z,\tau)=e^{\pi i\alpha^2\tau+2\pi i\alpha(z+\beta)}\theta[0,0](z+\alpha\tau+\beta,\tau).
$$

At $z=(1+\tau)/2$, the unshifted series cancels in pairs $n,-n-1$. Hence the [zeros of theta functions with characteristics](../../../../../../zeros-of-theta-functions-with-characteristics.md) occur exactly and simply at

$$
\boxed{z=(1/2-\alpha)\tau+(1/2-\beta)\pmod{\mathbb Z+\mathbb Z\tau}.}
$$

Reindexing also gives $\theta[\alpha,\beta](-z)=\theta[-\alpha,-\beta](z)$. For half-integer characteristics the parity is $e^{4\pi i\alpha\beta}$, so only $(1/2,1/2)$ is odd and vanishes at zero; the other three theta constants are nonzero.

The [modular transformations of theta characteristics](../../../../../../modular-transformations-of-theta-characteristics.md) are obtained from Gaussian [Poisson summation](../../../../../../poisson-summation-formula.md) and elementary phase rearrangement. With the holomorphic branch of $\sqrt{-i\tau}$ positive at $\tau=i$,

$$
\boxed{\theta[\alpha,\beta](z/\tau,-1/\tau)=\sqrt{-i\tau}\,e^{\pi iz^2/\tau+2\pi i\alpha\beta}\theta[\beta,-\alpha](z,\tau),}
$$



$$
\boxed{\theta[\alpha,\beta](z,\tau+1)=e^{-\pi i\alpha(\alpha-1)}\theta[\alpha,\beta+\alpha-1/2](z,\tau).}
$$

For the first formula, apply Poisson summation to $F(t)=e^{\pi i\tau(t+\alpha)^2+2\pi i(t+\alpha)(z+\beta)}$. Completing the square in its Fourier transform gives

$$
\widehat F(m)=(-i\tau)^{-1/2}e^{2\pi im\alpha-\pi i(z+\beta-m)^2/\tau}.
$$

Rearranging $\sum_nF(n)=\sum_m\widehat F(m)$ proves the stated inversion law. For translation by one, use $e^{\pi in^2}=e^{\pi in}$ in the defining series; the remaining characteristic phase is precisely the displayed factor.

Write $Q=e^{\pi i\tau}$, so the modular-form variable of Question 1 is $q=Q^2$, and put $\Theta_2=\theta[1/2,0](0,\tau)$, $\Theta_3=\theta[0,0](0,\tau)$ and $\Theta_4=\theta[0,1/2](0,\tau)$. Inversion interchanges $\Theta_2,\Theta_4$ and fixes $\Theta_3$, each with factor $\sqrt{-i\tau}$. Translation interchanges $\Theta_3,\Theta_4$ and multiplies $\Theta_2$ by $e^{\pi i/4}$. The [Jacobi triple product](../../../../../../jacobi-triple-product.md) gives

$$
\Theta_2=2Q^{1/4}\prod_{m\geq1}(1-Q^{2m})(1+Q^{2m})^2,
$$



$$
\Theta_3=\prod_{m\geq1}(1-Q^{2m})(1+Q^{2m-1})^2,\qquad
\Theta_4=\prod_{m\geq1}(1-Q^{2m})(1-Q^{2m-1})^2.
$$

It also gives the conventional odd theta function $\theta_1=-\theta[1/2,1/2]$ its product $2Q^{1/4}\sin(\pi z)\prod_{m\geq1}(1-Q^{2m})(1-2Q^{2m}\cos(2\pi z)+Q^{4m})$. Differentiate at zero and multiply the three even products to obtain the [Jacobi derivative formula](../../../../../../jacobi-derivative-formula.md)

$$
\boxed{\theta_1'(0,\tau)=\pi\Theta_2\Theta_3\Theta_4.}
$$

In the constant-product simplification, $\prod_m(1+Q^{2m})(1-Q^{4m-2})=1$, by separating even and odd positive exponents. The products prove nonvanishing of all three even constants as well.

The [Jacobi abstruse identity](../../../../../../jacobi-abstruse-identity.md) can be proved directly, without assuming it from the products. Splitting pairs of summation indices according to whether their sum and difference are even or odd gives

$$
\Theta_3(\tau)^2=\Theta_3(2\tau)^2+\Theta_2(2\tau)^2,\qquad
\Theta_4(\tau)^2=\Theta_3(2\tau)^2-\Theta_2(2\tau)^2,
$$



$$
\Theta_2(\tau)^2=2\Theta_2(2\tau)\Theta_3(2\tau).
$$

For example, $u=(n+m)/2,v=(n-m)/2$ are either both integers or both half-integers, and $n^2+m^2=2u^2+2v^2$. The alternating signs give the second identity; shifting both original indices by one half gives the third. Squaring the first two and subtracting then proves **$\Theta_3^4=\Theta_2^4+\Theta_4^4$**.

These identities connect theta theory to [modular forms](../../../../../../modular-form.md) and [elliptic curves](../../../../../../elliptic-curve.md). The fourth powers are weight-two forms on the principal level-two [congruence subgroup](../../../../../../congruence-subgroup.md). The [modular lambda function](../../../../../../modular-lambda-function.md) $\lambda=\Theta_2^4/\Theta_3^4$ obeys $\lambda(-1/\tau)=1-\lambda(\tau)$ and $\lambda(\tau+1)=\lambda(\tau)/(\lambda(\tau)-1)$; the characteristic permutation kernel is $\Gamma(2)$. It parametrizes an elliptic curve with its ordered two-torsion in Legendre form $y^2=x(x-1)(x-\lambda)$. The corresponding [Klein j-invariant](../../../../../../klein-j-invariant.md) is $256(1-\lambda+\lambda^2)^3/[\lambda^2(1-\lambda)^2]$. Finally the same products give

$$
\boxed{\Delta(\tau)=2^{-8}(\Theta_2\Theta_3\Theta_4)^8.}
$$

Indeed $\Theta_2\Theta_3\Theta_4=2Q^{1/4}\prod_m(1-Q^{2m})^3$, whose eighth power divided by $256$ is $q\prod_m(1-q^m)^{24}$. This recovers the normalized modular discriminant of Question 1 and displays the bridge between Gaussian theta sums and the lattice discriminant of Question 2.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
