<h1 id="18b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Substitute the rotating [velocity field](../../../../../../velocity-field.md) into the [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md). Its acceleration is $(-\dot\Omega y-\Omega^2x,\dot\Omega x-\Omega^2y,0)$, so

$$
\frac{p_x}{\rho}=(\alpha+\Omega^2)x+(\beta+\dot\Omega)y,\qquad
\frac{p_y}{\rho}=(\gamma-\dot\Omega)x+(\delta+\Omega^2)y,\qquad p_z=0.
$$

The preceding angular acceleration makes both mixed coefficients $(\beta+\gamma)/2$, ensuring integrability. Thus

$$
\boxed{p(x,y,t)=p_0(t)+\frac\rho2\left[(\alpha+\Omega(t)^2)x^2+(\beta+\gamma)xy+(\delta+\Omega(t)^2)y^2\right].}
$$

Pressure is determined up to the spatially uniform function $p_0(t)$. The specified force has no vertical component; if gravity were additionally included in the body force, the usual hydrostatic term $-\rho gz$ would also appear. It is not implied by the displayed force here.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [18B](../../18b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
