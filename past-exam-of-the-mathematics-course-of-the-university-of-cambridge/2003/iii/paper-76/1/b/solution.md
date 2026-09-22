<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The radius law integrates to $r(z)=r_0e^{-\beta z}$, so the cross-sectional area is $A(z)=\pi r_0^2e^{-2\beta z}$. Conserving gas volume in a horizontal slice yields

$$
\partial_t(A\phi)+\partial_z\bigl[AV_s\phi(1-\phi)\bigr]=0,
$$

or the [kinematic bubble transport in an exponentially narrowing vessel](../../../../../../kinematic-bubble-transport-in-an-exponentially-narrowing-vessel.md) equation

$$
\boxed{\phi_t+V_s(1-2\phi)\phi_z=2\beta V_s\phi(1-\phi).}
$$

The geometrical term increases the concentration as a given gas flux enters a smaller area. On concentration [characteristic curves](../../../../../../characteristic-curve.md),

$$
\boxed{\frac{dz}{dt}=V_s(1-2\phi),\qquad
\frac{d\phi}{dt}=2\beta V_s\phi(1-\phi).}
$$

Put $c=2\beta V_s$. A characteristic starting at $(z_0,0)$ with $\phi_i=\phi(z_0,0)$ has

$$
\boxed{\phi(t)=\frac{\phi_i e^{ct}}{1-\phi_i+\phi_i e^{ct}},\qquad
z(t)=z_0+V_st-\frac1\beta\log\left(1-\phi_i+\phi_i e^{ct}\right).}
$$

The first formula follows by integrating $d\phi/[\phi(1-\phi)]=c\,dt$; inserting it into $dz/dt$ gives the second. For initially uniform $\phi_0$, the uninterrupted bubbly region remains spatially uniform, with this time-dependent concentration. These [characteristic curves](../../../../../../characteristic-curve.md) carry concentration information; they are not individual bubble trajectories, whose speed is $V_s(1-\phi)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
