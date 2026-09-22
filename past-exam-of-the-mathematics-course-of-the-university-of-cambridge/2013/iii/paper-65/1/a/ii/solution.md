<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The leading [Stokes drift](../../../../../../../stokes-drift.md) comes from evaluating the oscillatory [velocity](../../../../../../../velocity.md) at the displaced particle position. [Taylor expansion](../../../../../../../taylor-expansion.md) gives

$$
u(X,Z,t)-u(x,z,t)=(X-x)u_x+(Z-z)u_z+O(a^3k^2\omega).
$$

Here $u_x=-ak\omega e^{kz}\sin\vartheta$ and $u_z=ak\omega e^{kz}\cos\vartheta$. Inserting the initial-position displacements from the preceding solution yields

$$
\boxed{u(X,Z,t)-u(x,z,t)=a^2k\omega e^{2kz}[1-\cos(\omega t)]+O(a^3k^2\omega).}
$$

In particular the instantaneous difference is zero at $t=0$, as it must be. The unaveraged constant equality in the PDF is incompatible with its initial labels. Averaging over a period $\mathcal T=2\pi/\omega$ removes the oscillatory term:

$$
\boxed{u_s\equiv\left\langle u(X,Z,t)-u(x,z,t)\right\rangle=a^2k\omega e^{2kz}.}
$$

Equivalently, using mean parcel labels and the purely oscillatory displacements gives $a^2k\omega e^{2kz}(\sin^2\vartheta+\cos^2\vartheta)$ at this order. This recovers the intended constant result. **The period-mean drift is in the wave-propagation direction and decreases as $e^{2kz}$.** The corresponding second-order vertical difference is $a^2k\omega e^{2kz}\sin(\omega t)$ for initial labels and has zero mean. The resulting horizontal displacement per cycle is $u_s\mathcal T$; closed first-order circles do not imply zero second-order transport.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
