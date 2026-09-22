<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The radial velocity of a [Kepler orbit](../../../../../../kepler-orbit.md) follows from the [vis-viva equation](../../../../../../vis-viva-equation.md) after subtracting the tangential component:

$$
v_r^2=\frac{\mu_\star}{a}\frac{(r-q)(Q-r)}{r^2},\qquad
T_c=\frac{2\pi a^{3/2}}{\sqrt{\mu_\star}},\qquad a=\frac{Q+q}{2}.
$$

Each radial interval is crossed twice per [orbital period](../../../../../../orbital-period.md), so its fraction of time is

$$
\boxed{\frac{dt_{\rm both}}{T_c}=p_r(r)\,dr=\frac{r\,dr}{\pi a\sqrt{(r-q)(Q-r)}}.}
$$

This is the [phase-mixed radial probability of a Kepler orbit](../../../../../../phase-mixed-radial-probability-of-a-kepler-orbit.md), normalized to one between $q$ and $Q$. Dividing by the annular area $2\pi r\,dr$ gives the [phase-mixed comet surface density](../../../../../../phase-mixed-comet-surface-density.md) per [comet](../../../../../../comet.md):

$$
\boxed{\Sigma_c(r)=\frac{1}{\pi^2(Q+q)\sqrt{(r-q)(Q-r)}}.}
$$

For $Q\gg a_p>q$,

$$
\boxed{\Sigma_c(a_p)\simeq\frac{1}{\pi^2Q^{3/2}a_p^{1/2}}\left(1-\frac q{a_p}\right)^{-1/2}.}
$$

**The printed density has the powers of $Q$ and $a_p$ interchanged.** Its expression is too large by $Q/a_p$ in this limit. The normalized residence-time derivation fixes the corrected expression, which is also required for the later $Q^{1/2}$ ejection-time scaling. For a population of $N_c$ independent identical [comets](../../../../../../comet.md), multiply $\Sigma_c$ by $N_c$ to obtain a number [surface density of a disk](../../../../../../surface-density-of-a-disk.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
