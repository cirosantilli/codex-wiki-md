<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [elastic pendulum](../../../../elastic-pendulum.md), set $r=l+x>0$ and measure $\theta$ from the downward vertical. In the vertical plane, Cartesian coordinates are $X=r\sin\theta$ and $Z=-r\cos\theta$, with $Z$ upward. Differentiating gives $\dot X^2+\dot Z^2=\dot x^2+r^2\dot\theta^2$. Thus the [Lagrangian](../../../../lagrangian.md) is

$$
\boxed{L=\frac12m\left(\dot x^2+(l+x)^2\dot\theta^2\right)
-\frac12kx^2+mg(l+x)\cos\theta.}
$$

For $x$, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) gives

$$
\boxed{m\ddot x=m(l+x)\dot\theta^2-kx+mg\cos\theta.}
$$

For $\theta$, the [canonical momentum](../../../../canonical-momentum.md) is $p_\theta=m(l+x)^2\dot\theta$. Its [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\frac{d}{dt}\left[m(l+x)^2\dot\theta\right]+mg(l+x)\sin\theta=0,
$$

or, for positive length,

$$
\boxed{(l+x)\ddot\theta+2\dot x\dot\theta+g\sin\theta=0.}
$$

At an [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md), all time derivatives vanish, so $kx=mg\cos\theta$ and $\sin\theta=0$. Modulo full rotations, the two formal possibilities are

$$
\boxed{(x,\theta)=\left(\frac{mg}{k},0\right),\qquad
(x,\theta)=\left(-\frac{mg}{k},\pi\right).}
$$

The lower configuration always has positive length. The upper one is a physical straight-spring configuration only if $l>mg/k$. For example, $l=mg/(2k)$ would give the purported upper state a negative length $-mg/(2k)$; at $l=mg/k$ its zero length makes the angular coordinate singular. Also, the straight compressed spring is an idealization; a real unsupported compressed spring can buckle.

The [potential energy](../../../../potential-energy.md) is $V=kx^2/2-mg(l+x)\cos\theta$. At either formal stationary point its mixed second derivative vanishes, while

$$
V_{xx}=k,\qquad V_{\theta\theta}=mg(l+x)\cos\theta.
$$

Both curvatures are positive at the lower state, making it a [stable equilibrium](../../../../stable-equilibrium.md); the upper state, when it has positive length, has negative angular curvature and is unstable.

To linearize about the stable state, define the small displacement $\xi=x-mg/k$, not $x$ itself, and $r_0=l+mg/k$. Products such as $\dot\theta^2$, $\dot\xi\dot\theta$ and $\xi\ddot\theta$ are second order, while $\cos\theta=1+O(\theta^2)$ and $\sin\theta=\theta+O(\theta^3)$. The first-order [equations of motion](../../../../equation-of-motion.md) therefore decouple:

$$
\boxed{\ddot\xi+\frac{k}{m}\xi=0,\qquad
\ddot\theta+\frac{g}{l+mg/k}\theta=0.}
$$

There are two independent [normal modes](../../../../normal-mode.md). The radial one is vertical [simple harmonic motion](../../../../simple-harmonic-motion.md) with [angular frequency](../../../../angular-frequency.md) $\omega_r=\sqrt{k/m}$. The transverse one is a [simple pendulum](../../../../simple-pendulum-split.md) oscillation at fixed, statically stretched length $r_0$, with [angular frequency](../../../../angular-frequency.md) $\omega_\theta=\sqrt{g/r_0}$. Their decoupling is a first-order small-oscillation result, not an assertion about the nonlinear motion of the [elastic pendulum](../../../../elastic-pendulum.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
