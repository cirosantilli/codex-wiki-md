# Rapidity

↑ **Parent:** [Lorentz boost](lorentz-boost.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rapidity)

[Rapidity](rapidity.md) is a dimensionless parameter for a signed collinear [velocity](velocity.md) $u$ with $|u|<c$, defined using the [inverse hyperbolic functions](inverse-hyperbolic-functions.md) by

$$
\theta=\operatorname{artanh}(u/c)=\frac12\ln\frac{1+u/c}{1-u/c},\qquad u=c\tanh\theta.
$$

Here $c$ is the [speed of light](speed-of-light.md), and $\tanh$ is the [hyperbolic tangent](hyperbolic-tangent.md). Zero [velocity](velocity.md) has zero [rapidity](rapidity.md); negative [velocity](velocity.md) has negative [rapidity](rapidity.md). Every finite real [rapidity](rapidity.md) gives $|u|<c$, while $u\to\pm c$ requires $\theta\to\pm\infty$. Thus a [light](light.md) ray has no finite [rapidity](rapidity.md) in this parametrization. The header's formula uses [natural units](natural-units.md) $c=1$: its $v$ is the numerical [velocity](velocity.md) $u/c$.

For the [inertial frames](inertial-frame.md) in the [velocity-addition formula](velocity-addition-formula.md), $S'$ moves at signed [velocity](velocity.md) $V$ along the $x$-axis of $S$. Set $\phi=\operatorname{artanh}(V/c)$. Re-expressing the same particle in the moving [inertial frame](inertial-frame.md) gives

$$
\theta'=\theta-\phi,\qquad \theta=\theta'+\phi.
$$

The subtraction is a passive change of [reference frame](reference-frame.md); the inverse adds the particle's [rapidity](rapidity.md) in $S'$ to the frame's [rapidity](rapidity.md) relative to $S$. For example, $V=0.6c$ and $u'=0.6c$ give $\phi=\theta'=\ln2$, so $\theta=\ln4$ and $u=c\tanh(\ln4)=15c/17$, exactly as in the [velocity-addition formula](velocity-addition-formula.md).

For a massive particle of [rest mass](invariant-mass.md) $m>0$ moving in one spatial dimension, its [energy](energy-split.md) and signed [momentum](momentum-split.md) are

$$
E=mc^2\cosh\theta,\qquad p=mc\sinh\theta.
$$

The [hyperbolic cosine](hyperbolic-cosine.md) is the particle's [Lorentz factor](lorentz-factor.md), and the [hyperbolic sine](hyperbolic-sine.md) is $\gamma u/c$. The [hyperbolic Pythagorean identity](hyperbolic-pythagorean-identity.md) immediately gives the [relativistic energy-momentum relation](energy-momentum-relation.md) $E^2-c^2p^2=m^2c^4$. In the older $c=1$ notation, writing the [rest mass](invariant-mass.md) as $M$ recovers $v=\tanh\theta$, $E=M\cosh\theta$, and $p=M\sinh\theta$. These expressions use [natural units](natural-units.md) in which the factors of $c$ are numerically one; the preceding formulas restore those factors explicitly. [David Tong, Dynamics and Relativity, §7.3.2: rapidity; §7.4.3: energy and momentum](https://davidtong.org/pdfs/teaching/dynamics-and-relativity/dynrel7.pdf).

The useful simplification follows from the [hyperbolic-function identity](hyperbolic-function-identity.md) $\tanh(a+b)=(\tanh a+\tanh b)/(1+\tanh a\tanh b)$: the nonlinear [velocity-addition formula](velocity-addition-formula.md) becomes ordinary addition of [rapidities](rapidity.md). See [iterated collinear boosts with equal rapidity](iterated-collinear-boosts-with-equal-rapidity.md) for a plotted example. A common collinear [Lorentz boost](lorentz-boost.md) shifts every [rapidity](rapidity.md) by the same constant, so a [rapidity](rapidity.md) difference is invariant. This makes [rapidity](rapidity.md) useful for relativistic [factorized scattering](factorized-scattering.md) in one spatial dimension, where two-body [S-matrices](s-matrix.md) depend on the difference of the incoming [rapidities](rapidity.md), with particle species fixed.

**Table of contents**

- [Iterated collinear boosts with equal rapidity](iterated-collinear-boosts-with-equal-rapidity.md)

## ↑ Ancestors (6)

1. [Lorentz boost](lorentz-boost.md)
2. [Lorentz transformation](lorentz-transformation.md)
3. [Special relativity](special-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (49)

- [Angular-diameter ratio under a collinear boost](angular-diameter-ratio-under-a-collinear-boost.md)
- [Angular size under a collinear relativistic boost](angular-size-under-a-collinear-relativistic-boost.md)
- [Bound-state fusion of factorized S-matrices](bound-state-fusion-of-factorized-s-matrices.md)
- [Faddeev-Zamolodchikov algebra](faddeev-zamolodchikov-algebra.md)
- [Faddeev-Zamolodchikov associativity constraint](faddeev-zamolodchikov-associativity-constraint.md)
- [Finite-acceleration correction to a relativistic cruise](finite-acceleration-correction-to-a-relativistic-cruise.md)
- [Full S-matrix phase from a classical soliton delay](full-s-matrix-phase-from-a-classical-soliton-delay.md)
- [Hermitian analyticity of a two-particle S-matrix](hermitian-analyticity-of-a-two-particle-s-matrix.md)
- [Hyperbolic motion from an initial event and rapidity](hyperbolic-motion-from-an-initial-event-and-rapidity.md)
- [Integrable quantum field theory](integrable-quantum-field-theory.md)
- [Iterated collinear boosts with equal rapidity](iterated-collinear-boosts-with-equal-rapidity.md)
- [Orthogonal-invariant scattering channels](orthogonal-invariant-scattering-channels.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/7c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-4/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-46/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-47/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-47/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-47/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-50/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-50/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-50/3/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2013/paper-1/1/a/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2013/paper-1/3/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2019/section-a/2/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2022/section-a/1/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2022/section-b/6/b/ii/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2022/section-b/6/b/iv/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2013/paper-1/5/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2013/paper-1/5/b/solution.md)
- [Photon rocket](photon-rocket.md)
- [Photon-rocket fuel for acceleration and braking](photon-rocket-fuel-for-acceleration-and-braking.md)
- [Physical rapidity strip](physical-rapidity-strip.md)
- [Rapidity](rapidity.md)
- [Rapidity form of one-dimensional proper acceleration](rapidity-form-of-one-dimensional-proper-acceleration.md)
- [Relativistic bound-state mass from a rapidity pole](relativistic-bound-state-mass-from-a-rapidity-pole.md)
- [Scattering s-channel](scattering-s-channel.md)
- [Sine-Gordon multisoliton tau representation](sine-gordon-multisoliton-tau-representation.md)
- [Sine-Gordon two-kink time advance](sine-gordon-two-kink-time-advance.md)
- [Three-particle bound state from equal-mass fusion](three-particle-bound-state-from-equal-mass-fusion.md)
- [Transverse mass](transverse-mass.md)
- [Unit-modulus hyperbolic scattering block](unit-modulus-hyperbolic-scattering-block.md)
- [Unwrapped reflectionless sine-Gordon transmission phase](unwrapped-reflectionless-sine-gordon-transmission-phase.md)
- [Velocity-addition formula](velocity-addition-formula.md)
- [Z pair mass and W transverse-mass limits](z-pair-mass-and-w-transverse-mass-limits.md)
