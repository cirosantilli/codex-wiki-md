<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $E(t)=-\delta A/\delta\mathbf x(t)$. For a specified forward trajectory, the equation of motion determines

$$
\mathbf f_F=E+\zeta\dot{\mathbf x},
$$

whereas its time reverse requires

$$
\mathbf f_B=E-\zeta\dot{\mathbf x}.
$$

Assume the action is invariant under [time-reversal symmetry](../../../../../../t-symmetry.md), the position is even and velocity is odd under time reversal, and the trajectory-to-noise Jacobian is identical in the two directions. The [Onsager--Machlup path probability](../../../../../../onsager-machlup-path-probability.md) is then

$$
\mathbb P_F[\mathbf x]
=\mathcal N\exp\left[-\frac1{2\sigma^2}
\int_{t_1}^{t_2}|E+\zeta\dot{\mathbf x}|^2dt\right],
$$

with $\zeta\dot{\mathbf x}$ replaced by $-\zeta\dot{\mathbf x}$ for $\mathbb P_B$. Since

$$
|E+\zeta\dot{\mathbf x}|^2-|E-\zeta\dot{\mathbf x}|^2
=4\zeta E\mathbin\cdot\dot{\mathbf x},
$$

their ratio is

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}
=\exp\left[\frac{2\zeta}{\sigma^2}
\int_{t_1}^{t_2}
\dot{\mathbf x}\mathbin\cdot
\frac{\delta A}{\delta\mathbf x(t)}dt\right].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
