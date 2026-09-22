<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Cartesian streamfunction](../../../../../../cartesian-streamfunction.md) convention $u=\psi_y$, $v=-\psi_x$. Taking the [curl](../../../../../../curl.md) of the incompressible [Stokes equation](../../../../../../stokes-equation.md) eliminates pressure and gives the [biharmonic stream function for planar Stokes flow](../../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) equation

$$
\boxed{\nabla^4\psi=0\quad\hbox{for }y>\epsilon\sin\theta,\qquad \theta=x-t.}
$$

The material points have no horizontal velocity in the swimming frame and have vertical velocity $-\epsilon\cos\theta$. The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) is therefore

$$
\boxed{\psi_y(x,\epsilon\sin\theta,t)=0,\qquad \psi_x(x,\epsilon\sin\theta,t)=\epsilon\cos\theta.}
$$

At infinity the laboratory fluid is at rest, so in this translating frame it moves with $U\mathbf e_x$:

$$
\boxed{\psi_y\to U,\qquad \psi_x\to0\quad(y\to\infty).}
$$

Velocity and its perturbations are periodic in $x$, with period $2\pi$, and the pressure has no imposed mean gradient. The [Taylor swimming sheet](../../../../../../taylor-swimming-sheet.md) is [force-free](../../../../../../force-free.md); the unbounded problem's bounded far-field velocity enforces the absence of mean shear. An additive constant in the streamfunction has no physical effect.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 334](../../../paper-334-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
