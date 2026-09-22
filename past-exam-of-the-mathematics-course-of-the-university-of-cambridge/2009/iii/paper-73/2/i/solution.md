<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $X(t)$ denote the polymer–oil material interface, measured from the injection well, and let $U(t)$ be the [Darcy velocity](../../../../../../darcy-velocity.md). [Incompressibility](../../../../../../incompressible-flow.md) and uniform cross-sectional area make $U$ independent of $x$ in this planar model. Integrating [Darcy's law](../../../../../../darcy-law.md) through the injected layer and the oil layer gives

$$
\Delta P=\frac{U}{k}\left[\mu X+\mu_h(L-X)\right].
$$

The material interface moves at the [pore velocity](../../../../../../pore-velocity.md), so $X'=U/\phi$. Put $a=\mu-\mu_h$ and $A=\mu_hL$. Then $(A+aX)X'=k\Delta P/\phi$, which integrates from $X(0)=0$ to

$$
AX+\frac a2X^2=\frac{k\Delta P}{\phi}t.
$$

Thus the [fixed-pressure planar Darcy displacement](../../../../../../fixed-pressure-planar-darcy-displacement.md) has

$$
\boxed{\dot X(t)=\frac{k\Delta P}{\phi\sqrt{(\mu_hL)^2+2(\mu-\mu_h)k\Delta P\,t/\phi}},\qquad U(t)=\phi\dot X(t).}
$$

For $a\ne0$, $X=[\sqrt{A^2+2ak\Delta P\,t/\phi}-A]/a$; its continuous $a=0$ limit is $X=k\Delta P\,t/(\phi\mu_hL)$. Positive layer [dynamic viscosities](../../../../../../dynamic-viscosity.md) ensure the resistance stays positive until breakthrough, which occurs at $t_b=\phi L^2(\mu+\mu_h)/(2k\Delta P)$. The formulas stop there, since the two-layer geometry then changes.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
