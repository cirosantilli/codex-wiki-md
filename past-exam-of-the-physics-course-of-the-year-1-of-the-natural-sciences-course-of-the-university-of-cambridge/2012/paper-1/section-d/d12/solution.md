<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

Fixed endpoints require $k_n=n\pi/L$, with $n=1,2,\ldots$. Writing $c_s=\sqrt{T/\rho}$,

$$
\boxed{\omega_1=\frac{\pi c_s}{L},\qquad\omega_2=\frac{2\pi c_s}{L}.}
$$

For equal [amplitudes](../../../../../wave-amplitude.md) $A$, the two requested profiles are

$$
y(x,0)=A[\sin(\pi x/L)+\sin(2\pi x/L)],\qquad
y(x,t_1)=-A\sin(2\pi x/L).
$$

The first is asymmetric, with an interior zero at $x=2L/3$; the second has its interior [node](../../../../../node-dynamical-systems.md) at $L/2$. For [two-mode string recurrence](../../../../../two-mode-string-recurrence.md), [orthogonality](../../../../../orthogonal-vectors.md) means the whole initial profile recurs only when both [cosine](../../../../../cosine.md) coefficients equal one. Since $\omega_2=2\omega_1$,

$$
\boxed{t=\frac{2\pi n}{\omega_1},\qquad n=0,1,2,\ldots.}
$$

<a id="section-d/d12/image-two-mode-string-profiles-and-the-small-change-produced-by-weak-positive-dispersion-at-the-original-quarter-period"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1-ia2012-string-modes.png)

**[Figure 3](#section-d/d12/image-two-mode-string-profiles-and-the-small-change-produced-by-weak-positive-dispersion-at-the-original-quarter-period). Two-mode string profiles and the small change produced by weak positive dispersion at the original quarter-period**.

The [weak-stiffness string frequency shift](../../../../../weak-stiffness-string-frequency-shift.md) follows by expanding the supplied [dispersion relation](../../../../../dispersion-relation-split.md):

$$
\omega(k)=c_sk\left(1+\frac{\alpha k^2}{2c_s^2}\right)+O(\alpha^2),\qquad [\alpha]=\mathrm{m^4\,s^{-2}}.
$$

Higher [normal modes](../../../../../normal-mode.md) acquire larger fractional [frequency](../../../../../frequency.md) shifts. Let $\eta=\alpha k_1^2/c_s^2\ll1$ and retain $\omega_1^{(0)}=c_sk_1$ for the original ideal [frequency](../../../../../frequency.md). At the originally defined time $t_1=\pi/(2\omega_1^{(0)})$,

$$
\cos(\omega_1t_1)=-\frac{\pi\eta}{4}+O(\eta^2),\qquad
\cos(\omega_2t_1)=-1+O(\eta^2).
$$

Thus the $t=0$ sketch is unchanged, whereas the original quarter-period sketch gains a small negative fundamental component. If $t_1$ is redefined using the new fundamental [frequency](../../../../../frequency.md), its fundamental component is exactly zero and the second-mode change there is only second order. Both conventions agree that generic later shapes change because of relative [phase](../../../../../phase-waves.md) drift.

The new [frequency](../../../../../frequency.md) ratio is

$$
r=\frac{\omega_2}{\omega_1}=2\sqrt{\frac{1+4\eta}{1+\eta}}=2+3\eta+O(\eta^2).
$$

An exact recurrence now requires $\omega_1t=2\pi q$ and $\omega_2t=2\pi p$ for integers $p,q$. **If $r=p/q$ in lowest terms, the first recurrence is $2\pi q/\omega_1$; for irrational $r$ there is no exact finite recurrence.** Near-recurrences remain possible. Positive stiffness alone does not prove that the ratio is irrational.

## ↑ Ancestors (13)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
