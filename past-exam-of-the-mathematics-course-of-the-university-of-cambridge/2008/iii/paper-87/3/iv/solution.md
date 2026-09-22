<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The motivation for [Kolmogorov refined similarity hypothesis](../../../../../../kolmogorov-refined-similarity-hypothesis.md) is [internal intermittency](../../../../../../internal-intermittency.md): instantaneous energy dissipation is spatially uneven, so scaling every [velocity](../../../../../../velocity.md) increment by the global mean dissipation can mix regions of very different activity. Define the [coarse-grained energy dissipation](../../../../../../coarse-grained-energy-dissipation.md) over a region of size $r$ by

$$
\epsilon_r(\boldsymbol x)=\frac1{|B_r|}\int_{B_r(\boldsymbol x)}2\nu S_{ij}(\boldsymbol y)S_{ij}(\boldsymbol y)d^3y.
$$

Its mean is $\epsilon$ in homogeneous turbulence. The refined hypothesis asserts that, at high local Reynolds number and within the [inertial range](../../../../../../inertial-range.md), the normalized increment

$$
V_r=\frac{\Delta v}{(\epsilon_r r)^{1/3}}
$$

has universal conditional statistics independent of $\epsilon_r$ and of $r$. In particular, $\langle V_r^p\mid\epsilon_r\rangle=\beta_p$ for finite moments. Taking a conditional expectation and then averaging gives

$$
\boxed{\langle(\Delta v)^p\rangle
=\beta_pr^{p/3}\langle\epsilon_r^{p/3}\rangle.}
$$

Here $\epsilon_r$ is the paper's $\epsilon_{AV}(r)$. Signed odd moments need not have positive coefficients; the third-order forward-cascade coefficient is negative. The signed first moment is zero in homogeneous flow, so one does not assign it a nonzero scaling law. Absolute moments are often used when discussing general positive-order scaling exponents.

The refined hypothesis alone does not specify the distribution of $\epsilon_r$. Kolmogorov's 1962 estimate supplements it with a [lognormal intermittency model](../../../../../../lognormal-intermittency-model.md). Let $Y_r=\ln(\epsilon_r/\epsilon)$ be Gaussian with [variance](../../../../../../variance-split.md) $\sigma_r^2=\mu\ln(\ell/r)+\mathrm{constant}$. The condition $\langle\epsilon_r\rangle=\epsilon$ fixes its mean at $-\sigma_r^2/2$. The Gaussian exponential moment then gives, with $q=p/3$,

$$
\langle\epsilon_r^q\rangle=\epsilon^q
\exp\left(\frac{q(q-1)}2\sigma_r^2\right)
\propto\epsilon^q r^{-\mu q(q-1)/2}.
$$

Combining with the refined moment formula yields, for the nonzero moments described by that model,

$$
\boxed{\zeta_p=\frac p3-\frac\mu{18}p(p-3).}
$$

The intermittency parameter $\mu$ must be supplied by dissipation statistics; it is not determined by [dimensional analysis](../../../../../../dimensional-analysis.md). The formula preserves $\zeta_3=1$. Its extrapolation to arbitrarily high orders is not justified: the quadratic correction eventually predicts pathological exponents and is one limitation of the lognormal model, distinct from the refined hypothesis itself.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
