<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The initial data and $\ddot u=0$ give $u=\tau$. To first order in $\epsilon$, replace $x$ and $y$ on the right-hand sides of the transverse equations by $x_0$ and $y_0$. Twice integrating with the initial rest conditions gives

$$
\boxed{x(\tau)=x_0+\epsilon y_0
\int_{-\infty}^{\tau}(\tau-s)a(s)\,ds+O(\epsilon^2)},
$$



$$
\boxed{y(\tau)=y_0+\epsilon x_0
\int_{-\infty}^{\tau}(\tau-s)a(s)\,ds+O(\epsilon^2)}.
$$

For $\tau>U$, define $A_0=\int_{-\infty}^{\infty}a(s)\,ds$ and $A_1=\int_{-\infty}^{\infty}s,a(s)\,ds$. Then

$$
x=x_0-\epsilon y_0A_1+\tau\epsilon y_0A_0,
\qquad
y=y_0-\epsilon x_0A_1+\tau\epsilon x_0A_0.
$$

Hence

$$
\boxed{\delta x=-\epsilon y_0A_1,
\quad\delta v_x=\epsilon y_0A_0,
\quad\delta y=-\epsilon x_0A_1,
\quad\delta v_y=\epsilon x_0A_0}.
$$

These permanent changes are forms of [displacement memory](../../../../../../../displacement-memory.md) and [velocity memory](../../../../../../../velocity-memory.md).

There is a discrepancy in the question's final instruction. The longitudinal equation actually gives

$$
\ddot z=\epsilon x_0y_0a'(\tau)+O(\epsilon^2),
$$

and therefore

$$
\boxed{\dot z=\epsilon x_0y_0a(\tau)+O(\epsilon^2),
\qquad
z=\epsilon x_0y_0\int_{-\infty}^{\tau}a(s)\,ds+O(\epsilon^2)}.
$$

Thus $z$ does not vanish to first order for a general allowed profile. It vanishes after the pulse under the additional hypothesis $A_0=0$ used in part (iv), but it need not vanish while that pulse is passing. The [proper-time normalization](../../../../../../../proper-time-normalization.md) independently gives the same relation $\dot z=xyA+O(\epsilon^2)$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
