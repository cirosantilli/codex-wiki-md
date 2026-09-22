<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

The [fixed points](../../../../../fixed-point.md) are $(0,0)$ and $(\pm1,1)$. The [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}1-y&-x\\2x&-1\end{pmatrix}.
$$

At the origin its [eigenvalues](../../../../../eigenvalue.md) are $1,-1$, so it is a saddle with stable direction the y-axis. At either other [fixed point](../../../../../fixed-point.md), the characteristic [polynomial](../../../../../polynomial-split.md) is $\lambda^2+\lambda+2$, giving [eigenvalues](../../../../../eigenvalue.md) $(-1\pm i\sqrt7)/2$. Thus both are stable foci. The [nullclines](../../../../../nullcline.md) are $x=0$, $y=1$ and $y=x^2$. In the right half-plane $x$ grows below $y=1$ and decreases above it; in the left half-plane these horizontal arrows reverse. Vertically, $y$ increases below $y=x^2$ and decreases above it.

A global argument determines the requested [omega-limit sets](../../../../../omega-limit-set.md), rather than guessing from the local [phase portrait](../../../../../phase-portrait.md). For $x\ne0$, use the [quadratic-logarithmic Lyapunov function for a feedback system](../../../../../quadratic-logarithmic-lyapunov-function-for-a-feedback-system.md)

$$
L=x^2-1-\log(x^2)+(y-1)^2,\qquad
\dot L=-2(y-1)^2.
$$

Its sublevel sets are [compact](../../../../../compact-space.md) and bounded away from $x=0$, so trajectories starting in either half-plane exist for all positive time and stay in such a set. Since $L$ decreases, it tends to a limit, and is constant on the [omega-limit set](../../../../../omega-limit-set.md). Every point of that set therefore has $y=1$. Invariance then requires $\dot y=x^2-1=0$, so only the corresponding focus can occur. Also $x(t)=x(0)\exp(\int_0^t(1-y(s))\,ds)$ preserves its sign.

Consequently

$$
\boxed{\omega(2,-1)=\{(1,1)\},\qquad
\omega(x,y)=\{(0,0)\}\ \Longleftrightarrow\ x=0}.
$$

On $x=0$, the exact solution is $y(t)=y(0)e^{-t}$. The [phase portrait](../../../../../phase-portrait.md) below shows this stable axis, the [nullclines](../../../../../nullcline.md) and the spiral attraction in each half-plane.

<a id="7b/image-phase-portrait-with-a-saddle-at-the-origin-and-stable-foci-at-plus-or-minus-one-one"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4-phase-plane.png)

**[Figure 1](#7b/image-phase-portrait-with-a-saddle-at-the-origin-and-stable-foci-at-plus-or-minus-one-one). Phase portrait with a saddle at the origin and stable foci at plus or minus one, one**.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
