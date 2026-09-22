<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the forward-slope convention established in part a, with $x'=Ax+B\theta$ and $\theta'=Cx+D\theta$, where $AD-BC=1$. Assume $B\ne0$. Solve for the endpoint slopes:

$$
\theta=\frac{x'-Ax}{B},\qquad \theta'=\frac{Dx'-x}{B}.
$$

[Fermat's principle](../../../../fermat-principle.md) makes the optical path stationary against variations at internal interfaces. Consequently only endpoint terms survive when its endpoints change. For optical path $l(x,x')$, these are

$$
\frac{\partial l}{\partial x}=-\theta=\frac{Ax-x'}B,\qquad
\frac{\partial l}{\partial x'}=\theta'=\frac{Dx'-x}B.
$$

Integrate the first equation with respect to $x$, then match the second and impose $l(0,0)=L_0$. The resulting [ABCD optical path generating function](../../../../abcd-optical-path-generating-function.md) is

$$
\boxed{l(x,x')=L_0+\frac{Ax^2+Dx'^2-2xx'}{2B}.}
$$

Thus the geometrical kernel defined in the source would have the form

$$
\boxed{K(x,x')=\frac{\exp\!\left\{ik\left[L_0+(Ax^2+Dx'^2-2xx')/(2B)\right]\right\}}{L_0+(Ax^2+Dx'^2-2xx')/(2B)}.}
$$

**The printed minus sign is inconsistent with forward propagation under these conventions.** A concrete counterexample is free space: $A=D=1$, $B=L>0$, $C=0$. Its true geometrical path is

$$
\sqrt{L^2+(x'-x)^2}=L+\frac{(x'-x)^2}{2L}+O\!\left((x'-x)^4/L^3\right),
$$

whereas the printed expression predicts a path shorter than $L$ for nonzero transverse separation. For example, $L=1\,\mathrm m$, $x=0$, $x'=1\,\mathrm{mm}$ gives $1\,\mathrm m+0.5\,\mu\mathrm m$, rather than the printed $1\,\mathrm m-0.5\,\mu\mathrm m$. Reversing the slope convention would also reverse the free-space $B$ entry and must be done consistently; it cannot justify the minus sign with $P(L)$ from part a.

The printed form can be recovered by explicitly using the opposite slope coordinate $\widetilde\theta=-dx/dz$. Then $\widetilde B=-B$, free space has $\widetilde B=-L$, and the same physical path is $l=L_0-(Ax^2+Dx'^2-2xx')/(2\widetilde B)$. Thus the sign can be a convention choice, but the printed minus sign must not be combined with the positive-$B$ free-space [ray transfer matrix](../../../../ray-transfer-matrix-analysis.md) used here.

For physical field propagation, the paraxial [diffraction](../../../../diffraction.md) kernel retains this quadratic optical-path [phase](../../../../phase-waves.md) while using the leading spreading [amplitude](../../../../wave-amplitude.md). In one transverse dimension the normalized [linear canonical transform](../../../../linear-canonical-transformation.md) is

$$
E(x')=\frac{e^{ikL_0}}{\sqrt{i\lambda B}}\int\exp\!\left[\frac{ik}{2B}(Ax^2+Dx'^2-2xx')\right]E(x)\,dx,
$$

with a consistent square-root branch and $\lambda=2\pi/k$. The source's prefactor and $1/l$ kernel are a schematic one-dimensional version of the [Fresnel-Kirchhoff diffraction integral](../../../../fresnel-kirchhoff-diffraction-integral.md), not this normalized general-system propagator. The quadratic denominator is normally replaced by its leading value when making the Fresnel approximation. When $B=0$, propagation is an imaging limit rather than an ordinary integral with division by $B$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
