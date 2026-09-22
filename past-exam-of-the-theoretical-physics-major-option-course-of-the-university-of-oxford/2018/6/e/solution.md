<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take $a=a_0(T-T_c)$ and hold $b,c$ fixed. The [heat capacity](../../../../heat-capacity.md) comes from the minimized [free energy](../../../../thermodynamic-free-energy.md), $C=-T\,d^2F_{\min}/dT^2$, with any smooth background added separately. For $b>0$ and $T<T_c$,

$$
F_{\min}-F_{\mathrm{reg}}=-\frac{a^2}{4b}+O(a^3),\qquad
C_{\mathrm{sing},-}=\frac{T a_0^2}{2b}+O(T_c-T).
$$

Above $T_c$, $m=0$ and the polynomial contributes zero. There is a finite jump, rather than a divergence: the conventional ordinary [mean-field critical exponents](../../../../mean-field-critical-exponent.md) are

$$
\boxed{\alpha_-=\alpha_+=0\quad(b>0),\qquad \Delta C=\frac{T_ca_0^2}{2b}.}
$$

The upper branch has zero order-parameter contribution; a finite regular [heat capacity](../../../../heat-capacity.md) has exponent zero.

Along the tuned tricritical path $b=0$, the ordered minimum gives

$$
F_{\min}-F_{\mathrm{reg}}=-\frac{(-a)^{3/2}}{3\sqrt c},\qquad
\boxed{C_{\mathrm{sing},-}=\frac{T a_0^2}{4\sqrt c\sqrt{-a}}
=\frac{T a_0^{3/2}}{4\sqrt c}(T_c-T)^{-1/2},\quad \alpha_-^{\mathrm{tri}}=\frac12.}
$$

**Upper-side qualification:** the [vanishing disordered-side heat-capacity amplitude in Landau theory](../../../../vanishing-disordered-side-heat-capacity-amplitude-in-landau-theory.md) matters here: for $b=0$ and $a>0$, the minimizing solution is still exactly $m=0$, so this saddle-point polynomial gives $F_{\min}-F_{\mathrm{reg}}=0$ and $C_{\mathrm{sing},+}=0$. A zero function cannot determine a nonzero-amplitude power-law exponent. For example, adding the allowed smooth background $F_{\mathrm{reg}}=-C_0T\log(T/T_*)$, with $C_0>0$, leaves the entire [phase diagram](../../../../phase-diagram.md) unchanged but makes the upper-side [heat capacity](../../../../heat-capacity.md) exactly $C_0$, not a $(T-T_c)^{-1/2}$ divergence.

One convention assigns the tricritical scaling exponent $\alpha=1/2$ to both sides, writing $C_{\mathrm{sing},\pm}=A_\pm|T-T_c|^{-1/2}$ with $A_+=0$ at this [mean-field approximation](../../../../mean-field-approximation.md) saddle. If the source's literal $C\sim|T-T_c|^{-\alpha_+}$ is meant to have a nonzero leading coefficient, the given polynomial establishes **no upper-side tricritical singular exponent**; with a nonzero smooth background its leading upper-side exponent is zero. A nonzero upper-side singularity requires fluctuation information beyond this minimization. This distinction prevents claiming an upper-side divergence that the displayed [Landau free energy](../../../../landau-free-energy.md) does not produce.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
