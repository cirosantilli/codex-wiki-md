<h1 id="34d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The expansion about the [liquid-gas critical point](../../../../../../liquid-gas-critical-point.md) is

$$
\bar p=1+4t-6t\phi+9t\phi^2-\frac32\phi^3-\frac{27}{2}t\phi^3+O(\phi^4)+O(t\phi^4).
$$

Differentiating at fixed $t$ gives the requested $-9\phi^2/2+O(\phi^3)+t[-6+O(\phi)]$. At coexistence $\phi=O(\sqrt{-t})$, so to leading nontrivial order keep the cubic odd part $\bar p=1+4t-6t\phi-3\phi^3/2$.

Let $a=\phi_l$, $b=\phi_g$ for this leading cubic model. Equality of endpoint [pressures](../../../../../../pressure.md) gives $a^2+ab+b^2=-4t$. The Maxwell condition in [pressure](../../../../../../pressure.md) coordinates is $\int_a^b(1+\phi)\bar p'(\phi)\,d\phi=0$. Since the endpoint [pressures](../../../../../../pressure.md) agree, its first term vanishes, leaving

$$
(b^2-a^2)\left[-3t-\frac98(a^2+b^2)\right]=0.
$$

If $a+b\ne0$, these two equations would imply $(a-b)^2=0$, contrary to distinct phases. Therefore $a=-b$, and the [pressure](../../../../../../pressure.md) equality gives $a^2=b^2=-4t$. Hence

$$
\boxed{\phi_l=-2\sqrt{-t}+O(t),\qquad\phi_g=2\sqrt{-t}+O(t),\qquad
\bar v_g-\bar v_l\sim4\sqrt{\frac{T_c-T}{T_c}}.}
$$

Thus the coexistence gap has exponent one half. **The printed equality $\phi_l(t)=-\phi_g(t)$ is a leading-order statement, not an exact identity for the full [Van der Waals equation](../../../../../../van-der-waals-equation.md).** Discarded asymmetric terms shift both phase [volumes](../../../../../../volume.md) at higher order. This distinction is needed even though the leading cubic calculation has exact antisymmetry within its truncation.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [34D](../../34d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
