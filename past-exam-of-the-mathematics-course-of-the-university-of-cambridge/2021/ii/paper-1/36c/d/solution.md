<h1 id="36c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the $(p,V)$ plane, the [Otto cycle](../../../../../../otto-cycle.md) consists of:

- $A\to B$: an adiabatic compression along $pV^\gamma=\text{constant}$ from $V_1$ to $V_2$;
- $B\to C$: a vertical constant-volume rise at $V_2$;
- $C\to D$: an adiabatic expansion back to $V_1$;
- $D\to A$: a vertical constant-volume fall at $V_1$.

It is a clockwise loop, so its enclosed area is the positive net work output. In the $(T,S)$ plane, the two reversible adiabats $A\to B$ and $C\to D$ are vertical constant-entropy segments. Constant-volume heating $B\to C$ moves upward and to the right, while constant-volume cooling $D\to A$ moves downward and to the left.

Let

$$
r=\frac{V_1}{V_2}>1.
$$

The two adiabatic relations give

$$
T_B=T_A r^{\gamma-1},
\qquad
T_C=T_D r^{\gamma-1}.
$$

Because heat is exchanged at constant volume,

$$
Q_1=C_V(T_C-T_B),
\qquad
Q_2=C_V(T_D-T_A),
$$

where $Q_2$ denotes the positive amount rejected. Hence

$$
\begin{aligned}
\frac{Q_2}{Q_1}
&=\frac{T_C/r^{\gamma-1}-T_A}
{T_C-T_A r^{\gamma-1}}\\
&=\frac1{r^{\gamma-1}}.
\end{aligned}
$$

The [thermal efficiency](../../../../../../thermal-efficiency.md) is therefore

$$
\boxed{
\eta=\frac W{Q_1}
=1-\frac{Q_2}{Q_1}
=1-\frac1{r^{\gamma-1}}}.
$$

For a fixed gas, $\gamma$ is fixed and the idealized efficiency increases monotonically with the compression ratio $r$, so it is maximized by making $r$ as large as the physical constraints allow.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [36C](../../36c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
