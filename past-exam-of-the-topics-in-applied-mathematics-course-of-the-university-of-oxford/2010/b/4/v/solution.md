<h1 id="b/4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First assume $\omega_0\ne0$ and regard $\theta$ modulo $2\pi$. The section $\theta=0$ has return time $T=2\pi/|\omega_0|$. Solving the resonantly forced oscillator from this section gives

$$
x(t)=x_0\cos(\omega_0t)+\frac{y_0}{\omega_0}\sin(\omega_0t)+\frac{\gamma}{2\omega_0}t\sin(\omega_0t).
$$

At $t=T$, the sine vanishes and the cosine is one, while differentiating the secular term adds $\gamma T/2$ to $y$. Hence the [Poincaré map](../../../../../poincare-map.md) is

$$
\boxed{P(x,y)=(x,y+\gamma T/2).}
$$

For $\gamma>0$, every iterate has $y_n=y_0+n\gamma T/2\to\infty$. Thus every oscillator trajectory is unbounded, regardless of its initial amplitude. For an arbitrary section phase $\theta_0$, the return map translates by $(\gamma T\sin\theta_0/(2\omega_0),\gamma T\cos\theta_0/2)$, which is still nonzero. At $\gamma=0$ the map is the identity, and all $(x,y)$ motions are bounded harmonic oscillations, including the zero-amplitude [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md).

**The zero-frequency case allowed by the printed parameter range is different.** If $\omega_0=0$, then $\theta=\theta_0$ is constant and $x=x_0+y_0t+\tfrac12\gamma\cos\theta_0t^2$. There is no phase-crossing Poincaré section. For $\gamma>0$, choosing $\cos\theta_0=0$ and $y_0=0$ gives bounded [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md), contradicting an unqualified “all trajectories” statement. For $\gamma=0$ at zero frequency, free-particle motion is unbounded unless $y_0=0$. The [resonance](../../../../../resonance.md) conclusion therefore requires the natural nonzero-frequency assumption.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
