<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $m,k,\gamma,F_0>0$ and $\omega>0$, and write $D_\omega=k-m\omega^2$ and $B_\omega=m\gamma\omega$. Substitution of $z=A\cos\omega t$ into the [forced harmonic oscillator](../../../../forced-harmonic-oscillator.md) equation gives

$$
A D_\omega\cos\omega t-A B_\omega\sin\omega t
=F_0\cos\phi_0\cos\omega t-F_0\sin\phi_0\sin\omega t.
$$

Equating the independent [sine](../../../../sine.md) and [cosine](../../../../cosine.md) coefficients yields

$$
\boxed{A D_\omega=F_0\cos\phi_0,\qquad A B_\omega=F_0\sin\phi_0.}
$$

Thus the required [phase matching for a displacement referenced driven oscillator](../../../../phase-matching-for-a-displacement-referenced-driven-oscillator.md) is

$$
\boxed{(k-m\omega^2)\sin\phi_0=m\gamma\omega\cos\phi_0.}
$$

For a positive [amplitude](../../../../wave-amplitude.md) $A$, one must also choose the correct quadrant: $\cos\phi_0=D_\omega/\sqrt{D_\omega^2+B_\omega^2}$ and $\sin\phi_0=B_\omega/\sqrt{D_\omega^2+B_\omega^2}$. Squaring and adding the coefficient equations gives

$$
\boxed{A=\frac{F_0}{\sqrt{(k-m\omega^2)^2+(m\gamma\omega)^2}}.}
$$

For arbitrary forcing [phase](../../../../phase-waves.md), the steady response is instead $z=A\cos(\omega t+\phi_0-\delta)$, where $\delta$ has the sine and cosine just specified. A change of time origin can put this displacement into $A\cos\omega t$, but it also changes the stated forcing [phase](../../../../phase-waves.md).

The source's requested parameter list for $A$ omits $\gamma$; in general it cannot be omitted. As a concrete counterexample, take $m=k=F_0=\omega=1$ and $\phi_0=\pi/2$. The prescribed cosine response exists for every $\gamma>0$, but $A=1/\gamma$, so fixing all four listed parameters does not fix the [amplitude](../../../../wave-amplitude.md). Likewise, with fixed $\phi_0=0$, positive damping and nonzero $\omega$, the second coefficient equation prevents a nonzero pure-cosine response. The forcing [phase](../../../../phase-waves.md) is an essential part of the condition.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
