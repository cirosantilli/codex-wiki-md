<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $w(x)$ be the downward velocity between the vertical plates. A steady vertical momentum balance gives

$$
\frac{d\tau_{xz}}{dx}=-\rho g.
$$

Symmetry requires $\tau_{xz}(0)=0$, so the stress magnitude is

$$
|\tau_{xz}(x)|=\rho g|x|.
$$

The wall stress first reaches the yield stress when $\rho gl_c=\tau_y$. The onset measurement therefore gives

$$
\boxed{\tau_y=\rho gl_c}.
$$

For $l>l_c$, define $\Delta=l-l_c$. The central region $|x|\leq l_c$ is a [plug flow of a yield-stress fluid](../../../../../../plug-flow-of-a-yield-stress-fluid.md), while the layers $l_c<|x|\leq l$ are yielded. The [Herschel–Bulkley fluid](../../../../../../herschel-bulkley-fluid.md) law gives, for $x\geq l_c$,

$$
\left|w'(x)\right|
=\left[\frac{\rho g(x-l_c)}K\right]^{1/n}.
$$

Integrating from the no-slip wall $w(l)=0$ gives

$$
w(x)=\left(\frac{\rho g}{K}\right)^{1/n}
\frac{n}{n+1}
\left[\Delta^{1+1/n}-(x-l_c)^{1+1/n}\right]
$$

in the yielded layer, and the plug moves at

$$
w_p=\left(\frac{\rho g}{K}\right)^{1/n}
\frac{n}{n+1}\Delta^{1+1/n}.
$$

The [volumetric flow rate](../../../../../../volumetric-flow-rate.md) per unit span is consequently

$$
\boxed{
Q=2\left(\frac{\rho g}{K}\right)^{1/n}
\left[
\frac{n}{2n+1}\Delta^{2+1/n}
+\frac{nl_c}{n+1}\Delta^{1+1/n}
\right]}.
$$

Near onset, the plug term dominates and

$$
Q\sim(l-l_c)^{1+1/n}.
$$

The observed exponent two therefore corresponds to $n=1$, a linear post-yield constitutive law at small shear rate. Far above onset, the fully yielded contribution scales as

$$
Q\sim l^{2+1/n}.
$$

The observed exponent four corresponds to $n=1/2$, a shear-thinning square-root law at high shear rate.

A plausible stress curve is therefore odd in $\dot\gamma$, starts at the two yield-stress values $\tau=\pm\tau_y$, and has finite linear slope just after yield:

$$
\tau-\tau_y\sim K_1\dot\gamma
\qquad(\dot\gamma>0\text{ small}).
$$

It then crosses smoothly to the concave high-rate behavior

$$
\tau-\tau_y\sim K_2\dot\gamma^{1/2}
\qquad(\dot\gamma>0\text{ large}),
$$

with the negative-rate branch fixed by odd symmetry. This combines the two [power laws](../../../../../../power-law.md) inferred independently from the measured flux limits.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
