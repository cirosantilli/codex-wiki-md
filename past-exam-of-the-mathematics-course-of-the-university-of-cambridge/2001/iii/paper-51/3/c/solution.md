<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Along a perturbed saddle loop the incoming and outgoing endpoints have the same [Hamiltonian](../../../../../../hamiltonian.md) value. Integrating $H'=\varepsilon(\beta+u)v^2$ and evaluating the leading integral on the conservative [homoclinic orbit](../../../../../../homoclinic-orbit.md) gives

$$
0=\varepsilon(\beta I_0+I_1)+O(\varepsilon^2),\qquad
I_0=\int_{-\infty}^{\infty}v^2d\tau,\quad I_1=\int_{-\infty}^{\infty}uv^2d\tau.
$$

On the upper half of the loop $v_+(u)=\sqrt{2/3}(a-u)\sqrt{u+2a}$ and $d\tau=du/v_+$. The lower half makes an equal contribution, so

$$
\begin{aligned}
I_0&=2\sqrt{2/3}\int_0^{3a}(3a-s)s^{1/2}ds={24\sqrt2\over5}a^{5/2},\\
I_1&=2\sqrt{2/3}\int_0^{3a}(s-2a)(3a-s)s^{1/2}ds=-{24\sqrt2\over7}a^{7/2}.
\end{aligned}
$$

These [homoclinic integrals for a quadratic-force oscillator](../../../../../../homoclinic-integrals-for-a-quadratic-force-oscillator.md) give the simple first-order splitting zero $\beta=5a/7$, since $\partial_\beta(\beta I_0+I_1)=I_0>0$. The [Melnikov energy-balance method](../../../../../../melnikov-energy-balance-method.md) therefore yields **the leading global bifurcation curve**

$$
\boxed{\beta\sim{5\over7}\sqrt\alpha,\qquad\mu\sim{5\over7}\sqrt\lambda.}
$$

This is an asymptotic curve near the double-zero point, not an exact finite-parameter identity. More precisely, time reversal $(\tau,v,\varepsilon)\mapsto(-\tau,-v,-\varepsilon)$ preserves the loop condition. The smooth curve selected by its simple splitting zero is even in $\varepsilon$, giving $\beta=5\sqrt\alpha/7+O(\varepsilon^2)$ and hence $\mu=5\sqrt\lambda/7+O(\lambda)$ for fixed scaled $\alpha>0$.

Between the saddle-loop curve and $\mu=\sqrt\lambda$, a stable focus is surrounded by the repelling [periodic orbit](../../../../../../periodic-orbit.md) created at the [subcritical Hopf bifurcation](../../../../../../subcritical-hopf-bifurcation.md). As $\mu$ decreases, this orbit grows until it reaches the saddle. Below the saddle-loop curve there is a stable focus and a saddle, but no nearby cycle. Above the Hopf curve there is an unstable focus and a saddle, with no nearby cycle. At the global curve the saddle separatrices form the repelling loop. Under the stipulated absence of further bifurcations, these are the distinct nearby regions in the earlier sketch; no extra remote phase structure is being inferred from the leading-order calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
