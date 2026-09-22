<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
 A=\frac1{D^2}+\frac{ik}{2F},\qquad
 q(x)=1+\frac{2iAx}{k}=1-\frac xF+\frac{2ix}{kD^2}.
$$

In free space, the [parabolic wave equation](../../../../../../parabolic-wave-equation.md) is $E_x=iE_{zz}/(2k)$. Under the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat E(p)=\int E(z)e^{-ipz}\,dz$, it becomes

$$
 \partial_x\widehat E=-\frac{ip^2}{2k}\widehat E,\qquad
 \widehat E(0,p)=\sqrt{\frac\pi A}\exp\left(-\frac{p^2}{4A}\right).
$$

The [Gaussian integral](../../../../../../gaussian-integral.md) is legitimate because $\operatorname{Re}A=1/D^2>0$. Invert the transform after multiplying by $e^{-ip^2x/(2k)}$. A second [Gaussian integral](../../../../../../gaussian-integral.md), or equivalently [one-dimensional transverse Fresnel propagation](../../../../../../one-dimensional-transverse-fresnel-propagation.md), gives

$$
\boxed{E(x,z)=q(x)^{-1/2}\exp\left(-\frac{Az^2}{q(x)}\right).}
$$

Choose the square-root branch continuously from $q(0)^{-1/2}=1$; for real $x\geq0$ there is no zero of $q$. This gives the correct incident field at $x=0$, and direct differentiation verifies the free [parabolic wave equation](../../../../../../parabolic-wave-equation.md).

For clarity, the squared envelope magnitude is

$$
 |E(x,z)|^2=\frac1{|q(x)|}\exp\left(-\frac{2z^2}{D^2|q(x)|^2}\right),\qquad
 D(x)=D\sqrt{(1-x/F)^2+\left(\frac{2x}{kD^2}\right)^2}.
$$

The [Gaussian beam with one transverse coordinate](../../../../../../gaussian-beam-with-one-transverse-coordinate.md) remains Gaussian, with one-transverse-coordinate amplitude factor $q^{-1/2}$, not the $q^{-1}$ of a beam with two transverse coordinates. The negative initial quadratic phase produces focusing for $F>0$; [diffraction](../../../../../../diffraction.md) prevents a singularity at $x=F$. These expressions describe the [paraxial approximation](../../../../../../paraxial-approximation.md) to free propagation, rather than an exact unrestricted [Helmholtz equation](../../../../../../helmholtz-equation.md) beam.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
