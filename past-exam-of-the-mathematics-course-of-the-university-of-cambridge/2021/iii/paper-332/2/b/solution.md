<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Measure $z$ upward from the heat exchanger and let the steady ice front be at $z=h>0$. In the exchanger frame, salt in the liquid satisfies the [advection-diffusion equation](../../../../../../advection-diffusion-equation.md)

$$
-VC_z=DC_{zz}.
$$

The decaying solution and the prescribed total salt mass are

$$
C(z)=C_i e^{-V(z-h)/D},
\qquad
S=\rho\int_h^\infty C(z)\,dz,
$$

so

$$
\boxed{C_i=\frac{SV}{\rho D}}.
$$

The linear [liquidus](../../../../../../liquidus.md) condition fixes the interface temperature as

$$
\boxed{T_i=T_m-mC_i=T_m-\frac{mSV}{\rho D}}.
$$

A solid layer between the exchanger and the interface can therefore exist only if

$$
\boxed{T_c<T_m-\frac{mSV}{\rho D}}.
$$

Write $\vartheta=T-T_\infty$. Heat advection, conduction, and environmental loss give

$$
\vartheta''+\frac V\kappa\vartheta'-\frac Fk\vartheta=0.
$$

Its characteristic exponents are

$$
r_\pm=-\frac{V}{2\kappa}
\pm\sqrt{\frac{V^2}{4\kappa^2}+\frac Fk},
\qquad r_+>0>r_-.
$$

Below the exchanger and above the ice front, boundedness gives

$$
T_-(z)=T_\infty+(T_c-T_\infty)e^{r_+z}
\quad(z<0),
$$



$$
T_l(z)=T_\infty+(T_i-T_\infty)e^{r_-(z-h)}
\quad(z>h).
$$

In $0<z<h$, the ice temperature is

$$
T_+(z)=T_\infty+A e^{r_+z}+B e^{r_-z},
$$

where

$$
A+B=T_c-T_\infty,
\qquad
Ae^{r_+h}+Be^{r_-h}=T_i-T_\infty.
$$

Substitution of these fields into the [Stefan condition](../../../../../../stefan-condition.md)

$$
k[T_+'(h)-T_l'(h)]=\rho LV
$$

gives one scalar equation for the steady height $h$, which can be solved numerically. The heat flux may jump at $z=0$ because the exchanger supplies the required localized cooling.

The local equilibrium freezing temperature ahead of the front is

$$
T_L(z)=T_m-mC(z).
$$

Because $T_l(h)=T_L(h)$, [constitutional supercooling](../../../../../../constitutional-supercooling.md) begins when the actual liquid-temperature gradient at the interface is smaller than the liquidus gradient:

$$
T_l'(h)<T_L'(h).
$$

Using the solutions above, this is

$$
\boxed{
q\left(T_\infty-T_m+\frac{mSV}{\rho D}\right)
<\frac{mSV^2}{\rho D^2}},
\qquad
q=-r_-=\frac{V}{2\kappa}
+\sqrt{\frac{V^2}{4\kappa^2}+\frac Fk}.
$$

At criticality the inequality is an equality. If $F/k\ll V^2/\kappa^2$, then $q\sim V/\kappa$ and, for $\kappa>D$,

$$
\boxed{
V_c\sim\frac{\rho D^2(T_\infty-T_m)}
{mS(\kappa-D)}}.
$$

The critical curve is proportional to $S^{-1}$. If $F/k\gg V^2/\kappa^2$, put $q\sim\sqrt{F/k}$ to obtain

$$
\boxed{
V_c\sim\frac D2
\left[q+\sqrt{q^2+\frac{4q\rho(T_\infty-T_m)}{mS}}\right]}.
$$

This curve behaves as $S^{-1/2}$ for small $S$ and approaches $D\sqrt{F/k}$ for large $S$. Supercooling occurs above the corresponding critical curve, where solute rejection steepens the liquidus faster than heat transport raises the actual temperature.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
