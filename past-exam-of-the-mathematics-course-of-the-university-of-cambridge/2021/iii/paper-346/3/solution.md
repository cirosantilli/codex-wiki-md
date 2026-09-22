<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a spherical orbit,

$$
v_c^2=r\frac{d\phi}{dr}=v_0^2,
$$

so the [galaxy rotation curve](../../../../../galaxy-rotation-curve.md) is flat. The isotropic spherical [Jeans equation](../../../../../jeans-equation.md) with constant dispersion is

$$
\frac d{dr}(\rho\sigma^2)=-\rho\frac{d\phi}{dr}.
$$

Since $\rho\propto r^{-2}$,

$$
-\frac{2\rho\sigma^2}{r}
=-\frac{\rho v_0^2}{r},
\qquad
\boxed{\sigma=\frac{v_0}{\sqrt2}}.
$$

Write

$$
\mathcal F(X)=\operatorname{erf}X
-\frac{2X}{\sqrt\pi}e^{-X^2}.
$$

For $X\ll1$,

$$
\mathcal F(X)=\frac{4X^3}{3\sqrt\pi}+O(X^5),
$$

so [Chandrasekhar dynamical friction](../../../../../chandrasekhar-dynamical-friction.md) is linear in $\mathbf v$ at low speed. At $X\gg1$, $\mathcal F(X)\to1$, so its acceleration magnitude decays as $v^{-2}$. At zero speed the wake is symmetric and the drag vanishes; at high speed the subhalo spends too little time deflecting each background particle efficiently.

For a circular orbit $v=v_0$, so $X=1$ and $\mathcal F(1)=0.428$. The tangential acceleration is

$$
a_{\rm df}
=-0.428\,\frac{4\pi G^2M\rho\log\Lambda}{v_0^2}
=-0.428\,\frac{GM\log\Lambda}{r^2}.
$$

The specific angular momentum is $L=rv_0$, hence $v_0\dot r=ra_{\rm df}$ and

$$
\boxed{
r\dot r=-0.428\,\log\Lambda\,\frac{GM}{v_0}
}.
$$

Integration from $r_i$ to zero gives

$$
\boxed{
t_{\rm df}
=\frac{r_i^2v_0}{2(0.428)GM\log\Lambda}
=\frac{1.17\,r_i^2v_0}{GM\log\Lambda}
}.
$$

For a circular orbit of radius $r$,

$$
E=\frac{v_0^2}{2}+v_0^2\log(r/r_0).
$$

Solving for $r$ gives

$$
\boxed{
L_{\rm circ}(E)
=v_0r_0
\exp\left(\frac{E-v_0^2/2}{v_0^2}\right)
}.
$$

Since $\eta=L/L_{\rm circ}(E)$,

$$
\boxed{
\dot\eta
=\eta\left(\frac{\dot L}{L}
-\frac{\dot E}{v_0^2}\right)
}.
$$

The friction acceleration is antiparallel to velocity, so locally $\dot L/L=(1/v)\dot v$ and $\dot E=v\dot v$. Applying the chain rule $\dot e=(de/d\eta)\dot\eta$ gives

$$
\boxed{
\dot e
=\frac{\eta}{v}\frac{de}{d\eta}
\left(1-\frac{v^2}{v_0^2}\right)\dot v
}.
$$

Because $d\eta/de<0$ and $\dot v<0$, at pericentre $v>v_0$ gives $\dot e<0$: friction circularizes. At apocentre $v<v_0$ gives $\dot e>0$: it makes the orbit more eccentric. Orbit averaging produces substantial cancellation; the denser pericentre region generally gives modest net circularization, but the eccentricity changes much less dramatically than the orbital energy and radius.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
