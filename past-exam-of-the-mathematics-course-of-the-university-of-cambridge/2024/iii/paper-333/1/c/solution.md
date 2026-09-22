<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce

$$
\tau=f_0t,
\qquad
X=\frac{f_0x}{V},
\qquad
Y=\frac{f_0y}{V},
\qquad
\epsilon=\widetilde\beta=\frac{\beta V}{f_0^2}.
$$

Because the speed is $V$, write

$$
\dot x=V\sin\phi,
\qquad
\dot y=V\cos\phi.
$$

The momentum equations give

$$
\frac{d\phi}{d\tau}=1+\epsilon Y,
\qquad
\frac{dX}{d\tau}=\sin\phi,
\qquad
\frac{dY}{d\tau}=\cos\phi.
$$

Use an [asymptotic expansion](../../../../../../asymptotic-expansion.md)

$$
\phi=\tau+\epsilon\phi_1+O(\epsilon^2),
\quad
X=X_0+\epsilon X_1+O(\epsilon^2),
\quad
Y=Y_0+\epsilon Y_1+O(\epsilon^2).
$$

The zeroth-order [inertial oscillation](../../../../../../inertial-oscillation.md) is

$$
X_0=1-\cos\tau,
\qquad
Y_0=\sin\tau.
$$

At first order,

$$
\phi_1'=\sin\tau,
\qquad
\phi_1=1-\cos\tau,
$$

and integration with the initial conditions gives

$$
X_1=\sin\tau-\frac14\sin2\tau-\frac12\tau,
$$



$$
Y_1=\cos\tau-1+\frac12\sin^2\tau.
$$

Therefore

$$
\boxed{
x(t)=\frac V{f_0}
\left[
1-\cos\tau
+\widetilde\beta
\left(\sin\tau-\frac14\sin2\tau-\frac12\tau\right)
\right]
+O(\widetilde\beta^2)},
$$



$$
\boxed{
y(t)=\frac V{f_0}
\left[
\sin\tau
+\widetilde\beta
\left(\cos\tau-1+\frac12\sin^2\tau\right)
\right]
+O(\widetilde\beta^2)}.
$$

The periodic terms describe a slightly distorted clockwise circle. The secular term in $x$ is a westward drift with velocity

$$
\boxed{
U_{\rm drift}=-\frac{\beta V^2}{2f_0^2}}.
$$

This [beta drift of an inertial oscillation](../../../../../../beta-drift-of-an-inertial-oscillation.md) occurs because the [Coriolis parameter](../../../../../../coriolis-parameter.md), and hence the turning rate, is larger on the poleward half of the orbit than on its equatorward half. A trajectory sketch therefore consists of clockwise loops whose centers move steadily westward; the parcel starts at the westernmost point of its first loop and initially travels northward.

<a id="1/c/image-westward-beta-drift-of-inertial-loops"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-333-beta-drift.png)

**[Figure 1](#1/c/image-westward-beta-drift-of-inertial-loops). Westward beta drift of inertial loops**. The first-order beta-plane trajectory forms slightly distorted clockwise loops. Their centers follow the dashed westward path because the Coriolis turning rate is stronger on the poleward side.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
