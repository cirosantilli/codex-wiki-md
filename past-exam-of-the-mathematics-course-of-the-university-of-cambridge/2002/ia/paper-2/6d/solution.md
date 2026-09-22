<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

For the [logistic differential equation](../../../../../logistic-differential-equation.md), separate variables to obtain $\log|y/(1-ay)|=rt+C$ away from the constant solutions. Applying the positive [initial condition](../../../../../initial-condition.md) gives

$$
\boxed{y(t)=\frac{1}{a+(y_0^{-1}-a)e^{-rt}}=\frac{y_0e^{rt}}{1+ay_0(e^{rt}-1)},\quad t\ge0.}
$$

The formula also includes the constant solution $y_0=1/a$. Below $1/a$ positive solutions increase; above $1/a$ they decrease. They approach $1/a$ as $t\to\infty$. Equivalently, linearizing $F(y)=ry(1-ay)$ gives $F'(0)=r>0$ and $F'(1/a)=-r<0$. Thus **zero is unstable and $1/a$ is asymptotically stable.**

The [Forward Euler method](../../../../../euler-method.md) gives $y_{n+1}=(1+r\delta t)y_n-ra\delta t\,y_n^2$. Set $\lambda=1+r\delta t$ and $u_n=a(\lambda-1)y_n/\lambda$; multiplying the recurrence by this scaling factor gives the [logistic map](../../../../../logistic-map.md)

$$
\boxed{u_{n+1}=\lambda u_n(1-u_n).}
$$

Its [fixed points](../../../../../fixed-point.md) are $u=0$ and $u_*=1-1/\lambda$. The [fixed-point multipliers](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are $F'(0)=\lambda$ and $F'(u_*)=2-\lambda$. Since $\lambda>1$, zero is always unstable. The positive [fixed point](../../../../../fixed-point.md) is stable for $1<\lambda<3$ and unstable for $\lambda>3$. For $\lambda>3$, a small displacement obeys $\epsilon_{n+1}\simeq(2-\lambda)\epsilon_n$: its sign alternates and its amplitude grows, giving an oscillatory instability whose period is **$2\delta t$**.

This is an artifact of [Euler discretization of logistic growth](../../../../../euler-discretization-of-logistic-growth.md). Exact small perturbations decay by the positive factor $e^{-r\delta t}$ per time step; a one-dimensional autonomous [differential equation](../../../../../differential-equation-split.md) cannot have a nonconstant [periodic orbit](../../../../../periodic-orbit.md), since its solutions move monotonically between [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md). The artificial instability occurs when $r\delta t>2$, beyond the stable step range of this discretization.

For $\lambda=3.2$, remove the [fixed point](../../../../../fixed-point.md) factors from $F(F(u))-u$ to obtain $\lambda^2u^2-\lambda(\lambda+1)u+\lambda+1=0$. The resulting [logistic map two-cycle](../../../../../logistic-map-two-cycle.md) is

$$
\boxed{u_-\simeq0.5130445,\quad u_+\simeq0.7994555,\qquad u_\pm=\frac{\lambda+1\pm\sqrt{(\lambda-3)(\lambda+1)}}{2\lambda}.}
$$

These points map to each other. Their [periodic-orbit multiplier](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is $F'(u_-)F'(u_+)=4+2\lambda-\lambda^2=0.16$, so the two-cycle attracts nearby iterates. The cobweb shows a small initial departure from $u_*=0.6875$ growing with alternating sign and then settling into the finite rectangle between $u_-$ and $u_+$. The time trace shows the corresponding finite-amplitude oscillation.

<a id="6d/image-logistic-map-cobweb-and-alternating-iterates-approaching-the-stable-two-cycle-at-parameter-3-2"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2-logistic.png)

**[Figure 3](#6d/image-logistic-map-cobweb-and-alternating-iterates-approaching-the-stable-two-cycle-at-parameter-3-2). Logistic-map cobweb and alternating iterates approaching the stable two-cycle at parameter 3.2**.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
