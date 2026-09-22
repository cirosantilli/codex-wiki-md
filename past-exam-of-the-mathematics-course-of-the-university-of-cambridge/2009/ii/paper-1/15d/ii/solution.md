<h1 id="15d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For constant equation-of-state parameter $w$, the [cosmological continuity equation](../../../../../../cosmological-continuity-equation.md) integrates to $\rho=\rho_0a^{-3(1+w)}$ using today's normalization. In [conformal time](../../../../../../conformal-time.md), $\mathcal H=a'/a=\dot a$, so the [Friedmann equation](../../../../../../friedmann-equations.md) becomes

$$
\boxed{\mathcal H^2+kc^2=\frac{8\pi G\rho_0}{3}a^{-(1+3w)}.}
$$

Since $\mathcal H'=a\ddot a$, the [Friedmann acceleration equation](../../../../../../friedmann-acceleration-equation.md) gives

$$
\boxed{\mathcal H'+\tfrac12(1+3w)(\mathcal H^2+kc^2)=0.}
$$

For $kc^2=1$, put $q=(1+3w)/2$. When $q\ne0$, integration gives $\mathcal H=\cot(q(\tau-\tau_0))$. Integrating $a'/a=\mathcal H$ then yields the [closed constant-equation-of-state Friedmann scale factor](../../../../../../closed-constant-equation-of-state-friedmann-scale-factor.md)

$$
\boxed{a=\alpha[\sin(q(\tau-\tau_0))]^{1/q},\quad \beta=q,\quad
\alpha=\left(\frac{8\pi G\rho_0}{3}\right)^{1/(1+3w)}.}
$$

Choose a connected interval with positive sine; the origin of [conformal time](../../../../../../conformal-time.md) can absorb $\tau_0$. For $w>-1/3$ this is the expansion and recollapse branch between consecutive zeros of the sine. Negative $q$ instead gives the corresponding minimum-radius branch on its positive-sine interval. The printed power formula excludes $w=-1/3$: in that exceptional case $\mathcal H=H_0$ is constant and $a=Ae^{H_0\tau}$, with $H_0^2+1=8\pi G\rho_0/3$. A real solution requires the latter constant to be at least one; equality permits a static solution.

For pressure-free matter, $w=0$, so $\beta=1/2$. Set the big-bang origins to zero. The [closed matter-dominated Friedmann solution](../../../../../../closed-matter-dominated-friedmann-solution.md) follows by $\sin^2(\beta\tau)=(1-\cos2\beta\tau)/2$ and integrating $dt=a\,d\tau$:

$$
\boxed{a=\frac\alpha2(1-\cos2\beta\tau),\qquad
 t=\frac{\alpha}{4\beta}(2\beta\tau-\sin2\beta\tau).}
$$

The entire cycle is $0\leq2\beta\tau\leq2\pi$; maximum expansion has $a=\alpha$ at $2\beta\tau=\pi$, and the big crunch occurs at $t=\alpha\pi/(2\beta)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
