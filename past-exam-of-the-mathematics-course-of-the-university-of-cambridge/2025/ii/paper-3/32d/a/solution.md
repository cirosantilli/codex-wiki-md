<h1 id="32d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
c=\beta _0e^{8\chi^3t},
\qquad F(s)=ce^{-\chi s},
$$

and seek the [rank-one Gelfand-Levitan-Marchenko kernel](../../../../../../rank-one-gelfand-levitan-marchenko-kernel.md) in the separable form

$$
K(x,y)=-B(x)e^{-\chi y}.
$$

Substitution into the [Gelfand-Levitan-Marchenko equation](../../../../../../marchenko-equation.md) gives

$$
-B(x)+ce^{-\chi x}
-B(x)c\int_x^\infty e^{-2\chi z}\,dz=0,
$$

so

$$
B(x)=\frac{ce^{-\chi x}}
{1+ce^{-2\chi x}/(2\chi)}
$$

and hence

$$
K(x,x)=-\frac{ce^{-2\chi x}}
{1+ce^{-2\chi x}/(2\chi)}.
$$

Write

$$
q=\frac{ce^{-2\chi x}}{2\chi}
=\frac{\beta _0}{2\chi}e^{8\chi^3t-2\chi x}.
$$

The reconstruction formula for this [inverse scattering transform](../../../../../../inverse-scattering-transform.md) convention yields

$$
u(x,t)=-2\frac{\partial}{\partial x}K(x,x)
=-\frac{8\chi^2q}{(1+q)^2}.
$$

If $q=e^{-2s}$, then $4q/(1+q)^2=\operatorname{sech}^2s$. Taking

$$
s=\chi(x-4\chi^2t-\phi)
$$

therefore produces the required one-[soliton](../../../../../../soliton.md) of the [Korteweg-De Vries equation](../../../../../../korteweg-de-vries-equation.md), with

$$
\boxed{\phi=\frac{1}{2\chi}\log\!\left(\frac{\beta _0}{2\chi}\right)}.
$$

Here the usual bound-state norming constant has $\beta _0>0$ and $\chi>0$, so $\phi$ is real.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32D](../../32d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
