<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a genus-zero [Polyakov path integral](../../../../../polyakov-path-integral.md), target signature $(-,+,\ldots,+)$ and all four momenta incoming. Define the [Mandelstam variables](../../../../../mandelstam-variables.md) by $s=-(p_1+p_2)^2$, $t=-(p_1+p_3)^2$, $u=-(p_1+p_4)^2$. The [string mass-shell condition](../../../../../string-mass-shell-condition.md) is $p_i^2=4/\alpha'$ and [momentum](../../../../../momentum.md) conservation is $\sum_i p_i=0$, so

$$
\boxed{s+t+u=-\frac{16}{\alpha'}.}
$$

The reduced amplitude omits the overall momentum-conservation [Dirac delta distribution](../../../../../dirac-delta-function.md) and any conventional overall scattering-matrix phase. Interpret each [tachyon vertex operator](../../../../../tachyon-vertex-operator.md) as normal ordered; self-contractions must not be included.

The [free-boson worldsheet propagator](../../../../../free-boson-worldsheet-propagator.md) is $\langle X^a(z)X^b(w)\rangle=-(\alpha'/2)\eta^{ab}\log|z-w|^2$. [Wick theorem](../../../../../wick-s-theorem.md) then evaluates the normal-ordered exponential correlator as the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md)

$$
\left\langle\prod_{j=1}^4{:}e^{ip_j\cdot X(z_j)}{:}\right\rangle\propto\prod_{i<j}|z_i-z_j|^{\alpha'p_i\cdot p_j}.
$$

The [worldsheet zero mode](../../../../../worldsheet-zero-mode.md) supplies [momentum](../../../../../momentum.md) conservation. Four vertices give $g_s^4$ and the sphere contributes $g_s^{-2}$ through the [string genus expansion](../../../../../string-genus-expansion.md), leaving $g_s^2$.

The sphere's residual [Möbius transformations](../../../../../mobius-transformation.md) fix three insertion points. In [sphere gauge fixing for four string vertices](../../../../../sphere-gauge-fixing-for-four-string-vertices.md), take $(z_1,z_2,z_3,z_4)=(z,0,1,\infty)$. The [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md), equivalently the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) for this residual group, supply $|z_{23}z_{24}z_{34}|^2$. At finite $z_4$, this determinant grows as $|z_4|^4$, while the matter correlator decays as $|z_4|^{-4}$ by [momentum](../../../../../momentum.md) conservation and the tachyon [mass](../../../../../mass.md) shell; their product has a finite limit. Equivalently the weight-$(1,1)$ matter operator at infinity is normalized with $|z_4|^4$, while the ghost pair uses the inverse factor. After stripping the fixed-position normalization, only

$$
A^{(4)}=g_s^2\int_{\mathbb C}d^2z\,|z|^{-4-\alpha's/2}|1-z|^{-4-\alpha't/2}
$$

remains. Here choose the standard complex-coordinate measure $d^2z=i\,dz\wedge d\bar z=2\,dx\,dy$. With $dx\,dy$ instead, the reduced normalization must acquire a factor two to give the same requested amplitude. Absolute vertex/sphere normalization is a convention; this choice fixes it consistently with the displayed $2\pi$ prefactor.

Set $a=-1-\alpha's/4$, $b=-1-\alpha't/4$, $c=-1-\alpha'u/4$. Then $a+b+c=1$ and the integrand is $|z|^{2a-2}|1-z|^{2b-2}$. To evaluate the [complex beta integral](../../../../../complex-beta-integral.md) first work where $\operatorname{Re}a,\operatorname{Re}b,\operatorname{Re}c>0$. This ensures convergence near $0$, $1$ and infinity. Set $v=1-a$ and $w=1-b$. [Schwinger parameterization](../../../../../schwinger-parameterization.md) gives

$$
|z|^{-2v}|1-z|^{-2w}=\frac1{\Gamma(v)\Gamma(w)}\int_0^\infty d\lambda\,d\rho\,\lambda^{v-1}\rho^{w-1}e^{-\lambda|z|^2-\rho|z-1|^2}.
$$

Completing the square, the $dx\,dy$ [Gaussian integral](../../../../../gaussian-integral.md) is $\pi(\lambda+\rho)^{-1}\exp[-\lambda\rho/(\lambda+\rho)]$. Change variables to $q=\lambda+\rho$ and $x=\lambda/q$; their [Jacobian determinant](../../../../../jacobian-determinant.md) is $q$. Integrating $q$ gives $\Gamma(v+w-1)[x(1-x)]^{-(v+w-1)}$. The remaining integral is the ordinary [beta function](../../../../../beta-function.md) $B(1-w,1-v)=B(b,a)$. Thus

$$
\int_{\mathbb C}dx\,dy\,|z|^{2a-2}|1-z|^{2b-2}
=\pi\frac{\Gamma(a)\Gamma(b)\Gamma(c)}{\Gamma(1-a)\Gamma(1-b)\Gamma(1-c)}.
$$

Restoring $d^2z=2dx\,dy$ and substituting the [Mandelstam variables](../../../../../mandelstam-variables.md) proves the [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md):

$$
\boxed{A^{(4)}=2\pi g_s^2\frac{\Gamma(-1-\alpha's/4)\Gamma(-1-\alpha't/4)\Gamma(-1-\alpha'u/4)}{\Gamma(2+\alpha's/4)\Gamma(2+\alpha't/4)\Gamma(2+\alpha'u/4)}.}
$$

For physical scattering the original position integral generally fails to converge. The formula defines the amplitude by [analytic continuation](../../../../../analytic-continuation.md) from the convergence domain, with the desired scattering boundary value at real poles; the convergent integral should not be claimed valid for every physical [momentum](../../../../../momentum.md).

The [gamma function](../../../../../gamma-function.md) is a [meromorphic function](../../../../../meromorphic-function.md), with [simple poles](../../../../../simple-pole.md) at nonpositive integers and no zeros, while its reciprocal $1/\Gamma$ is an [entire function](../../../../../entire-function.md). Consequently it is a [meromorphic function](../../../../../meromorphic-function.md) of the independent invariants and a [crossing-symmetric scattering amplitude](../../../../../crossing-symmetry.md): permuting $s,t,u$ leaves it unchanged. Its generic channel poles are

$$
\boxed{s=\frac4{\alpha'}(n-1),\quad n=0,1,2,\ldots,}
$$

and the same tower in $t$ and $u$. They represent the exchanged [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md): the tachyon, massless states including the graviton, and an infinite sequence of massive closed-string levels. There are no threshold [branch cuts](../../../../../branch-cut.md) at this tree order.

A precise check of factorization is the [Virasoro–Shapiro amplitude pole residue](../../../../../virasoro-shapiro-amplitude-pole-residue.md). Near $a=-n$, set $c=1+n-b$ in the nonsingular factor. The [gamma function](../../../../../gamma-function.md) recurrence gives

$$
\frac{\Gamma(b)\Gamma(1+n-b)}{\Gamma(1-b)\Gamma(b-n)}=(-1)^n\prod_{j=1}^n(b-j)^2.
$$

Combining this with $\Gamma(a)\sim(-1)^n/[n!(a+n)]$ shows

$$
\operatorname*{Res}_{s=4(n-1)/\alpha'}A^{(4)}=-\frac{8\pi g_s^2}{\alpha'(n!)^2}\prod_{j=1}^n(b-j)^2.
$$

The [residue](../../../../../residue.md) is a degree-$2n$ polynomial in $t$, consistent with exchange up to spin $2n$ and [scattering-amplitude factorization](../../../../../scattering-amplitude-factorization.md). At exceptional kinematics reciprocal Gamma zeros can remove apparent poles. In particular, when both $a$ and $b$ approach nonpositive integers, the zero from $1/\Gamma(a+b)$ cancels the putative double pole, leaving channel simple-pole terms. Thus one must not count products of numerator poles without using $a+b+c=1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
