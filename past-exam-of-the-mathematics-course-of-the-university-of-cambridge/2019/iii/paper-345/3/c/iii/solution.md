<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $a=6\alpha/5$ and $\lambda=R/B$, so that $B=aZ$ and $R=\lambda aZ$ with constant $\lambda\geq1$. The volume balance gives

$$
4\pi R^2\dot R=\pi B^2(w_p-U),\qquad \dot R=\lambda aU.
$$

Consequently

$$
\boxed{\frac U{w_p}=\frac1{1+4a\lambda^3}=\frac5{5+24\alpha\lambda^3}.}
$$

For the definition of $C_t$ printed in the question, using $g_p$ in its denominator, the [starting-plume thermal Froude-number ratio](../../../../../../../starting-plume-thermal-froude-number-ratio.md) is

$$
\boxed{\frac{C_t}{C_p}=\frac{U/\sqrt{g_pR}}{w_p/\sqrt{g_pB}}
=\frac5{\sqrt\lambda(5+24\alpha\lambda^3)}.}
$$

All factors are constant in the [self-similar starting plume](../../../../../../../self-similar-starting-plume.md). This expression decreases strictly with $\lambda>0$, giving

$$
\boxed{\frac{C_t}{C_p}\leq\frac5{5+24\alpha}=\frac{15}{15+72\alpha},\qquad \lambda\geq1.}
$$

The stronger bound requested in the PDF does not follow from its stated definition and $R\geq B$. For example, $\lambda=1$ already contradicts that bound. If instead the thermal [Froude number](../../../../../../../froude-number.md) is normalized by its own [reduced gravity](../../../../../../../reduced-gravity-split.md), $\widetilde C_t=U/\sqrt{g_tR}$, the preceding result $g_t=9g_p/4$ supplies the missing factor $2/3$:

$$
\boxed{\frac{\widetilde C_t}{C_p}=\frac{10}{\sqrt\lambda(15+72\alpha\lambda^3)}
\leq\frac{10}{15+72\alpha}.}
$$

The inequality is strict for $R>B$, with equality allowed by the stated endpoint $R=B$. This alternative normalization recovers the numerical bound while keeping the distinction between the plume and thermal [reduced gravities](../../../../../../../reduced-gravity-split.md) explicit.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 345](../../../../paper-345-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
