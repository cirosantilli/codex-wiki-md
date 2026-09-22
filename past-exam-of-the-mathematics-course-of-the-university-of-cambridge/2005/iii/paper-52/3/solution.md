<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Set $\epsilon=4-n$ and $a=3/(16\pi^2)=-C$. The kinetic term gives the scalar [mass dimension](../../../../../mass-dimension.md) $(n-2)/2$, so the quartic [bare coupling](../../../../../bare-coupling.md) has [mass dimension](../../../../../mass-dimension.md) $4-n=\epsilon$. A dimensionless [renormalized coupling](../../../../../renormalized-coupling.md) therefore comes with the factor $\mu^\epsilon=(\mu^2)^{2-n/2}$.

The order-$\lambda_R^2$ proper four-point corrections are precisely the three $s,t,u$ [bubble diagrams](../../../../../bubble-diagram.md) in the diagram plate, with external partitions $(12|34),(13|24),(14|23)$. Each carries a [symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) one half. Its two-propagator integral has logarithmic ultraviolet divergence in four dimensions, represented in [dimensional regularization](../../../../../dimensional-regularization.md) by a simple pole at $n=4$. That pole's residue is independent of external momenta, so a local quartic counterterm cancels it. The three channels add, rather than describing three separate couplings. The two-point tadpole has no momentum dependence, so it does not supply a one-loop field-normalization correction to the four-point coupling. The first momentum-dependent field correction contributes to this relation only at higher order.

With the supplied residue $C=-a$, the subtraction relation consequently reads

$$
\lambda_0=\mu^\epsilon\left(\lambda_R+\frac{a}{\epsilon}\lambda_R^2+O(\lambda_R^3)\right).
$$

A possible scheme-dependent finite subtraction does not change the displayed four-dimensional one-loop coefficient. Keep the regulator and [bare coupling](../../../../../bare-coupling.md) fixed while varying the [renormalization scale](../../../../../renormalization-scale.md), and define $\beta(\lambda_R)=d\lambda_R/d\log\mu$. Differentiation gives

$$
0=\epsilon\left(\lambda_R+\frac a\epsilon\lambda_R^2\right)
+\beta(\lambda_R)\left(1+\frac{2a}{\epsilon}\lambda_R\right)+O(\lambda_R^3).
$$

To retain all quadratic terms, put $\beta=-\epsilon\lambda_R+b\lambda_R^2+O(\lambda_R^3)$. The engineering term times the pole factor contributes $-2a\lambda_R^2$, and the remaining quadratic coefficient is $a-2a+b$. It vanishes only when $b=a$. Thus

$$
\boxed{\beta(\lambda_R)=-(4-n)\lambda_R+\frac{3}{16\pi^2}\lambda_R^2+O(\lambda_R^3).}
$$

Dropping the product of the engineering term and pole factor would give the wrong sign for the loop term.

At $n=4$, separation of the one-loop [renormalization-group flow](../../../../../renormalization-group-flow.md) gives

$$
\frac{d\lambda_R}{\lambda_R^2}=a\,d\log\mu,
\qquad
\frac1{\lambda_R(\mu)}=\frac1{\lambda_s}-a\log\frac\mu{\mu_s}.
$$

Therefore

$$
\boxed{\lambda_R(\mu)=\frac{\lambda_s}{1-\dfrac{3\lambda_s}{16\pi^2}\log(\mu/\mu_s)}.}
$$

This is the solution of the truncated one-loop equation, not an exact all-orders running law. It applies while the coupling remains sufficiently weak; its [Landau pole](../../../../../landau-pole.md) is at $\mu=\mu_s\exp[16\pi^2/(3\lambda_s)]$ for $\lambda_s>0$.

A [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md) has $\beta(\lambda^*)=0$. For $t=\log(\mu/\mu_s)$ and a small perturbation $\delta=\lambda_R-\lambda^*$, linearization gives

$$
\frac{d\delta}{dt}=\beta'(\lambda^*)\delta+O(\delta^2),\qquad
\delta(t)\approx\delta(0)e^{\beta'(\lambda^*)t}.
$$

Thus $\beta'(\lambda^*)<0$ means attraction as $\mu\to\infty$, or ultraviolet stability; $\beta'(\lambda^*)>0$ means attraction as $\mu\to0$, or infrared stability. If the derivative vanishes, higher terms decide marginal stability. These statements concern the specified coupling direction; other couplings or the mass can be relevant even when this direction is stable.

For $\epsilon>0$, the quadratic [renormalization-group beta function](../../../../../beta-function-physics.md) has zeros $0$ and $\epsilon/a$. At the nonzero zero,

$$
\lambda^*=\frac{\epsilon}{a},\qquad
\beta'(\lambda^*)=-\epsilon+2a\frac\epsilon a=\epsilon>0.
$$

Consequently

$$
\boxed{\lambda^*=(4-n)\frac{16\pi^2}{3}\quad\text{is infrared stable in the quartic direction}.}
$$

This is the weak-coupling [Wilson-Fisher fixed point](../../../../../wilson-fisher-fixed-point.md), perturbatively controlled near four dimensions. Reaching its full critical limit also requires tuning the mass, the [thermal relevant direction at the Wilson-Fisher fixed point](../../../../../thermal-relevant-direction-at-the-wilson-fisher-fixed-point.md).

At $n=4$, this nonzero fixed point merges with the [Gaussian fixed point](../../../../../gaussian-fixed-point.md). Although the derivative at zero vanishes, $\beta=a\lambda_R^2>0$ for a positive weak coupling, so the running solution tends to zero logarithmically toward the infrared. **The four-dimensional critical long-distance limit is Gaussian: the quartic interaction is marginally irrelevant, rather than flowing to a nonzero weakly interacting infrared fixed point.** This is the [Gaussian infrared limit of positive four-dimensional quartic coupling](../../../../../gaussian-infrared-limit-of-positive-four-dimensional-quartic-coupling.md). It is not ultraviolet [asymptotic freedom](../../../../../asymptotic-freedom.md); the positive coupling grows in the ultraviolet. Nor does it say a massive theory has no interactions at finite energy: the critical or massless scaling regime is the one described by this limiting flow. Extrapolating the one-loop law to arbitrarily high cutoff at fixed positive low-energy coupling encounters its Landau pole; avoiding that pole as the cutoff is removed forces the perturbative coupling toward zero. This motivates the usual triviality conclusion, but the one-loop calculation alone is not a nonperturbative theorem excluding all possible strongly coupled ultraviolet completions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
