<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Away from the first [parametric resonance](../../../../../../parametric-resonance.md), one forcing interaction changes a harmonic [frequency](../../../../../../frequency.md) by one and produces no resonant coupling of the two conjugate oscillations. Two interactions can couple [frequency](../../../../../../frequency.md) $+1$ to [frequency](../../../../../../frequency.md) $-1$, so the next [parametric resonance](../../../../../../parametric-resonance.md) is near $\omega=1$ and its effect first appears at order $\epsilon^2$. This gives **$p=2$** and the appropriate slow time $T=\epsilon^2t$.

Write $\omega=1+\kappa\epsilon^2$ and $y_0=a(T)\cos t+b(T)\sin t$. The first correction satisfies $(\partial_t^2+1)y_1=-\cos t\,y_0$, whose bounded particular solution is

$$
y_1=-\frac a2+\frac a6\cos2t+\frac b6\sin2t.
$$

At second order,

$$
(\partial_t^2+1)y_2=-2\partial_t\partial_Ty_0-2\kappa y_0-\cos t\,y_1.
$$

The resonant part of $-\cos t\,y_1$ is $(5a/12)\cos t-(b/12)\sin t$. Applying the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) gives

$$
\boxed{a_T=(\kappa+1/24)b,\qquad b_T=(5/24-\kappa)a.}
$$

The squared slow [eigenvalue](../../../../../../eigenvalue.md) is

$$
\lambda^2=(\kappa+1/24)(5/24-\kappa)
=\frac1{64}-(\kappa-1/12)^2.
$$

The [second instability tongue of a weak Mathieu oscillator](../../../../../../second-instability-tongue-of-a-weak-mathieu-oscillator.md) therefore has the leading interval

$$
\boxed{-\frac1{24}<\kappa<\frac5{24},\qquad
1-\frac{\epsilon^2}{24}+o(\epsilon^2)<\omega<1+\frac{5\epsilon^2}{24}+o(\epsilon^2).}
$$

Here the two little-$o$ terms describe the respective exact edge locations; the strict inequality in $\kappa$ is the leading interior criterion. In particular $\omega=1$ is unstable, with physical growth rate $\epsilon^2\sqrt5/24+o(\epsilon^2)$. The general leading solution for bounded $T$ again has $y_0=a(T)\cos t+b(T)\sin t$, where the [matrix exponential](../../../../../../matrix-exponential.md) of the displayed two-by-two [amplitude](../../../../../../wave-amplitude.md) system evolves arbitrary $a(0),b(0)$. Adding $\epsilon y_1$ identifies the first nonresonant harmonic correction. The leading expression alone has error $O(\epsilon)$ on $t=O(\epsilon^{-2})$.

For comparison, at fixed $\omega\ne1/2,1$, write $y_0=A(T)e^{i\omega t}+\overline A(T)e^{-i\omega t}$. The first forced harmonics have coefficients $A/[2(2\omega+1)]$ and $A/[2(1-2\omega)]$. Their return to the original harmonic at the next order gives

$$
A_T=\frac{i}{4\omega(1-4\omega^2)}A.
$$

It is a phase correction, not [amplitude](../../../../../../wave-amplitude.md) growth. Consequently, away from the first two resonance neighborhoods, a general leading solution valid for bounded $\epsilon^2t$ is

$$
y=C\cos(\Omega t)+D\sin(\Omega t)+O(\epsilon),\qquad
\Omega=\omega+\frac{\epsilon^2}{4\omega(1-4\omega^2)}.
$$

Narrower higher-order instability intervals are invisible on this time scale. The detuned resonant calculation above is needed near $\omega=1$ because both the phase shift and the conjugate-mode coupling then matter.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
