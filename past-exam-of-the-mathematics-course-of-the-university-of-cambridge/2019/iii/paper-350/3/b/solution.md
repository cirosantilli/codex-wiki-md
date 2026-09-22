<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The notation $P_0=\mathcal N(0,I)$ denotes generalized [Gaussian white noise](../../../../../../gaussian-white-noise.md) over $H=L^2(\mathbb R^2)$, not a [Gaussian measure](../../../../../../gaussian-measure.md) supported on $H$: the identity is not a [trace-class operator](../../../../../../trace-class-operator.md) there. For example, realize the observation on a suitable space of [tempered distributions](../../../../../../tempered-distribution.md). Its [Cameron-Martin space of a Gaussian measure](../../../../../../cameron-martin-space-of-a-gaussian-measure.md) is $H$. For deterministic $h\in H$, the stochastic pairing $W_m(h)$ has [normal distribution](../../../../../../normal-distribution.md) $\mathcal N(0,\|h\|_H^2)$ under $P_0$ and is the [isonormal Gaussian process](../../../../../../isonormal-gaussian-process.md) indexed by $H$.

Interpret the stated maps between [Sobolev spaces](../../../../../../sobolev-space-split.md) as bounded [linear operators](../../../../../../linear-operator.md), as usual. In particular $K:H\to H^2(\mathbb R^2)\subset H$ is bounded, so its [adjoint operator](../../../../../../adjoint-operator.md) $K^*$ is bounded on $H$. Hence $A=K^*K$ maps $H$ into $H$, which is the property needed here. The stronger smoothing follows by [Sobolev duality](../../../../../../sobolev-duality.md): boundedness of $K:H^{-4}\to H^{-2}$ gives $K^*:H^2\to H^4$, and therefore $A:H\to H^4\subset H$. As $\Pi(H)=1$, the shift $Au$ belongs to the noise [Cameron-Martin space of a Gaussian measure](../../../../../../cameron-martin-space-of-a-gaussian-measure.md) for $\Pi$-almost every $u$.

The [white-noise likelihood for a square-integrable shift](../../../../../../white-noise-likelihood-for-a-square-integrable-shift.md), obtained from the [Cameron-Martin theorem for a Gaussian measure](../../../../../../cameron-martin-theorem-for-a-gaussian-measure.md) in its white-noise form, is

$$
L(u,m)=\frac{dP_u}{dP_0}(m)
=\exp\left(W_m(Au)-\tfrac12\|Au\|_H^2\right)
=e^{-\Phi(u;m)},\qquad
\Phi(u;m)=\tfrac12\|Au\|_H^2-W_m(Au).
$$

Here $P_u$ is the law of $Au+\eta$. In an [orthonormal basis](../../../../../../orthonormal-basis.md) $(e_j)$ of $H$, with white-noise coordinates $m_j$, the pairing under $P_0$ is

$$
W_m(Au)=\lim_{N\to\infty}\sum_{j=1}^Nm_j\langle Au,e_j\rangle_H.
$$

For fixed $u$ this has [mean-square convergence](../../../../../../convergence-in-l2.md) and converges [almost surely](../../../../../../almost-sure-convergence.md), since $\sum_j|\langle Au,e_j\rangle|^2=\|Au\|_H^2$. The stipulated joint measurability allows the likelihood to be used under $\nu_0(du,dm)=\Pi(du)P_0(dm)$. One must not replace this expression by a finite $\|m-Au\|_H^2$, because white noise is not $H$-valued. On the unbounded domain $\mathbb R^2$, membership of white noise in a global unweighted negative [Sobolev space](../../../../../../sobolev-space-split.md) must not be assumed either; the stochastic pairing avoids that issue.

Let $\nu(du,dm)=\Pi(du)P_u(dm)$ be the actual joint law. The shift formula gives $\nu\ll\nu_0$ with [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) $L$. Define

$$
Z(m)=\int_HL(u,m)\,\Pi(du).
$$

For each fixed admissible $u$, the [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) gives

$$
\int L(u,m)\,P_0(dm)=
e^{-\|Au\|_H^2/2}\mathbb E^{P_0}e^{W_m(Au)}=1.
$$

By [Tonelli theorem](../../../../../../tonelli-theorem.md), $\int Z(m)P_0(dm)=1$, so $Z(m)<\infty$ for $P_0$-almost every $m$. The likelihood is finite and strictly positive for $\nu_0$-almost every $(u,m)$; [Fubini's theorem](../../../../../../fubini-s-theorem.md) then gives $Z(m)>0$ for $P_0$-almost every $m$. The marginal observation law is $Z(m)P_0(dm)$ and is an [equivalent probability measure](../../../../../../equivalent-probability-measure.md) to $P_0$.

The [Bayes formula for a dominated observation model](../../../../../../bayes-formula-for-a-dominated-observation-model.md) therefore defines

$$
\boxed{\frac{d\Pi^m}{d\Pi}(u)=\frac1{Z(m)}
\exp\left(W_m(Au)-\tfrac12\|Au\|_{L^2}^2\right).}
$$

To verify that it is the [conditional distribution](../../../../../../conditional-distribution.md), for measurable sets $B$ of unknowns and $C$ of data,

$$
\int_C\Pi^m(B)Z(m)\,P_0(dm)
=\int_{B\times C}L(u,m)\,\nu_0(du,dm)=\nu(B\times C).
$$

Thus the [posterior distribution](../../../../../../bayesian-posterior.md) is well defined for almost every observation under the actual data law. This is the appropriate almost-everywhere assertion supplied by [Bayes' theorem](../../../../../../bayes-theorem.md); the stated assumptions do not prescribe a canonical posterior at every exceptional generalized datum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
