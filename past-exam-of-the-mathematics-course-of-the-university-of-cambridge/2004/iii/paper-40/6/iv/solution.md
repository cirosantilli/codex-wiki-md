<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For these counts, start with any $0<\theta^{(0)}<1$. The conditional missing count from part (ii) has [mean](../../../../../../expected-value.md)

$$
z_r=\mathbb E[Z\mid\mathbf x,\theta^{(r)}]
=\frac{340\theta^{(r)}}{7+4\theta^{(r)}}.
$$

The E-step objective is

$$
Q(\theta\mid\theta^{(r)})=(5+z_r)\log\theta+30\log(1-\theta)+\mathrm{constant}.
$$

Its strictly [concave](../../../../../../concave-function.md) M-step is explicit:

$$
\boxed{\theta^{(r+1)}=\frac{5+z_r}{35+z_r},\qquad
z_r=\frac{340\theta^{(r)}}{7+4\theta^{(r)}}.}
$$

Equivalently, the update map is $F(\theta)=(35+360\theta)/(245+480\theta)$. Its fixed-point equation is

$$
480\theta^2-115\theta-35=0.
$$

The unique root in $(0,1)$ is the [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\theta=\frac{115+\sqrt{80425}}{960}\approx0.4152.}
$$

For example, starting at $1/2$ gives $0.443299$, then approximately $0.425065$, and subsequent iterates approach the displayed root. Convergence is also transparent without relying only on the general EM theorem: $F$ is increasing and

$$
F(\theta)-\theta=\frac{35+115\theta-480\theta^2}{245+480\theta}.
$$

This is positive below the feasible fixed point and negative above it. Monotonicity of $F$ prevents crossing that fixed point, so the iterates converge monotonically toward it from either side. The original [log-likelihood](../../../../../../log-likelihood.md) is strictly [concave](../../../../../../concave-function.md) and diverges to minus infinity at both endpoints, establishing that the fixed point is the unique global maximum.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
