<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) says that every [holomorphic](../../../../../complex-differentiability-at-a-point.md) self-map $F$ of the [unit disc](../../../../../unit-disc.md) contracts [pseudohyperbolic distance](../../../../../pseudohyperbolic-distance.md) and therefore [hyperbolic distance](../../../../../hyperbolic-distance.md):

$$
\left|\frac{F(z)-F(w)}{1-\overline{F(w)}F(z)}\right|
\le\left|\frac{z-w}{1-\overline wz}\right|,\qquad
\rho(F(z),F(w))\le\rho(z,w).
$$

Its infinitesimal form is

$$
\boxed{\frac{|F'(w)|}{1-|F(w)|^2}\le\frac1{1-|w|^2}.}
$$

Equality for distinct points in the distance inequality, or at one point in the [derivative](../../../../../derivative.md) inequality, holds exactly when $F$ is a disc [Möbius transformation](../../../../../mobius-transformation.md).

For completeness, first prove the [Schwarz lemma](../../../../../schwarz-lemma.md). If $H:\mathbb D\to\mathbb D$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) and $H(0)=0$, the quotient $H(z)/z$ extends holomorphically at zero. On $|z|=r<1$ its modulus is at most $1/r$. The [maximum modulus principle](../../../../../maximum-modulus-principle.md), followed by $r\uparrow1$, gives $|H(z)|\le|z|$ and $|H'(0)|\le1$. Equality at a nonzero point or in the [derivative](../../../../../derivative.md) forces that quotient to be a constant of modulus one, again by the [maximum modulus principle](../../../../../maximum-modulus-principle.md); hence $H(z)=e^{i\theta}z$.

Now let $\phi_a(z)=(z-a)/(1-\overline az)$ and apply this result to $H=\phi_{F(w)}\circ F\circ\phi_w^{-1}$, which fixes zero. The modulus inequality is exactly the displayed distance inequality, and $\rho=\log((1+\delta)/(1-\delta))$ is increasing in $\delta$, giving hyperbolic contraction. Also $|\phi_a'(a)|=(1-|a|^2)^{-1}$ and $|({\phi_w^{-1}})'(0)|=1-|w|^2$, so the [chain rule](../../../../../chain-rule.md) proves the [derivative](../../../../../derivative.md) inequality. The equality statement follows from the rotation case of the [Schwarz lemma](../../../../../schwarz-lemma.md) after undoing the two automorphisms. Conversely a disc automorphism preserves the distance and attains equality.

There is a maximum of the [derivative](../../../../../derivative.md) modulus in the given annulus family, which is nonempty because it contains the constant function one. Indeed the functions are bounded by $e$, and [Cauchy estimates](../../../../../cauchy-estimate.md) bound their [derivatives](../../../../../derivative.md) at zero. Take a sequence whose [derivative](../../../../../derivative.md) moduli approach the finite supremum. By [Montel theorem](../../../../../montel-s-theorem.md) it has a subsequence converging locally uniformly to a [holomorphic function](../../../../../holomorphic-function.md) $f$, with $f(0)=1$ and $e^{-1}\le|f|\le e$. The upper equality cannot occur at an interior point, because the [maximum modulus principle](../../../../../maximum-modulus-principle.md) would force a constant of modulus $e$, contrary to $f(0)=1$. The lower equality is excluded by applying the same argument to $1/f$, which is [holomorphic](../../../../../complex-differentiability-at-a-point.md) because $|f|\ge e^{-1}$. Thus the limit still maps into the open annulus. [Locally uniform convergence](../../../../../locally-uniform-convergence.md) gives convergence of [derivatives](../../../../../derivative.md) by the [Cauchy integral formula](../../../../../cauchy-integral-formula.md), so this limit attains the supremum.

To compute it and all extremizers, the nonvanishing function $f$ on the [simply connected](../../../../../simply-connected-space.md) disc has a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) $h$ with $h(0)=0$. One can construct it by integrating $f'/f$ from zero; differentiation shows $e^h/f$ is constant, hence one. Its real part obeys $-1<\operatorname{Re}h<1$. The map

$$
T(h)=\tan\frac{\pi h}{4}
$$

is a [biholomorphism](../../../../../biholomorphism.md) from this vertical strip onto the disc. To check the inverse explicitly, for $|z|<1$ the ratio $(1+iz)/(1-iz)$ has positive real part, so its logarithm with value zero at zero has imaginary part in $(-\pi/2,\pi/2)$. Therefore

$$
s(z)=\frac4\pi\arctan z=\frac{2}{\pi i}\log\frac{1+iz}{1-iz}
$$

has real part between minus one and one, and direct substitution gives $T(s(z))=z$. The strip restriction removes the period ambiguity of the [tangent](../../../../../tangent.md), so these are inverse maps.

Applying the [Schwarz lemma](../../../../../schwarz-lemma.md) to $T\circ h$ gives $(\pi/4)|h'(0)|\le1$. Since $f'(0)=h'(0)$, the exact maximum is

$$
\boxed{\max_{f\in\mathcal F}|f'(0)|=\frac4\pi.}
$$

It is attained by $f(z)=\exp((4/\pi)\arctan z)$. The equality case requires $T(h(z))=e^{i\theta}z$, and hence all maximizing functions are

$$
\boxed{f_\theta(z)=\exp\left(\frac4\pi\arctan(e^{i\theta}z)\right),\qquad\theta\in\mathbb R.}
$$

Their [derivatives](../../../../../derivative.md) are $(4/\pi)e^{i\theta}$, so **the extremizer is not unique**: there is exactly this circle of distinct functions, with the parameter considered modulo $2\pi$. This is the [extremal derivative of a disc map into a symmetric annulus](../../../../../extremal-derivative-of-a-disc-map-into-a-symmetric-annulus.md) for $L=1$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
