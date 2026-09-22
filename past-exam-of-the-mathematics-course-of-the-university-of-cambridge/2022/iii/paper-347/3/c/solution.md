<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The swept shell has $M_s=Ar$, where $A=2f_{\rm gas}\sigma^2/G$. Its steady radial [thin-shell momentum equation](../../../../../../thin-shell-momentum-equation.md) is

$$
v\frac d{dr}(Arv)=F_{\rm rad}-\frac{4f_{\rm gas}\sigma^4}{G}.
$$

Let $r_0$ be the launch radius and impose $v(r_0)=0$.

In the single-scattering regime, define

$$
\Gamma_{\rm ss}=\frac{L}{L_{\rm crit,s.s.}}>1.
$$

The force difference is constant, and integration gives

$$
\boxed{v_{\rm ss}^2(r)=2\sigma^2(\Gamma_{\rm ss}-1)
\left[1-\left(\frac{r_0}r\right)^2\right].}
$$

The shell accelerates monotonically, but continuous sweeping of $M_s\propto r$ makes the speed approach the finite maximum

$$
\boxed{v_{\rm ss,max}=v_{\rm ss}(\infty)
=\sqrt2\sigma\sqrt{\Gamma_{\rm ss}-1}.}
$$

For the optically thin ultraviolet regime, define the launch Eddington factor

$$
\Gamma_{\rm UV}=\frac{L}{L_{\rm crit,UV}(r_0)}>1.
$$

Since $F_{\rm rad}=\tau_{\rm UV}L/c\propto r^{-1}$ while the shell's gravitational force is constant, integration gives

$$
\boxed{v_{\rm UV}^2(r)=2\sigma^2\left[
2\Gamma_{\rm UV}\frac{r_0}r-1
+(1-2\Gamma_{\rm UV})\left(\frac{r_0}r\right)^2
\right].}
$$

It initially accelerates, reaches its maximum at

$$
\boxed{r_{\max}=r_0\left(2-\Gamma_{\rm UV}^{-1}\right),
\qquad
v_{\max}=\sqrt2\sigma
\frac{\Gamma_{\rm UV}-1}{\sqrt{2\Gamma_{\rm UV}-1}},}
$$

and then decelerates, formally stalling at $r=r_0(2\Gamma_{\rm UV}-1)$. The contrast is physical: single-scattering transfers the same $L/c$ to the shell at every radius, whereas an ultraviolet-thin shell intercepts a fraction proportional to its declining optical depth, so the isothermal host's gravity eventually wins.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
