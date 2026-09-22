<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [normal modes](../../../../../../normal-mode.md) $e^{ikx+st}$, so $s=-i\omega$ in the convention $e^{ikx-i\omega t}$. For a translation-invariant, well-posed linear [initial value problem](../../../../../../initial-value-problem.md) on the whole line, localized data are propagated by a causal [Green function](../../../../../../green-s-function.md). The [Fourier transform](../../../../../../fourier-transform.md) in space and [Laplace transform](../../../../../../laplace-transform.md) in time give an inverse [integral](../../../../../../integral.md) whose denominator is the [dispersion relation](../../../../../../dispersion-relation.md) $D(k,s)$. The initial temporal contour is a Bromwich line to the right of every real-wave-number temporal singularity.

The [Briggs-Bers technique](../../../../../../briggs-bers-criterion.md) lowers that temporal contour while deforming the spatial contour to avoid its poles. A [spatial pinch point](../../../../../../spatial-pinch-point.md) occurs when two spatial branches originating on opposite sides of the original Fourier contour collide and prevent further deformation. Algebraically a simple candidate satisfies $D=D_k=0$, with $D_s\ne0$ and $D_{kk}\ne0$; these equations alone do not establish the pinch topology. A same-side collision is a [false spatial saddle in quartic dispersion](../../../../../../false-spatial-saddle-in-quartic-dispersion.md). The opposite-side requirement is also explicit in [the primary numerical study of pinch-point detection](https://www.sciencedirect.com/science/article/abs/pii/S0021999105003177).

The rightmost contributing pinch determines the fixed-position exponential growth of the impulse response, ordinarily with a $t^{-1/2}$ [saddle point](../../../../../../saddle-point.md) prefactor. A positive rate is [absolute wave-packet instability](../../../../../../absolute-wave-packet-instability.md). If real-wave-number [normal modes](../../../../../../normal-mode.md) grow but the impulse response decays at each fixed position, it is [convective wave-packet instability](../../../../../../convective-wave-packet-instability.md); growth can then occur along moving rays. If no temporal [normal mode](../../../../../../normal-mode.md) grows, the system is stable, with equality thresholds treated as marginal rather than exponential decay. Along a ray $x=vt$, apply the same argument to $s(k)+ikv$, whose [saddle point](../../../../../../saddle-point.md) condition is $s'(k)+iv=0$. Thus the laboratory frame is part of the absolute/convective definition.

For the quartic problem the temporal [dispersion relation](../../../../../../dispersion-relation.md) is

$$
s(k)=a_1k^2-a_2k^4-a_3,\qquad D(k,s)=s+a_3-a_1k^2+a_2k^4.
$$

Write $a=\operatorname{Re}a_1$, $b=\operatorname{Re}a_2$, $c=\operatorname{Re}a_3$. For $b>0$ the causal Fourier kernel is absolutely convergent for positive time and the [finite maximum temporal growth rate](../../../../../../finite-maximum-temporal-growth-rate.md) is

$$
\boxed{\sigma_T=\sup_{k\in\mathbb R}\operatorname{Re}s(k)=-c+\frac{\max(a,0)^2}{4b}.}
$$

The usual initial-value framework fails if $b<0$, or if $b=0$ and $a>0$, because arbitrarily large real [wave numbers](../../../../../../wavenumber.md) grow arbitrarily fast: no finite Bromwich line can start to their right. This is a high-frequency ill-posedness obstruction, not an absolute instability criterion. If $b=0$ and $a\leq0$, the growth bound is finite, but the dispersive limiting case needs oscillatory Fourier inversion or a limiting-absorption construction when there is no quadratic damping. It must not be justified by the absolutely convergent quartic-diffusion argument. The following explicit calculation first assumes $b>0$ and $a_2\ne0$.

The double-root candidates are

$$
k_0=0,\quad s_0=-a_3;\qquad k_\pm^2=\frac{a_1}{2a_2},\quad s_\pm=\frac{a_1^2}{4a_2}-a_3.
$$

Rather than assume all are physical, compute the causal resolvent at the impulse location. Put $S=s+a_3$, and for large $\operatorname{Re}s$ factor

$$
S-a_1k^2+a_2k^4=a_2(k^2+\kappa_1^2)(k^2+\kappa_2^2),\qquad \operatorname{Re}\kappa_j>0.
$$

Then $\kappa_1\kappa_2=\sqrt{S/a_2}$ and $(\kappa_1+\kappa_2)^2=-a_1/a_2+2\sqrt{S/a_2}$, with sheets selected from that large-$s$ region. [Partial fraction decomposition](../../../../../../partial-fraction-decomposition.md) and $\int_{\mathbb R}(k^2+\kappa^2)^{-1}dk=\pi/\kappa$ give the [quartic impulse-response Laplace resolvent](../../../../../../quartic-impulse-response-laplace-resolvent.md)

$$
\boxed{\widehat G(0,s)=\frac1{2\pi}\int_{\mathbb R}\frac{dk}{S-a_1k^2+a_2k^4}=\frac1{2\sqrt S\sqrt{2\sqrt{a_2}\sqrt S-a_1}}.}
$$

All roots in this expression are continued from the causal region, not selected afresh at a candidate collision. The two possible singularities are now transparent. $S=0$ is a square-root singularity when $a_1\ne0$. The extra singularity requires $\sqrt S=a_1/(2\sqrt{a_2})$. Taking $\sqrt{a_2}$ with positive real part and putting $z=a_1/\sqrt{a_2}$, this lies on the physical $\sqrt S$ sheet precisely when $\operatorname{Re}z>0$. If that real part is zero the candidate is on a cut boundary and has nonpositive real $S$, so it cannot lie to the right of $S=0$. For $\operatorname{Re}z<0$, the apparently growing candidate may be on the wrong sheet altogether.

Therefore the [physical-sheet growth rate of a quartic impulse response](../../../../../../physical-sheet-growth-rate-of-a-quartic-impulse-response.md) is

$$
\boxed{\sigma_A=-c+M,\qquad M=\begin{cases}\max\{0,\operatorname{Re}(a_1^2/(4a_2))\},&\operatorname{Re}(a_1/\sqrt{a_2})>0,\\0,&\operatorname{Re}(a_1/\sqrt{a_2})\leq0.\end{cases}}
$$

These are resolvent branch singularities on the causal continuation, so the formula implements the pinch test instead of merely listing formal [saddle point](../../../../../../saddle-point.md) rates. For $a_1=0$, the zero [saddle point](../../../../../../saddle-point.md) is fourth-order and the resolvent is proportional to $S^{-3/4}$; its impulse response is proportional to $t^{-1/4}e^{-a_3t}$ and the same exponential-rate formula applies. At nondegenerate candidates the prefactor is $t^{-1/2}$.

The classification in this diffusive case is now explicit: **$\sigma_T<0$ gives stability; $\sigma_A>0$ gives absolute instability; $\sigma_T>0$ with $\sigma_A<0$ gives convective instability.** When $\sigma_T>0$ and $\sigma_A=0$, the nondegenerate fixed-position response still decays algebraically, at the marginal absolute/convective threshold. Other equality cases require the stated [saddle point](../../../../../../saddle-point.md) prefactors. Temporal instability supplies a growing ray: at a real maximum of $\operatorname{Re}s(k)$, choose $v=-\operatorname{Im}s'(k)$ so that the moving-ray [saddle point](../../../../../../saddle-point.md) is stationary there.

Three examples show why complex coefficients and sheets matter. For $(a_1,a_2,a_3)=(2,1,1/2)$, $\sigma_T=\sigma_A=1/2$, so the instability is absolute. For $(1+2i,1,1/10)$, $\sigma_T=3/20>0$ but $\sigma_A=-1/10$, so it is convective even though there is no explicit first-derivative advection term: dispersion carries packets in opposite directions. For $(-2,1,1/2)$, both physical rates are $-1/2$. The formal candidates $k=\pm i$ have $s=1/2$ but fail the physical-sheet condition, so this temporally stable example is not absolutely unstable.

On the admissible boundary $b=0$, $a\leq0$, $a_2\ne0$, the oscillatory or damped Fourier construction has $\sigma_T=-c$. The surviving zero-wave-number stationary response has the same exponential rate $-c$, with a quadratic or quartic algebraic factor; damping/dispersion therefore does not generate a separate convective-growth range there. If $a_2=0$, the problem is second order and its diffusion/dispersive kernel must be used instead of the quartic formula. Application to a finite interval or nonlocalized data also changes the spatial inversion problem, so the whole-line localized-data hypothesis is essential.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
