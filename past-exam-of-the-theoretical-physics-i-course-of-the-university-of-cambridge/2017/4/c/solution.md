<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Substitute $\omega=\alpha_3/\varepsilon+\cdots$ into the cubic denominator. Its leading terms are

$$
1-\omega^2-i\varepsilon\omega^3
=-\frac{\alpha_3^2+i\alpha_3^3}{\varepsilon^2}+O(1).
$$

The nonzero large root obeys $1+i\alpha_3=0$, so

$$
\boxed{\alpha_3=i,\qquad\omega_3\simeq\frac i\varepsilon}.
$$

The sum of the three roots is exactly $i/\varepsilon$. Combining this with the two slow-root expansions gives the refinement $\omega_3=i/\varepsilon+i\varepsilon+O(\varepsilon^3)$.

For physical radiative sign $\varepsilon>0$, the fast [pole](../../../../pole.md) lies high in the upper half-plane. Its homogeneous mode is $e^{-i\omega_3t}\simeq e^{t/\varepsilon}$, a runaway. It prevents a **bounded retarded response with the real-axis Fourier prescription** even though the two slow poles are damped. If $\varepsilon<0$, the fast [pole](../../../../pole.md) decays but the slow pair grow. No nonzero real sign puts every [pole](../../../../pole.md) in the lower half-plane.

There are two distinct boundary choices. A strictly causal initial-value [Green function](../../../../green-s-function-split.md) exists and includes the growing mode for $\varepsilon>0$; it must be represented by a Laplace/[Bromwich contour](../../../../bromwich-contour.md) above that [pole](../../../../pole.md) rather than the stated ordinary Fourier integral. Alternatively the real-axis inverse gives a bounded [stationary no-runaway response and preacceleration](../../../../stationary-no-runaway-response-and-preacceleration.md): for $\tau<0$, upper closure encloses the fast [pole](../../../../pole.md) and yields a nonzero response before the [force](../../../../force-split.md). Its leading contribution is

$$
G(\tau)\simeq\varepsilon e^{\tau/\varepsilon},\qquad \tau<0,\quad\varepsilon>0.
$$

This follows from the upper-pole [residue](../../../../residue.md) $\operatorname{Res}G\simeq-i\varepsilon$ and the factor $i$ from upper contour closure. Eliminating runaway growth by a future [boundary condition](../../../../boundary-condition.md) therefore sacrifices strict retardation on the short scale $\varepsilon$.

The singular root also shows why a perturbative expansion around only $\omega=\pm1$ misses the problem. For a low-frequency effective description, [order reduction of a radiation-reaction oscillator](../../../../order-reduction-of-a-radiation-reaction-oscillator.md) uses $\dddot x\simeq\dot f-\dot x$ in the small correction and gives $\ddot x+\varepsilon\dot x+x=f+\varepsilon\dot f$. For positive $\varepsilon$ this approximate second-order equation has a causal damped response and discards the fast mode outside its intended regime; it does not make the original third-order equation simultaneously bounded and retarded.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
