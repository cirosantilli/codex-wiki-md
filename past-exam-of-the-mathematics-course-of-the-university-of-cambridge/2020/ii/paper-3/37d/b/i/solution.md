<h1 id="37d/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put

$$
\rho=\sqrt{r^2+a^2},
\qquad
\varpi=\rho\sin\theta,
\qquad
z=r\cos\theta.
$$

Since $x^2+y^2=\varpi^2$, the Euclidean spatial line element is

$$
dx^2+dy^2+dz^2=d\varpi^2+\varpi^2d\phi^2+dz^2.
$$

Now

$$
d\varpi=\frac r\rho\sin\theta\,dr
+\rho\cos\theta\,d\theta,
\qquad
dz=\cos\theta\,dr-r\sin\theta\,d\theta.
$$

The cross terms cancel. With

$$
\Sigma=r^2+a^2\cos^2\theta,
\qquad
\Delta=r^2+a^2,
$$

we obtain the [oblate spheroidal coordinates](../../../../../../../oblate-spheroidal-coordinates.md) line element

$$
dx^2+dy^2+dz^2
=\frac\Sigma\Delta dr^2+\Sigma d\theta^2
+\Delta\sin^2\theta\,d\phi^2.
$$

Adding the time coordinate gives

$$
\boxed{
ds^2=-dt^2
+\frac{r^2+a^2\cos^2\theta}{r^2+a^2}dr^2
+(r^2+a^2\cos^2\theta)d\theta^2
+(r^2+a^2)\sin^2\theta\,d\phi^2}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [37D](../../../37d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
