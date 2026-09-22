<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Use a [translating accelerated reference frame](../../../../../translating-accelerated-reference-frame.md); its axes do not rotate. If $\mathbf R=(\xi,\eta,\zeta)$ is the block's [position](../../../../../position.md) relative to the table, then its inertial [position](../../../../../position.md) is $\mathbf r=\mathbf R+\mathbf A\sin\omega t$. Its relative [velocity](../../../../../velocity.md) is $\dot{\mathbf R}$ and its inertial [acceleration](../../../../../acceleration.md) is $\ddot{\mathbf R}-\omega^2\mathbf A\sin\omega t$. Let $N$ be the upward [normal force](../../../../../normal-force.md). During contact $\zeta=\dot\zeta=\ddot\zeta=0$, and the linear tangential resistance gives

$$
\boxed{m\ddot\xi+\lambda\dot\xi=mA_x\omega^2\sin\omega t,\qquad
m\ddot\eta+\lambda\dot\eta=0,\qquad
m\ddot\zeta=N-mg+mA_z\omega^2\sin\omega t.}
$$

These are [Newton's second law](../../../../../newton-s-second-law.md) transformed to the table's [reference frame](../../../../../reference-frame.md); the extra terms arise from the table's [acceleration](../../../../../acceleration.md). The last equation gives $N=m(g-A_z\omega^2\sin\omega t)$ while contact persists. If contact is lost, both the contact resistance and $N$ vanish, and free flight must be described by the corresponding gravity-only equations.

For $A_z=0$, assume $\lambda>0$ and put $\gamma=\lambda/m$. Seek a periodic particular solution $\xi_p=b\sin\omega t+c\cos\omega t$. Substitution into the first [differential equation](../../../../../differential-equation-split.md) gives

$$
-\omega^2b-\gamma\omega c=A_x\omega^2,\qquad
-\omega^2c+\gamma\omega b=0.
$$

Solving yields

$$
b=-\frac{A_x\omega^2}{\gamma^2+\omega^2},\qquad
c=-\frac{A_x\gamma\omega}{\gamma^2+\omega^2}.
$$

The homogeneous solutions are a constant and a multiple of $e^{-\gamma t}$. Choose the phase $0<\theta<\pi/2$ with $\tan\theta=\omega/\gamma=m\omega/\lambda$. Then $b=-A_x\sin^2\theta$ and $c=-A_x\sin\theta\cos\theta$, so

$$
\boxed{\xi(t)=\xi_0-A_x\sin\theta\cos(\omega t-\theta)+C e^{-\lambda t/m},\qquad
\sin^2\theta=\frac{m^2\omega^2}{\lambda^2+m^2\omega^2}.}
$$

Also $\eta(t)=\eta_\infty+C_\eta e^{-\lambda t/m}$. The decaying transients leave the stated steady orbit. Positive damping is essential to this late-time assertion; for $\lambda=0$ an additional constant drift may persist.

No attractive contact [force](../../../../../force.md) is available, so $N$ cannot be negative. Over a whole oscillation its minimum is $m(g-\omega^2|A_z|)$. Thus **strictly positive contact loading throughout requires** $\boxed{\omega^2|A_z|<g}$, or the printed form with $A_z$ taken as a nonnegative vertical [amplitude](../../../../../wave-amplitude.md). If $\omega^2|A_z|>g$, contact cannot persist: it would require $N<0$ during part of the cycle. At equality, $N$ vanishes only at isolated instants and the ideal constrained motion can still remain in contact. Hence the strict inequality characterizes positive loading; mere nonnegative contact permits the marginal equality case.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
