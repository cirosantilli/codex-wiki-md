<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Cartesian streamfunction](../../../../../cartesian-streamfunction.md) convention $u_x=\partial_y\Psi$, $u_y=-\partial_x\Psi$. In the creeping-flow regime implicit in the question's [biharmonic equation](../../../../../biharmonic-equation.md) hint, the [Stokes equations](../../../../../stokes-equation.md) are $\mu\nabla^2\mathbf u=\nabla p$, $\nabla\cdot\mathbf u=0$. Taking their curl eliminates pressure and gives

$$
\boxed{\nabla^4\Psi=0.}
$$

The fluid occupies the region above the actual sheet; the perturbation calculation expands its boundary about $y=0$. In the swimming frame the material velocity is $(0,-\omega y_0\cos(kx-\omega t))$. The vertical kinematic condition and the supplied [Navier slip boundary condition](../../../../../navier-slip-boundary-condition.md) therefore give, at $y=y_0\sin(kx-\omega t)$,

$$
\Psi_x=\omega y_0\cos(kx-\omega t),\qquad
\Psi_y=\gamma(\Psi_{yy}-\Psi_{xx}).
$$

At infinity, $\Psi_y\to U$ and $\Psi_x\to0$, with bounded velocity and no imposed shear; all fields are periodic in $x$ with period $2\pi/k$. The sign is important: a sheet translating at $-U\mathbf e_x$ sees the remote fluid translating at $+U\mathbf e_x$.

Set $X=kx$, $Y=ky$, $\tau=\omega t$, $\psi=k^2\Psi/\omega$, and $U^*=kU/\omega$. The two dimensionless parameters are the small-slope approximation parameter $\epsilon=ky_0$ and dimensionless [slip length](../../../../../slip-length.md) $\delta=k\gamma$. With $\theta=X-\tau$, the dimensionless [biharmonic stream function for planar Stokes flow](../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) satisfies

$$
\begin{aligned}
(\partial_X^2+\partial_Y^2)^2\psi&=0,\\
\psi_X&=\epsilon\cos\theta,\qquad
\psi_Y=\delta(\psi_{YY}-\psi_{XX})
&&\text{at }Y=\epsilon\sin\theta,\\
\psi_Y&\longrightarrow U^*,\qquad\psi_X\longrightarrow0
&&\text{as }Y\longrightarrow\infty.
\end{aligned}
$$

Expand $\psi=\epsilon\psi_1+\epsilon^2\psi_2+\cdots$ and $U^*=\epsilon U_1+\epsilon^2U_2+\cdots$. At first order,

$$
(\psi_1)_X(X,0,\tau)=\cos\theta,\qquad
(\psi_1)_Y(X,0,\tau)
=\delta[(\psi_1)_{YY}-(\psi_1)_{XX}](X,0,\tau).
$$

The decaying first harmonic of the [biharmonic equation](../../../../../biharmonic-equation.md) has the form $(A+BY)e^{-Y}\sin\theta$. The vertical condition fixes $A=1$ and excludes a cosine component. The horizontal condition gives

$$
B-1=\delta[(1-2B)-(-1)]
=-2\delta(B-1).
$$

Thus $(1+2\delta)(B-1)=0$ and $B=1$ for every $\delta\geq0$. The spatially averaged first-order [streamfunction](../../../../../stream-function.md) is affine in $Y$; its [Navier slip boundary condition](../../../../../navier-slip-boundary-condition.md) forces $U_1=0$. Therefore

$$
\boxed{\psi_1=(1+Y)e^{-Y}\sin(X-\tau),\qquad U_1=0.}
$$

This [first-order slip independence of a transverse sheet](../../../../../first-order-slip-independence-of-a-transverse-sheet.md) is independent of [slip length](../../../../../slip-length.md). Its surface tangential velocity and surface shear are both zero: $(\psi_1)_Y(0)=0$ and $(\psi_1)_{YY}(0)-(\psi_1)_{XX}(0)=0$. This explains why the first-order [streamfunction](../../../../../stream-function.md) agrees with the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md).

To find the [slip-enhanced swimming speed of a transverse sheet](../../../../../slip-enhanced-swimming-speed-of-a-transverse-sheet.md), expand only the [Navier slip boundary condition](../../../../../navier-slip-boundary-condition.md) through second order. Put $Q_j=(\psi_j)_{YY}-(\psi_j)_{XX}$. [Taylor expansion](../../../../../taylor-expansion.md) at the displaced boundary yields

$$
(\psi_2)_Y-\delta Q_2
=-\sin\theta\,(\psi_1)_{YY}
+\delta\sin\theta\,\partial_YQ_1
\quad\text{at }Y=0.
$$

Direct differentiation gives

$$
(\psi_1)_{YY}(0)=-\sin\theta,\qquad
Q_1=2Ye^{-Y}\sin\theta,\qquad
\partial_YQ_1(0)=2\sin\theta.
$$

Hence

$$
(\psi_2)_Y(X,0,\tau)-\delta Q_2(X,0,\tau)
=(1+2\delta)\sin^2\theta.
$$

Average over $X$. The zero [Fourier series](../../../../../fourier-series-split.md) mode of a [biharmonic streamfunction](../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) is a cubic polynomial in $Y$; bounded velocity at infinity removes the quadratic and cubic terms. Thus its velocity is the constant $U_2$, and its averaged shear $\langle Q_2\rangle_X$ is zero. The [mean boundary velocity determines Taylor-sheet swimming speed](../../../../../mean-boundary-velocity-determines-taylor-sheet-swimming-speed.md) principle then gives

$$
\boxed{U_2=\frac{1+2\delta}{2},\qquad
U^*=\frac{\epsilon^2}{2}(1+2\delta)+O(\epsilon^4).}
$$

The even remainder follows because changing the sign of the amplitude is equivalent to a half-period phase shift. In dimensional form,

$$
\boxed{\mathbf V_{\rm sheet}
=-\frac{\omega k y_0^2}{2}(1+2k\gamma)\,\mathbf e_x
+O\!\left(\frac{\omega}{k}\epsilon^4\right).}
$$

For the [Navier-slip Taylor swimming sheet](../../../../../navier-slip-taylor-swimming-sheet.md), the ratio of speed to the no-slip value is $1+2\delta>1$ whenever $\delta>0$: **slip increases the swimming speed**. The expansion is for fixed $\delta$ as $\epsilon\to0$; it is not a uniform prediction of arbitrarily large speed if the [slip length](../../../../../slip-length.md) is allowed to diverge with the inverse amplitude.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
