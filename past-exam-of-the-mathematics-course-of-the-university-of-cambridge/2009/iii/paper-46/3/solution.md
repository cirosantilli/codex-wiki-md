<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The Euclidean [dilaton](../../../../../dilaton.md) term is $S_\Phi=(4\pi)^{-1}\int\sqrt h\,\Phi(X)R^{(2)}$. A constant mode $\Phi_0$ therefore gives $S_\Phi=\Phi_0\chi$ by the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md). Setting the [string coupling](../../../../../string-coupling.md) to $g_s=e^{\Phi_0}$, an oriented closed worldsheet of genus $g$ has weight

$$
e^{-S_\Phi}=g_s^{-\chi}=g_s^{2g-2}.
$$

Each canonically normalized external closed-string vertex supplies a further factor $g_s$. Thus the connected $n$-point genus-$g$ contribution carries

$$
\boxed{g_s^{2g-2+n}.}
$$

This is the [string genus expansion](../../../../../string-genus-expansion.md). Four external strings on a sphere give $g_s^2$, as in the displayed tree amplitude.

Use the conventional complex-coordinate measure $d^2z=2\,d(\operatorname{Re}z)\,d(\operatorname{Im}z)$, with $\partial=(\partial_x-i\partial_y)/2$. The action then has the standard real-coordinate normalization $(4\pi\alpha')^{-1}\int(\nabla X)^2d^2x$. In these conventions the [free-boson worldsheet propagator](../../../../../free-boson-worldsheet-propagator.md) is

$$
\boxed{\langle X^\mu(z,\bar z)X^\nu(w,\bar w)\rangle
=-\frac{\alpha'}2\delta^{\mu\nu}\log|z-w|^2,}
$$

up to an additive infrared constant. Indeed the quadratic kernel after integration by parts is $-(\pi\alpha')^{-1}\partial\bar\partial$, and $\partial\bar\partial\log|z-w|^2=2\pi\delta^{(2)}(z-w)$ for this measure. Their product gives the required delta function. A simultaneous change of the coordinate-measure convention and action coefficient leaves this physical normalization unchanged.

Separate the constant mode $x_0$ of $X$. Its integral supplies $(2\pi)^D\delta^{(D)}(\sum_i p_i)$, so [four-momentum conservation](../../../../../four-momentum-conservation.md) is essential, even when that delta function is suppressed in the amplitude notation. Treat the exponential vertices as normal ordered: self-contractions are then absent. The [Gaussian functional integral](../../../../../gaussian-functional-integral.md) and [Wick theorem](../../../../../wick-s-theorem.md) give

$$
\left\langle\prod_{i=1}^4:e^{ip_i\cdot X(z_i)}:\right\rangle
\propto\delta^{(D)}\!\left(\sum_i p_i\right)
\exp\!\left(-\sum_{j<l}p_j\cdot p_l\,\langle X(z_j)X(z_l)\rangle\right)
=\delta^{(D)}\!\left(\sum_i p_i\right)\prod_{j<l}|z_j-z_l|^{\alpha'p_j\cdot p_l}.
$$

The oscillator determinant and normalization constants do not depend on the insertion positions. Substitution therefore gives the requested [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md) under the four insertion integrals, with the sphere's residual conformal-group volume divided out.

For the Möbius transformation $z'=(az+b)/(cz+d)$, the unit determinant condition gives

$$
z'_j-z'_l=\frac{z_j-z_l}{(cz_j+d)(cz_l+d)},\qquad
d^2z'_i=|cz_i+d|^{-4}d^2z_i.
$$

The distance-product factor attached to insertion $i$ is $|cz_i+d|^{-\alpha'\sum_{j\ne i}p_i\cdot p_j}$. Momentum conservation changes its exponent to $\alpha'p_i^2$. Thus the total factor at each insertion, including the measure, is

$$
|cz_i+d|^{\alpha'p_i^2-4}.
$$

On the [tachyon](../../../../../tachyon.md) mass shell $p_i^2=4/\alpha'$ it is one. This proves the [Möbius invariance of on-shell closed-string vertex integrals](../../../../../mobius-invariance-of-on-shell-closed-string-vertex-integrals.md). **The correlator is covariant; the correlator times all four measures is invariant.** This is the invariant integrand needed to quotient by the residual $SL(2,\mathbb C)$ transformations.

For the massless [Type II superstring theory](../../../../../type-ii-string-theory.md) amplitude, use $s=-(p_1+p_2)^2$ in Lorentzian target signature and $s+t+u=0$. At generic fixed $t$, the numerator factor $\Gamma(-\alpha's/4)$ has simple poles at

$$
\boxed{s=M_n^2=\frac{4n}{\alpha'},\qquad n=0,1,2,\ldots.}
$$

At these points $\Gamma(1+\alpha's/4)=\Gamma(1+n)=n!$ is finite and nonzero. The $t,u$ factors are also finite and nonzero for generic $t$, so the poles persist; isolated residue zeros at special kinematics do not remove the general mass level. Tree-level factorization interprets a pole at $s=M^2$ as exchange of a state of that mass. The [Type II gamma-factor mass poles](../../../../../type-ii-gamma-factor-mass-poles.md) therefore exhibit a massless level and an infinite tower of massive levels, with equally spaced squared masses $4/\alpha'$.

There is no negative-$s$ pole in this exchanged tower. In particular, at negative integer values of $\alpha's/4$ the reciprocal s-channel denominator can instead have zeros. This is consistent with the absence of the bosonic [tachyon](../../../../../tachyon.md) in the [Type II superstring mass spectrum](../../../../../type-ii-superstring-mass-spectrum.md). The factor alone does not determine degeneracies, spins or every possible uncoupled state; external polarizations and the rest of the amplitude control their residues.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
