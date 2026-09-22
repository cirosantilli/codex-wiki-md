<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

The [microcanonical ensemble](../../../../../microcanonical-ensemble.md) assigns equal [probability](../../../../../probability.md) to accessible quantum states in a narrow [energy](../../../../../energy.md) shell of an isolated system with fixed [energy](../../../../../energy.md), particle number and external parameters. To derive the [canonical ensemble](../../../../../canonical-ensemble.md), put a small system in weak thermal contact with a much larger isolated bath. If the small-system state has [energy](../../../../../energy.md) $E_i$, its [probability](../../../../../probability.md) is proportional to the number $\Omega_b(E_{\rm total}-E_i)$ of bath states. Expanding the bath [entropy](../../../../../entropy.md) gives $S_b(E_{\rm total}-E_i)=S_b(E_{\rm total})-E_i/T+\cdots$, since $\partial S_b/\partial E=1/T$. Negligible interaction [energy](../../../../../energy.md) and an effectively constant bath temperature therefore give $p_i=e^{-E_i/(k_BT)}/Z$. The [microcanonical ensemble](../../../../../microcanonical-ensemble.md) suits an isolated fixed-energy system; the [canonical ensemble](../../../../../canonical-ensemble.md) suits a system exchanging [energy](../../../../../energy.md) with a thermostat at fixed temperature, with particle number still fixed.

For one atom, summing the finite geometric [series](../../../../../series-mathematics.md) over $m=-J,\ldots,J$ gives the [partition function](../../../../../canonical-partition-function.md)

$$
\boxed{Z_1=\sum_{m=-J}^Je^{xm}=\frac{\sinh((J+1/2)x)}{\sinh(x/2)},\qquad x=\frac{\mu_BB}{k_BT}}.
$$

At $x=0$ the ratio is understood by [continuity](../../../../../continuous-function.md) as $2J+1$. Logarithmic differentiation gives the mean [magnetic dipole moment](../../../../../magnetic-dipole-moment.md)

$$
\boxed{\langle\mu_z\rangle=\mu_B\left[(J+\tfrac12)\coth((J+\tfrac12)x)-\tfrac12\coth(x/2)\right]}.
$$

This is odd in $x$, has small-$x$ expansion $\mu_BJ(J+1)x/3+O(x^3)$, and saturates at $\pm J\mu_B$. The requested common graph is plotted in units of $\mu_B$: its ordinate is $\langle\mu_z\rangle/(J\mu_B)$, so multiplication by $\mu_B$ gives $\langle\mu_z\rangle/J$. The normalized slopes at zero are $(J+1)/3$ and the limits are $\pm1$.

<a id="34d/image-magnetization-as-a-function-of-field-and-temperature"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1-magnetization.png)

**[Figure 2](#34d/image-magnetization-as-a-function-of-field-and-temperature). Magnetization as a function of field and temperature**.

The [magnetic susceptibility](../../../../../magnetic-susceptibility.md) is

$$
\boxed{\chi=\frac{N\mu_B^2}{k_BT}\left[\frac14\operatorname{csch}^2(x/2)-(J+\tfrac12)^2\operatorname{csch}^2((J+\tfrac12)x)\right]}.
$$

Equivalently it is $N\mu_B^2\operatorname{Var}(m)/(k_BT)\ge0$. For $k_BT\gg\mu_B|B|$, the apparent singular terms cancel, yielding [Curie law](../../../../../curie-s-law.md)

$$
\boxed{\chi\sim\frac{N\mu_B^2J(J+1)}{3k_BT}}.
$$

For fixed nonzero $B$, $T\to0$ and integer $J\ge1$, the first excited magnetic level is separated from the aligned [ground state](../../../../../ground-state.md) by $\mu_B|B|$. Its exponentially small occupation gives

$$
\boxed{\chi\sim\frac{N\mu_B^2}{k_BT}e^{-\mu_B|B|/(k_BT)}\longrightarrow0}.
$$

The moments are saturated, so changing the [magnetic field](../../../../../magnetic-field.md) hardly changes their alignment. This is a fixed-nonzero-field low-temperature limit. At exactly $B=0$, differentiating first gives the Curie expression for every $T>0$, which diverges as $T\to0$; the two limits do not commute in this noninteracting model. For $J=0$ both moment and susceptibility vanish identically.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
