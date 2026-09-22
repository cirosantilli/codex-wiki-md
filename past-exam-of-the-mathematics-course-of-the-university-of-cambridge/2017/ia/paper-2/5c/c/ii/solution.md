<h1 id="5c/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Every solution is the [resonant series RLC response](../../../../../../../resonant-series-rlc-response.md) $I_0(t)=R^{-1}\sin(\omega_0t)$ plus a solution of the homogeneous [damped harmonic oscillator](../../../../../../../damped-harmonic-oscillator.md). Define $\gamma=R/(2L)$ and $\omega_0^2=1/(LC)$. The three possibilities are

$$
\boxed{I(t)=\frac{\sin(\omega_0t)}R+
\begin{cases}
e^{-\gamma t}\bigl(A\cos(\Omega t)+B\sin(\Omega t)\bigr),
&\gamma<\omega_0,\quad\Omega=\sqrt{\omega_0^2-\gamma^2},\\
e^{-\gamma t}(A+Bt),&\gamma=\omega_0,\\
Ae^{(-\gamma+\kappa)t}+Be^{(-\gamma-\kappa)t},
&\gamma>\omega_0,\quad\kappa=\sqrt{\gamma^2-\omega_0^2}.
\end{cases}}
$$

These are respectively the [underdamped RLC response](../../../../../../../underdamped-rlc-response.md), [critically damped RLC response](../../../../../../../critically-damped-rlc-response.md) and [overdamped RLC response](../../../../../../../overdamped-rlc-response.md). Both exponents in the last case are negative because $0<\kappa<\gamma$. All three homogeneous contributions tend to zero as $t\to\infty$, so **every response approaches the unique periodic steady current $I_0(t)$.** No initial conditions were specified in this clause; they determine $A,B$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5C](../../../5c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
