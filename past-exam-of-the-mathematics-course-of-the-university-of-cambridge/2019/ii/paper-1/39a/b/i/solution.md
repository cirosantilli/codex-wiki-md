<h1 id="39a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The undisturbed gas has $u=0$, $c=c_0$, and hence $R_-=0$. The disturbance from the receding piston is a right-moving [simple wave](../../../../../../../simple-wave.md), so this invariant remains zero throughout it:

$$
c=c_0+\frac{\gamma-1}{2}u,
\qquad
\rho=\rho_0\left(1+\frac{\gamma-1}{2c_0}u\right)^{2/(\gamma-1)}.
$$

Let $s$ be the time at which the relevant $C_+$ characteristic leaves the piston. The boundary condition is $u=\dot X_p(s)$ there. Both $u$ and $c$ are constant along this characteristic, whose speed is

$$
u+c=c_0+\frac{\gamma+1}{2}\dot X_p(s).
$$

Hence $s=s(x,t)$ is determined implicitly by the [receding-piston rarefaction wave](../../../../../../../receding-piston-rarefaction-wave.md) equation

$$
\boxed{x=X_p(s)+\left[c_0+\frac{\gamma+1}{2}\dot X_p(s)\right](t-s).}
$$

Within $X_p(t)<x<c_0t$, the solution is therefore

$$
\boxed{u(x,t)=\dot X_p(s(x,t)),}
$$



$$
\boxed{\rho(x,t)=\rho_0
\left[1+\frac{\gamma-1}{2c_0}\dot X_p(s(x,t))\right]^{2/(\gamma-1)}.}
$$

For $x\geq c_0t$, the gas remains undisturbed: $u=0$ and $\rho=\rho_0$. The speed bound keeps $c$ and $\rho$ positive, and monotonic increase of $|\dot X_p|$ makes this an expanding [rarefaction wave](../../../../../../../rarefaction-wave.md) rather than a characteristic-crossing compression.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [39A](../../../39a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
