<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\eta>0$ denote the uniform [magnetic diffusivity](../../../../../magnetic-diffusivity.md). The [resistive induction equation](../../../../../resistive-induction-equation.md) for a [solenoidal vector field](../../../../../solenoidal-vector-field.md) in an [incompressible flow](../../../../../incompressible-flow.md) is

$$
\partial_t\mathbf B+(\mathbf u\cdot\nabla)\mathbf B=(\mathbf B\cdot\nabla)\mathbf u+\eta\nabla^2\mathbf B,\qquad\nabla\cdot\mathbf B=0.
$$

Here the radial compression and axial stretching have zero total divergence: $r^{-1}\partial_r(-\omega r^2)+\partial_z(2\omega z)=0$. A purely axial field independent of $z$ is automatically solenoidal, and the stretching term is $2\omega B_z\hat{\mathbf z}$. Thus the ansatz closes under the equation. For its angular mode, with $m$ a nonnegative integer,

$$
\partial_tB_z-\omega r\partial_rB_z
=2\omega B_z+\eta\left(\partial_r^2+r^{-1}\partial_r+r^{-2}\partial_\phi^2\right)B_z.
$$

This is [magnetic concentration by an incompressible stagnation flow](../../../../../magnetic-concentration-by-an-incompressible-stagnation-flow.md).

Put $q=r/g(t)$ and $D_mb=b''+q^{-1}b'-m^2q^{-2}b$. Substitution and division by $f$ give

$$
\left(\frac{f'}f-2\omega\right)b-\left(\frac{g'}g+\omega\right)qb'=\frac{\eta}{g^2}D_mb.
$$

A convenient [self-similar magnetic mode in a stagnation flow](../../../../../self-similar-magnetic-mode-in-a-stagnation-flow.md) is obtained by making the two dimensionless separation coefficients constant. Choose

$$
\boxed{gg'+\omega g^2=\eta,\qquad \frac{f'}f=2\omega-\frac{\lambda\eta}{g^2},\qquad
b''+(q^{-1}+q)b'+\left(\lambda-\frac{m^2}{q^2}\right)b=0.}
$$

The constant $\lambda$ labels the radial modes. More generally the first right side can be $\beta\eta$ and the radial drift term $\beta qb'$; the displayed equations choose the positive-width normalization $\beta=1$.

If $g(0)=g_0>0$, the width is

$$
\boxed{g(t)^2=\frac{\eta}{\omega}+\left(g_0^2-\frac{\eta}{\omega}\right)e^{-2\omega t}\quad(\omega\ne0).}
$$

For $\omega=0$ its continuous limiting expression is $g^2=g_0^2+2\eta t$. Since $\eta/g^2=\omega+g'/g$, the amplitude is

$$
\boxed{f(t)=f_0e^{(2-\lambda)\omega t}\left(\frac{g_0}{g(t)}\right)^\lambda.}
$$

For the compressive case $\omega>0$, the width tends to the diffusion-strain balance scale $\sqrt{\eta/\omega}$ rather than collapsing to zero.

Let $I_b=\int_0^\infty b(q)^2q\,dq$ be finite, and let $C_m=\int_0^{2\pi}\cos^2(m\phi)\,d\phi$, equal to $2\pi$ for $m=0$ and $\pi$ otherwise. The [magnetic energy](../../../../../magnetic-energy.md) per unit axial length is

$$
E(t)=\frac{C_m}{2\mu_0}f(t)^2g(t)^2I_b,
$$

so the complete time dependence is

$$
\boxed{\frac{E(t)}{E(0)}=e^{2(2-\lambda)\omega t}\left(\frac{g(t)}{g_0}\right)^{2-2\lambda},\qquad
\frac{E'}E=2\omega+\frac{2(1-\lambda)\eta}{g^2}.}
$$

The angular integral is only a constant; zero signed [magnetic flux](../../../../../magnetic-flux.md) does not force $I_b$ or $E$ to vanish.

For $m=0$, smoothness on the axis requires $b(0)$ finite and $b'(0)=0$. Set $s=-q^2/2$ and $b=h(s)$. The radial equation becomes the [Kummer differential equation](../../../../../kummer-differential-equation.md)

$$
s h''+(1-s)h'-\frac\lambda2h=0.
$$

Its regular solution is

$$
\boxed{b(q)=b(0)M\left(\frac\lambda2,1,-\frac{q^2}{2}\right),}
$$

where $M$ is the [confluent hypergeometric function of the first kind](../../../../../confluent-hypergeometric-function-of-the-first-kind.md). The second independent solution has a logarithmic singularity at the axis and is inadmissible for a smooth field. For real $\lambda>0$, the regular solution vanishes at infinity: generically it has a $q^{-\lambda}$ tail; at positive even integer $\lambda$ it instead has a Gaussian times a polynomial. Thus decay at infinity alone does not select a unique separation parameter. Generically finite [magnetic energy](../../../../../magnetic-energy.md) further requires $\lambda>1$.

The simplest finite-flux solution is $\lambda=2$, for which $M(1,1,s)=e^s$ and

$$
\boxed{b(q)=b_0e^{-q^2/2},\qquad f(t)=f_0\frac{g_0^2}{g(t)^2}.}
$$

Direct differentiation gives $b''+q^{-1}b'=(q^2-2)b$ and $qb'=-q^2b$, verifying the radial equation. Its axial [magnetic flux](../../../../../magnetic-flux.md) is $2\pi b_0fg^2=2\pi b_0f_0g_0^2$, while its [magnetic energy](../../../../../magnetic-energy.md) grows by $g_0^2/g^2$ if the original width is larger than $\sqrt{\eta/\omega}$. For positive $\eta$ this Gaussian amplification saturates, rather than giving indefinite exponential growth. The other rapidly decaying regular axisymmetric modes have $\lambda=2(n+1)$ and profiles $e^{-q^2/2}L_n(q^2/2)$, where $L_n$ solves $yL_n''+(1-y)L_n'+nL_n=0$.

The energy mechanism is transparent from a separate integral calculation. For any sufficiently decaying field of this axial form, [integration by parts](../../../../../integration-by-parts.md) in the transverse plane gives

$$
\boxed{\frac{dE}{dt}=2\omega E-\frac{\eta}{\mu_0}\int_{\mathbb R^2}|\nabla_\perp B_z|^2\,dS.}
$$

The positive term represents work by the axial stretching, with radial compression accounted for in the area integral. In the ideal limit, $g=g_0e^{-\omega t}$ and $f=f_0e^{2\omega t}$ for any smooth profile, so $E=E_0e^{2\omega t}$ even when $m\ne0$ and the angular mean is zero. For sufficiently weak initial diffusion, this also gives genuine finite-time energy amplification at positive $\eta$.

Even sustained energy growth is possible in this unbounded model if slowly decaying profiles are admitted. For example, with $\omega>0$, take the constant width $g=\sqrt{\eta/\omega}$, $m=1$ and $1<\lambda<2$. The regular radial solution $b=qM((1+\lambda)/2,2,-q^2/2)$ has a $q^{-\lambda}$ tail and finite $I_b$. It gives $E\propto e^{2(2-\lambda)\omega t}$ and zero signed flux through every centered disk. Its absolute flux integral over the whole plane diverges, so the zero-flux statement here means the limit of these disk integrals. This example is not an isolated bounded-body dynamo: the velocity is unbounded at infinity and the field has an algebraic tail. **The dynamo property concerns conversion of fluid energy into magnetic energy, not production of a nonzero signed magnetic flux; growth and its boundary assumptions must be specified.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
