<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The objective approximates the logarithm of the [product-form stationary distribution of a loss network](../../../../../../product-form-stationary-distribution-of-a-loss-network.md). To make the approximation precise, multiply arrival rates and capacities by $N$ and write $x=n/N$. The [Stirling formula](../../../../../../stirling-formula.md) gives, uniformly on the feasible compact set,

$$
\log\prod_r\frac{(N\nu_r)^{n_r}}{n_r!}=N H_\nu(n/N)+O(\log N),\qquad H_\nu(x)=\sum_r\bigl[x_r\log\nu_r+x_r-x_r\log x_r\bigr],
$$

with $0\log0=0$. The feasible set is $K=\{x\geq0:Ax\leq C\}$. Positive capacities and a nonempty route for each class make $K$ compact with a strictly positive feasible point. Since $H_\nu$ is a [strictly concave function](../../../../../../strictly-concave-function.md), its maximizer $x^*$ is unique; its infinite inward derivative at $x_r=0$ makes every component positive.

The [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) give nonnegative link [Lagrange multipliers](../../../../../../lagrange-multiplier.md) $z_j$ satisfying

$$
\boxed{x_r^*=\nu_r e^{-(A^Tz)_r},\qquad z_j\bigl(C_j-(Ax^*)_j\bigr)=0.}
$$

For any neighborhood of $x^*$, continuity and uniqueness give a strictly positive objective gap outside it. There are only polynomially many feasible lattice states, while their weights differ exponentially in $N$. The feasible point $\lfloor Nx^*\rfloor$ has objective tending to $H_\nu(x^*)$. It follows that the stationary law concentrates at $x^*$ on the scale $n/N$; in particular,

$$
\boxed{\frac nN\longrightarrow x^*\text{ in probability},\qquad \mathbb E[n]=Nx^*+o(N).}
$$

Thus NETWORK predicts the dominant occupancy and mean occupancy in a large [loss network](../../../../../../loss-network.md). For unscaled inputs it gives a continuous approximation to the modal integer state.

It also gives an exact useful change of variables. Substituting $\nu_r=x_r^*e^{(A^Tz)_r}$ into the equilibrium weights yields

$$
\pi_N(n)\propto\mathbf1_{\{An\leq NC\}}e^{z^T(An-NC)}\prod_r\Pr\{\operatorname{Poisson}(Nx_r^*)=n_r\}.
$$

This is [Poisson exponential tilting for a loss network](../../../../../../poisson-exponential-tilting-for-a-loss-network.md): independent [Poisson random variables](../../../../../../poisson-distribution.md) centered at the predicted occupancies, restricted to the feasible region and penalized for slack in positively priced resources. It explains why an unconstrained [Gaussian approximation](../../../../../../normal-approximation.md) should not automatically be applied at a saturated capacity boundary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
