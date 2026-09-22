<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The shear has $E_{xy}=E_{yx}=C/2$. The separation between centers is $2(X,Y,0)$, so in the leading [stresslet](../../../../../../force-dipole-flow.md) from part b, $q=4CXY$, $r=2R$ and the radial vector's $y$ component is $2Y$. Evaluating the other sphere's disturbance at the positive center gives

$$
\boxed{\dot Y=-\frac{5Ca^3}{8}\frac{XY^2}{R^5}+O(Ca^5/R^4).}
$$

This is the first [method of reflections for Stokes flow](../../../../../../method-of-reflections-for-stokes-flow.md) approximation. The next multipole in part b and the receiver's Faxén Laplacian contribute at $Ca^5/R^4$; changes to the incident strain from further reflections are smaller, $Ca^6/R^5$. The hypothesis $Y_\infty\gg a$ ensures well-separated spheres throughout the encounter.

The leading horizontal velocity is $\dot X=CY+O(Ca^3/R^2)$. Dividing and using $Y_\infty$ on the right at first order gives

$$
\frac{dY}{dX}=-\frac{5a^3Y_\infty}{8}\frac{X}{(X^2+Y_\infty^2)^{5/2}}+\text{higher orders}.
$$

Integrating from negative infinity,

$$
Y(X)=Y_\infty+\frac{5a^3Y_\infty}{24(X^2+Y_\infty^2)^{3/2}}
+O(a^5/Y_\infty^4).
$$

The correction increases until $X=0$ and decreases afterward. **Thus**

$$
\boxed{Y_m=Y_\infty\left(1+\frac{5a^3}{24Y_\infty^3}
+O(a^5/Y_\infty^5)\right).}
$$

The expansion gives $Y\to Y_\infty$ as $X\to+\infty$. More generally, [reversible scattering of two spheres in simple shear](../../../../../../reversible-scattering-of-two-spheres-in-simple-shear.md) gives no net transverse shift for this smooth, noncontact, deterministic two-sphere encounter: reflection $X\mapsto-X$ reverses the imposed shear, and time reversal restores it. Uniqueness makes the incoming and outgoing branches mirror images. Brownian motion, contact forces or finite inertia would remove the assumptions behind this conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
