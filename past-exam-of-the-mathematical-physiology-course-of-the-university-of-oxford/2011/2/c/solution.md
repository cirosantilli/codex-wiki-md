<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

During ejection the [mitral valve](../../../../mitral-valve.md) is closed, so $Q_v=0$. Adding the arterial and ventricular balances cancels aortic flow:

$$
R_cC_a\dot p_a+R_c\frac{d}{dt}(p_{LV}/E_{LV})=-(p_a-p_v)\simeq-p_a,
$$

where the last approximation assumes $p_v\ll p_a$.

Model the rapid contraction as a switch to approximately constant systolic elastance $E_S$, with $C_s=1/E_S$ the systolic ventricular compliance. A sufficiently small aortic-valve resistance makes $p_{LV}\simeq p_a$ after a short [pressure](../../../../pressure-split.md)-equalization transient. The systolic pressure must be high enough to open the valve, $E_S(V^+-V_0)>p_a^+$. During that transient neglect systemic runoff. Conservation of combined arterial and stressed ventricular volume gives

$$
C_ap_a^++V^+-V_0=(C_a+C_s)\widehat p_a,
$$

so

$$
\boxed{\widehat p_a\simeq\frac{C_ap_a^++V^+-V_0}{C_a+C_s}.}
$$

This is an approximation across a rapid transient, not a discontinuity at finite valve resistance. The subsequent common [pressure](../../../../pressure-split.md) obeys $R_c(C_a+C_s)\dot p_a\simeq-p_a$, giving

$$
\boxed{p_a(t)\simeq\widehat p_a\exp\left[-\frac{t}{R_c(C_a+C_s)}\right].}
$$

The source's $R_C$ in this expression denotes the same systemic resistance $R_c$.

At the end of firing, the remaining ventricular volume is $V_{\mathrm{end}}\simeq V_0+C_sp_a(\Delta t_F)$. The [stroke volume](../../../../stroke-volume.md) is $V^+-V_{\mathrm{end}}$, hence

$$
\boxed{\mathrm{SV}\simeq V^+-V_0-\frac{C_s}{C_a+C_s}(C_ap_a^++V^+-V_0)\exp\left[-\frac{\Delta t_F}{R_c(C_a+C_s)}\right].}
$$

The assumptions are a closed [mitral valve](../../../../mitral-valve.md) throughout ejection, negligible venous [pressure](../../../../pressure-split.md), rapid valve equalization relative to systemic runoff, and nearly constant systolic elastance during the interval measured by $\Delta t_F$. These give the [ventricular ejection pressure and stroke-volume approximation](../../../../ventricular-ejection-pressure-and-stroke-volume-approximation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
