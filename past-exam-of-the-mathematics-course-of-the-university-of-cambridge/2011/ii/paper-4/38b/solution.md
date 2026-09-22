<h1 id="38b/solution">Solution</h1>

↑ **Parent:** [38B](../38b.md)

For smooth [isentropic flow](../../../../../isentropic-flow.md) with $p=K\rho^\gamma$, $\gamma>1$, the continuity and momentum equations give

$$
u_t+u u_x+\frac{2c}{\gamma-1}c_x=0,\qquad
c_t+u c_x+\frac{\gamma-1}{2}c u_x=0,
$$

where $c^2=dp/d\rho$. Adding and subtracting these equations shows

$$
\boxed{[\partial_t+(u\pm c)\partial_x]\left[u\pm\frac{2(c-c_0)}{\gamma-1}\right]=0.}
$$

These are the [Riemann invariants](../../../../../riemann-invariant.md) on the two characteristic families.

Before any shock, the incoming $C_-$ characteristics originate in the initially uniform gas, so their invariant is zero. Thus $c=c_0+(\gamma-1)u/2$ throughout the disturbed [simple wave](../../../../../simple-wave.md). A $C_+$ characteristic leaving the piston at time $\tau$ has constant $u=\dot X(\tau)$ and speed $u+c=c_0+(\gamma+1)\dot X(\tau)/2$. Therefore

$$
\boxed{u(x,t)=\dot X(\tau),\qquad x=X(\tau)+\left[c_0+\frac{\gamma+1}{2}\dot X(\tau)\right](t-\tau).}
$$

This parametrization applies for $0\le\tau\le t$ in $X(t)\le x\le c_0t$ as long as the characteristics remain ordered. The gas for $x\ge c_0t$ is still at rest. The values $\tau=t$ and $\tau=0$ give the piston and leading disturbance respectively.

Characteristic crossing first occurs when the derivative of the displayed $x(\tau,t)$ with respect to $\tau$ vanishes. With $U(\tau)=\dot X(\tau)$ this gives

$$
t_s(\tau)=\tau+\frac{c_0+(\gamma-1)U(\tau)/2}{(\gamma+1)U'(\tau)/2}.
$$

For the printed $X=2c_0t^3/(3T^2)$, $U=2c_0\tau^2/T^2$, so

$$
t_s(\tau)=\frac{(3\gamma+1)\tau+T^2/\tau}{2(\gamma+1)}.
$$

Its minimum over $\tau>0$ occurs at $\tau_*=T/\sqrt{3\gamma+1}$ and satisfies $t_s>\tau_*$. Hence **the first shock forms at**

$$
\boxed{t_{\rm shock}=\frac{T\sqrt{3\gamma+1}}{\gamma+1}.}
$$

The characteristic formula is restricted to earlier times; crossing afterwards must be replaced by a shock satisfying the conservation laws.

## ↑ Ancestors (10)

1. [38B](../38b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
