<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Conditioned on $f$, the additive-noise trajectory has the [Onsager–Machlup functional](../../../../../../onsager-machlup-functional.md)

$$
P[x\mid f]\propto
\exp\left[
-\frac1{2C^2}\int_0^T
(\dot x+V'(x)-f)^2dt
\right].
$$

Under time reversal, $\dot x$ changes sign while $x$ and the active force $f$ are even. Subtracting the forward and backward conditional actions gives

$$
\log\frac{P_F[x\mid f]}{P_B[x\mid f]}
=\frac2{C^2}\left[
V(x_0)-V(x_T)
+\int_0^T\dot x\,f\,dt
\right].
$$

The corresponding ratio for an Ornstein–Uhlenbeck path conditioned on its initial endpoint is

$$
\log\frac{P_F[f]}{P_B[f]}
=\frac{\alpha}{c^2}
\left[f(0)^2-f(T)^2\right].
$$

Consequently

$$
\boxed{
\log\frac{P_F[f,x]}{P_B[f,x]}
=\Delta U[f,x]
+\frac2{C^2}\int_0^T\dot x(t)f(t)\,dt
},
$$

where

$$
\boxed{
\Delta U[f,x]
=\frac{\alpha}{c^2}[f(0)^2-f(T)^2]
+\frac2{C^2}[V(x_0)-V(x_T)]
}.
$$

If stationary endpoint densities are included in the path measures, their ratio cancels the Ornstein–Uhlenbeck boundary term; the displayed convention is the endpoint-conditioned path probability used in the calculation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
