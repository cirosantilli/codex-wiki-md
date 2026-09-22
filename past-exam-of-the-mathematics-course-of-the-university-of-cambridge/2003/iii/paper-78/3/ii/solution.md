<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The full [Love wave](../../../../../../love-wave.md) problem replaces the rigid base by a decaying substrate displacement. With $Y=A\cos(qz)$ in the layer and $Y=B e^{-\kappa(z-h)}$ below it,

$$
q^2=\frac{\omega^2}{\beta'^2}-k^2,\qquad
\kappa^2=k^2-\frac{\omega^2}{\beta^2}>0,
\qquad\tan(qh)=\frac{\mu\kappa}{\mu'q},
$$

where $\mu'=\rho'\beta'^2$ and $\mu=\rho\beta^2$. Displacement continuity gives $B=A\cos(qh)$ and [traction](../../../../../../traction.md) continuity gives $\mu'q\sin(qh)=\mu\kappa\cos(qh)$. The rigid base is therefore a good approximation only when $\mu\kappa\gg\mu'q$: then the substrate displacement is small and $qh$ lies close to $\chi_n=(n+1/2)\pi$.

Put $\epsilon=\beta'/\beta$, $\eta=\mu'/\mu$, $y=qh$, $W=\omega h/\beta'$ and $K=kh$. The complete dispersion branch can be parameterized without root finding:

$$
\boxed{W(y)=\frac{y\sqrt{1+\eta^2\tan^2y}}{\sqrt{1-\epsilon^2}},\qquad
K(y)=\frac{y\sqrt{\epsilon^2+\eta^2\tan^2y}}{\sqrt{1-\epsilon^2}},
\quad n\pi<y<\chi_n}.
$$

Then $c=\beta'W/K$ and $U=\beta'W'/K'$. At the lower end, $c\to\beta$ and $U\to\beta$. The [Love-wave cutoff frequencies](../../../../../../love-wave-cutoff-frequencies.md) are $\omega_{c,n}=n\pi\beta'/[h\sqrt{1-\epsilon^2}]$, with zero cutoff for the fundamental. Thus the rigid-layer formula cannot describe the fundamental's low-[frequency](../../../../../../frequency.md) limit or the low-[frequency](../../../../../../frequency.md) part of an overtone: it would either give no propagating mode or predict $c>\beta$, outside the trapping interval $\beta'<c<\beta$.

For comparable densities and a fixed mode index, $\eta=(\rho'/\rho)\epsilon^2\ll1$. Write $y=\chi_n-\delta$ near the strong-dispersion transition. In the region controlling the [group-velocity minimum of a high-contrast Love wave](../../../../../../group-velocity-minimum-of-a-high-contrast-love-wave.md), $\delta\ll1$ and $\eta/\delta\gg\epsilon$. The leading derivatives give

$$
\frac U{\beta'}\simeq\frac{\delta^2}{\eta\chi_n}+\frac\eta\delta.
$$

Their minimum is at

$$
\delta_{\min}\sim\left(\frac{\eta^2\chi_n}{2}\right)^{1/3},\qquad
\boxed{\omega_{\min,n}\sim\frac{\beta'\chi_n}{h}=\omega_n},
\qquad
\frac{U_{\min,n}}{\beta'}\sim\frac3{2^{2/3}}\left(\frac\eta{\chi_n}\right)^{1/3}.
$$

The [frequency](../../../../../../frequency.md) estimate follows by inserting $\delta_{\min}$ into $W\simeq(\chi_n-\delta)[1+\eta^2/(2\delta^2)+\epsilon^2/2]$: the two leading terms of size $\delta$ cancel. The real [group velocity](../../../../../../group-velocity.md) has a finite minimum and turns upwards near the rigid-layer threshold, whereas the rigid formula has zero group speed at its artificial threshold.

For a useful estimate of the validity range, put $\Delta=W-\chi_n>0$. The rigid prediction has $K_R^2=W^2-\chi_n^2\simeq2\chi_n\Delta$. The finite-load phase correction is $\delta\simeq\eta\chi_n/(\kappa h)$; its changes to both $K$ and $dK/dW$ are small if

$$
\boxed{\Delta\gg\max\left\{\chi_n\epsilon^2,(\eta^2\chi_n)^{1/3}\right\}}.
$$

The first condition keeps $K_R$ away from the substrate propagation boundary; the second controls the rapidly changing interface phase. Equivalently, the rigid formulas are reliable sufficiently above the actual group-velocity minimum, beyond its narrow transition interval. At fixed $\omega/\omega_n>1$ separated from one, they become asymptotically accurate as the contrast grows. They are particularly simple at $\omega\gg\omega_n$, where both velocities approach $\beta'$. Within the transition and below it the full [dispersion relation](../../../../../../dispersion-relation.md) is required.

The small speed ratio alone is insufficient if the layer density grows so strongly that $\mu'/\mu$ is not small. For such materials the exact load criterion $\mu\kappa\gg\mu'q$ and its [frequency](../../../../../../frequency.md) derivatives should be used; the preceding contrast estimates assume a bounded order-one density ratio and fixed $n$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
