<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

The [Hamilton equations](../../../../../hamilton-s-equations.md) are $\dot q=p/m$ and $\dot p=-V_q$. Applying the chain rule to $H(q,p,\lambda(t))$, their two phase-space contributions cancel, giving $\dot H=V_\lambda\dot\lambda=H_\lambda\dot\lambda$.

For fixed $\lambda$, a closed periodic orbit of energy $E$ has $p=\pm\sqrt{2m(E-V)}$. Thus its [action variable](../../../../../action-variable.md) is

$$
I(E,\lambda)=\frac1{2\pi}\oint p\,dq
=\frac{\sqrt{2m}}{2\pi}\oint\pm\sqrt{E-V(q,\lambda)}\,dq.
$$

The sign matches the direction on each half of the orbit, making the enclosed phase-plane area positive. Since $dq=\dot q\,dt=p\,dt/m$, differentiating under the integral gives

$$
\boxed{I_E=\frac1{2\pi}\oint\frac m p\,dq=\frac\tau{2\pi},
\qquad I_\lambda=-\frac1{2\pi}\oint V_\lambda\,dt.}
$$

For slowly varying $\lambda$, the exact energy equation averaged over a nearly frozen cycle gives $d\langle H\rangle/dt=\langle V_\lambda\rangle\dot\lambda$ to the retained adiabatic order. Using $E=\langle H\rangle$, the two chain-rule terms therefore cancel:

$$
\frac{dI}{dt}=\frac\tau{2\pi}\langle V_\lambda\rangle\dot\lambda
-\frac1{2\pi}\oint V_\lambda\,dt\,\dot\lambda=0.
$$

Here the angle brackets differentiate the explicit parameter dependence along the frozen cycle, not an independently chosen family of energies. **The action is an adiabatic invariant**, with errors beyond the slow-cycle approximation.

For $V=\lambda q^{2n}$, scale $q=(E/\lambda)^{1/(2n)}s$. Then

$$
I=\frac{2\sqrt{2m}}\pi E^{(n+1)/(2n)}\lambda^{-1/(2n)}
\int_0^1\sqrt{1-s^{2n}}\,ds.
$$

The integral is a positive constant depending only on $n$. Constancy of $I$ gives $E^{n+1}/\lambda$ constant, hence

$$
\boxed{\langle H\rangle=C\lambda^{1/(n+1)}.}
$$

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
