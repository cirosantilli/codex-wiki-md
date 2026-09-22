<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The reaction sign and the meaning of recoil translation matter here. In [Lighthill elongated-body theory](../../../../../lighthill-elongated-body-theory.md), put $\mathcal D=\partial_t+U\partial_x$. The transverse momentum imparted to the fluid per unit length is $m\mathcal Dh$, so the lateral [force](../../../../../force.md) on the fish is $-\mathcal D(m\mathcal Dh)$. Thus body [mass](../../../../../mass.md) and positive [added mass](../../../../../added-mass.md) enter effective inertia with the same sign. The periodic trailing-edge thrust, to quadratic order in slope, is

$$
\boxed{\overline T=\frac m2\left\langle h_t^2-U^2h_x^2\right\rangle_{x=L}.}
$$

The reaction sign and this small-amplitude thrust formula can also be checked in [the primary derivation of the elongated-body force](https://arxiv.org/pdf/2409.20162), equations (2.6), (3.2) and the discussion after (3.5). For the long-body limit below, the recoiling leading edge contributes only at relative order $\alpha^{-2}$.

**The requested recoil and thrust formulas cannot all hold for the literal fish described.** In particular, the printed thrust would remain $-mU^2/4$ when $h_1=0$, although a straight, unperturbed fish has $h_t=h_x=0$ and zero reactive thrust. Its negative term is missing an amplitude-squared slope factor. The stated effective translational coefficient $M'-1$ also has the wrong sign for positive [added mass](../../../../../added-mass.md), and the literal [centre of mass](../../../../../center-of-mass.md) translation cannot be equated to the translation of an arbitrarily chosen undeformed body reference line. The PDF defines $I'=I/[m(\alpha L)^3]$; the converted TeX incorrectly uses the square.

Here are the [force balance](../../../../../force-balance.md) and angular [momentum](../../../../../momentum.md) calculations for a consistent interpretation of the stated uniform fish. They give a corrected recoil solution, as well as a direct test of the printed equations. Define

$$
\ell=(\alpha+1)L,\qquad x_c=\frac{(1-\alpha)L}{2},\qquad \xi=x-x_c,\qquad \mu_b=\frac M\ell,
$$

and let $R$ be actual [centre of mass](../../../../../center-of-mass.md) displacement. The prescribed deformation has mean $a(t)=h_1f(t)/[2(\alpha+1)]$. Its mass-weighted mean must be removed in the [recoil correction in elongated-body theory](../../../../../recoil-correction-in-elongated-body-theory.md):

$$
h(x,t)=R(t)+\xi\theta(t)+h_0(x,t)-a(t).
$$

Indeed $\int h\,dx=\ell R$, since $\int\xi dx=0$ and $\int h_0dx=\ell a$. Introduce the two geometric integrals

$$
J=\int_{-\alpha L}^L\xi^2dx=\frac{\ell^3}{12},\qquad
C=\frac1{f}\int_{-\alpha L}^L\xi h_0dx=\frac{h_1L^2(3\alpha+1)}{12}.
$$

For uniform mass per unit length, $I=\mu_bJ$ at leading small-amplitude order. Retaining the symbol $I$ makes the rotational [momentum](../../../../../momentum.md) balance transparent.

The needed integrals of transverse acceleration and convective derivatives are

$$
\begin{aligned}
\int h_{tt}dx&=\ell\ddot R,&\int h_{xt}dx&=\ell\dot\theta+h_1\dot f,&\int h_{xx}dx&=\frac{h_1}{L}f,\\
\int\xi h_{tt}dx&=J\ddot\theta+C\ddot f,&\int\xi h_{xt}dx&=\frac{\alpha Lh_1}{2}\dot f,&\int\xi h_{xx}dx&=\frac{(\alpha-1)h_1}{2}f.
\end{aligned}
$$

The second spatial derivative includes the hinge's slope jump, as a [distributional derivative](../../../../../distributional-derivative.md); discarding it would incorrectly remove the $U^2$ terms. Newton's lateral equation is $M\ddot R=-m\int\mathcal D^2h\,dx$. The angular [momentum](../../../../../momentum.md) of the deforming fish is $I\dot\theta+\mu_bC\dot f$, so its time derivative equals $-m\int\xi\mathcal D^2h\,dx$. Consequently the consistent uniform-added-mass recoil equations are

$$
\boxed{(M+m\ell)\ddot R=-2mU(\ell\dot\theta+h_1\dot f)-\frac{mU^2h_1}{L}f,}
$$



$$
\boxed{(I+mJ)\ddot\theta=-(\mu_b+m)C\ddot f-mU\alpha Lh_1\dot f-\frac{mU^2(\alpha-1)h_1}{2}f.}
$$

These follow directly from the local [Lighthill elongated-body theory](../../../../../lighthill-elongated-body-theory.md) model with the physical reaction sign. An alternative reference-line translation replaces $R$ by $R-a$, and changes the shape forcing, but cannot change $M+m\ell$ to a difference of two positive inertias. Leading-edge details of a uniform-depth idealization can require an end model; they do not alter this reaction-sign test or the zero-stroke counterexample.

For $f=\cos\omega t$, write $R=\operatorname{Re}(re^{i\omega t})$ and $\theta=\operatorname{Re}(\tau e^{i\omega t})$, choosing the periodic response and omitting free rigid-motion constants. The two balances give the explicit recoil amplitudes

$$
\boxed{\tau=\frac{-(\mu_b+m)C+i mU\alpha Lh_1/\omega+mU^2(\alpha-1)h_1/(2\omega^2)}{I+mJ},}
$$



$$
\boxed{r=\frac{2imU(\ell\tau+h_1)/\omega+mU^2h_1/(L\omega^2)}{M+m\ell}.}
$$

At the tail the displacement and slope amplitudes are $H_L=h_1+r+\ell\tau/2-h_1/[2(\alpha+1)]$ and $S_L=h_1/L+\tau$. Thus a corrected, directly calculable mean thrust is

$$
\boxed{\overline T=\frac m4\left(\omega^2|H_L|^2-U^2|S_L|^2\right),}
$$

within the trailing-edge approximation, with any retained leading-edge contribution treated consistently. This expression has the correct dimensions and vanishes quadratically with stroke amplitude.

A particularly simple independent check is the limit $U=0$. For the uniform fish, $I=\mu_bJ$, the balances give $\ddot R=0$ and $\theta=-Cf/J$ for the periodic response. The tail displacement amplitude is then exactly

$$
H_L=h_1\left[1-\frac1{2(\alpha+1)}-\frac{3\alpha+1}{2(\alpha+1)^2}\right]=h_1\frac{\alpha^2}{(\alpha+1)^2}.
$$

Hence, to the requested relative order,

$$
\boxed{\overline T=\frac{mh_1^2\omega^2}{4}\left[1-\frac4\alpha+O(\alpha^{-2})\right]\quad(U=0).}
$$

The leading-edge contribution is only $O(\alpha^{-2})$ here. This recoil reduction contradicts the printed positive correction, for example for $M'=2$, $I'=1/6$. It also shows explicitly why treating the prescribed shape's moving mass as stationary would give a different model.

For completeness, the positive correction quoted in the question has a simple conditional origin if its two displayed recoil equations are accepted as formal equations rather than derived physical balances. Put $J'=I'+1/6$ and keep $U/(\omega L)$ fixed as $\alpha\to\infty$, away from $M'=1$. Adding those equations and then using the first gives their leading periodic response

$$
\theta\sim\frac{h_1f}{4\alpha^2LJ'},\qquad
R\sim\frac{h_1}{2\alpha(M'-1)}\left(f+\frac{4U}{L}\int fdt\right).
$$

Under the additional reference-line interpretation $h=h_0+R+\xi\theta$, the in-phase tail amplitude is $h_1[1+1/(2\alpha(M'-1))+1/(8\alpha J')]$. Squaring it in the trailing-edge thrust gives the printed frequency correction. Even this formal route, however, gives the amplitude-consistent result

$$
\overline T_{\mathrm{formal}}=\frac m4\left[h_1^2\omega^2-\frac{U^2h_1^2}{L^2}+\frac{h_1^2\omega^2}{\alpha}\left\{\frac1{M'-1}+\frac1{4J'}\right\}\right]+O(\alpha^{-2}),
$$

not a term $-mU^2/4$ independent of $h_1$. The quadrature part of $R$ first changes the squared displacement at relative order $\alpha^{-2}$, while recoil changes the tail slope at that order as well. This conditional calculation explains the intended algebra without presenting the flawed starting equations as a physical theorem.

Reactive thrust is positive when the tail's lateral-motion term exceeds its streamwise slope penalty; for an unrecoiling hinged tail this requires $\omega L>U$. A real steady swimming speed additionally balances the thrust against resistive [drag force](../../../../../drag-physics.md), absent from this inertial idealization. Recoil can alter either term and is not universally thrust-enhancing. A pole at $M'=1$ is not a physical negative-added-mass resonance: the genuine combined inertias remain positive.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
