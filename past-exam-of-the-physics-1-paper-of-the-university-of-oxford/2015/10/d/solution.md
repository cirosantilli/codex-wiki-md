<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

When the block is free, $x$ becomes a dynamical [generalized coordinate](../../../../generalized-coordinate.md) and its [kinetic energy](../../../../kinetic-energy.md) $M\dot x^2/2$ must be included. Expanding to quadratic order about the downward stationary state and dropping a constant gives

$$
\boxed{\mathcal L_2=\frac12(M+m)\dot x^2+ml\dot x\dot\theta+\frac12ml^2\dot\theta^2-\frac12mgl\theta^2.}
$$

The coordinate $x$ is cyclic. Its conserved [canonical momentum](../../../../canonical-momentum.md) is the total horizontal [momentum](../../../../momentum-split.md),

$$
P=(M+m)\dot x+ml\dot\theta.
$$

The two linear [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
(M+m)\ddot x+ml\ddot\theta=0,\qquad l\ddot\theta+\ddot x+g\theta=0.
$$

Eliminating $\ddot x$ gives

$$
\boxed{\ddot\theta+\Omega^2\theta=0,\qquad \Omega^2=\frac{(M+m)g}{Ml}.}
$$

Thus the [pendulum with a freely sliding support](../../../../pendulum-with-a-freely-sliding-support.md) has a zero-frequency translational mode and an oscillatory mode. With four independent constants $X_c,V,C,D$, the general solution is

$$
\boxed{\theta(t)=C\cos\Omega t+D\sin\Omega t,\qquad
x(t)=X_c+Vt-\frac{ml}{M+m}\theta(t).}
$$

Here $V=P/(M+m)$ and $X_c+Vt$ is the horizontal [centre of mass](../../../../center-of-mass.md) coordinate to first order, since $X_{\mathrm{CM}}=x+[ml/(M+m)]\theta$. The oscillation is faster than that of a pendulum with a fixed pivot; the limit $M\to\infty$ restores $\Omega\to\sqrt{g/l}$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [10](../../10.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
