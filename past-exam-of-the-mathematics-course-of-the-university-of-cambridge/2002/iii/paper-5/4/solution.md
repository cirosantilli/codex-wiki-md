<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $p:\mathbb D\to D$ be a [universal covering map](../../../../../universal-cover.md). On a small evenly covered neighborhood in $D$, choose a local inverse $s$ of $p$ and set

$$
ds_D=\lambda_D(z)|dz|,\qquad
\lambda_D(z)=\frac{2|s'(z)|}{1-|s(z)|^2}.
$$

Any two such lifts differ by a [deck transformation](../../../../../deck-transformation.md) of the disc. Every [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md) preserves the disc density: apply the derivative [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) to the automorphism and its inverse to get equality. Hence the definition is independent of the local inverse. Uniqueness of the [universal cover](../../../../../universal-cover.md) up to a covering isomorphism gives independence of the chosen cover as well. This is the [Poincare metric on a Riemann surface](../../../../../poincare-metric-on-a-riemann-surface.md), normalized to curvature $-1$.

For a piecewise continuously differentiable path $\gamma$, define its length by $L_D(\gamma)=\int\lambda_D(\gamma)|\gamma'|$, and the distance by the infimum of lengths of joining paths. Path reversal and concatenation prove symmetry and the triangle inequality. The distance between distinct points is positive: choose a small closed Euclidean disc around one point not containing the other, on which the positive continuous density is bounded below by $c>0$. Every joining path must leave that disc and has length at least $c$ times its radius before doing so. Joining paths of finite length exist because a plane domain is path connected and the density is locally bounded. Thus this construction gives an actual [metric](../../../../../metric.md), not just a nonnegative path-length expression.

For the punctured [unit disc](../../../../../unit-disc.md), use $p(w)=e^{iw}$ from the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). The half-plane line element is $|dw|/\operatorname{Im}w$, while $|dz|=|z||dw|$ and $\operatorname{Im}w=\log(1/|z|)$. Consequently

$$
\boxed{ds_A=\frac{|dz|}{|z|\log(1/|z|)}.}
$$

The domain called an annulus in the paper has inner radius zero, so it is this punctured-disc metric, not the metric of an annulus with positive inner radius.

We now prove the [Great Picard theorem](../../../../../great-picard-theorem.md). In its holomorphic form, an [essential singularity](../../../../../essential-singularity.md) takes every complex value, with at most one exception, infinitely often in every punctured neighborhood. It suffices to prove that a [holomorphic function](../../../../../holomorphic-function.md) on a punctured disc omitting $0$ and $1$ extends meromorphically through the puncture: if two values occurred only finitely often, a smaller punctured disc would omit both, and an affine change of target would reduce them to $0,1$.

Use the [universal covering by the modular lambda function](../../../../../universal-covering-by-the-modular-lambda-function.md) $\lambda:\mathbb H\to Y=\mathbb C\setminus\{0,1\}$, whose construction is given in the following solution. Its [deck transformation group](../../../../../deck-transformation-group.md) is the projective level-two [principal congruence subgroup](../../../../../principal-congruence-subgroup.md) $\Gamma(2)$. Rescale the source punctured disc to unit radius. Lift $f(e^{2\pi iw})$ to a [holomorphic function](../../../../../holomorphic-function.md) $L:\mathbb H\to\mathbb H$. Uniqueness of lifts gives

$$
L(w+1)=T L(w)
$$

for a fixed [deck transformation](../../../../../deck-transformation.md) $T\in\Gamma(2)$. The [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) gives

$$
\rho_{\mathbb H}(L(w),T L(w))
\leq\rho_{\mathbb H}(w,w+1)
=2\operatorname{arsinh}\frac1{2\operatorname{Im}w}\longrightarrow0
$$

as $\operatorname{Im}w\to\infty$. A nonidentity deck transformation has no interior fixed point, so it is either a [hyperbolic Möbius transformation](../../../../../hyperbolic-element-of-psl2-r.md) or a [parabolic Möbius transformation](../../../../../parabolic-element-of-psl2-r.md). The hyperbolic case is conjugate to a dilation $w\mapsto aw$ with $a>0$, $a
eq1$. Since $|d\log\operatorname{Im}w|\leq ds_{\mathbb H}$, its displacement is at least $|\log a|>0$, contradicting this inequality.

If $T$ is the identity, compose $L$ with the [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md). Its periodicity lets the resulting bounded function descend to the punctured disc and extend by the [Riemann removable singularity theorem](../../../../../riemann-removable-singularity-theorem.md). A nonconstant extension takes its central value inside the disc by the [maximum modulus principle](../../../../../maximum-modulus-principle.md). The covering map then gives an extension of $f$; a constant lift gives a constant $f$.

In the parabolic case, its fixed point is a rational [modular cusp](../../../../../cusp-of-a-modular-group.md). Indeed, a parabolic integral matrix of trace $\pm2$ has a rational eigenvector for its repeated eigenvalue. Conjugate by an element of the [modular group](../../../../../modular-group.md) sending this cusp to infinity. The level-two subgroup is normal, so the conjugated transformation is $\zeta\mapsto\zeta+2n$ for a nonzero integer $n$. The conjugated lift $P$ consequently satisfies

$$
P(w+1)=P(w)+2n,\qquad\operatorname{Im}P(w)>0.
$$

The modular transformations permute the three target cusp values $0,1,\infty$, as seen from the lambda transformation formulas below. It is therefore enough to examine $\lambda(P(w))$.

To fix the sign of $n$, the function $\operatorname{Im}P$ is periodic in the real direction. Its mean $M(y)=\int_0^1\operatorname{Im}P(x+iy)\,dx$ satisfies $M'(y)=2n$ by the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) and the increment of $\operatorname{Re}P$. Positivity for all $y>0$ forces $n>0$. The function

$$
Q(e^{2\pi iw})=e^{\pi iP(w)}
$$

is well-defined, nonvanishing and bounded by one on the punctured disc, so it extends holomorphically to zero. Its [winding number](../../../../../winding-number.md) along a circle around the puncture is $n$, because a unit increment in $w$ increases $\pi iP$ by $2\pi in$. The [argument principle](../../../../../argument-principle.md) therefore shows that $Q$ has a zero of order $n$ at the origin.

At the infinite cusp, the [modular lambda function](../../../../../modular-lambda-function.md) has the convergent expansion $\lambda(\zeta)=16q+O(q^2)$ in $q=e^{\pi i\zeta}$. Thus $\lambda(P(w))=16Q(z)+O(Q(z)^2)$ extends and tends to zero. Undoing the target permutation gives a removable singularity or a pole for $f$. In every case the puncture is not essential, which proves the holomorphic [Great Picard theorem](../../../../../great-picard-theorem.md). For a meromorphic function with an essential singularity, if three spherical values occurred only finitely often, a [Möbius transformation](../../../../../mobius-transformation.md) would make the omitted values $0,1,\infty$. The same proof applies because omission of infinity makes the transformed function holomorphic. Hence the meromorphic version has at most two exceptional spherical values.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
