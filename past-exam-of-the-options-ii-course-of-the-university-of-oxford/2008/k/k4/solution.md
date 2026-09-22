<h1 id="k/k4/solution">Solution</h1>

↑ **Parent:** [K4](../k4.md)

Put $\kappa=Q/(2\pi)$, $a=1+i$ and $b=1/\bar a=a/2$. The circle theorem gives, up to an additive constant,

$$
W(z)=\kappa\{\log(z-a)+\log(z-b)-\log z\},\qquad q(z)=W'(z)=\kappa\left\{\frac1{z-a}+\frac1{z-b}-\frac1z\right\}.
$$

Thus an image source lies at $b$ and an image sink at zero. With a counterclockwise contour around the cylinder, Blasius' force theorem is

$$
F_x-iF_y=\frac{i\rho}{2}\oint q(z)^2\,dz.
$$

If $q=s/(z-z_0)+h(z)$ locally, the [residue](../../../../residue.md) of $q^2$ is $2s h(z_0)$. The enclosed poles are zero and $b$, with residues

$$
\operatorname{Res}_0q^2=2\kappa^2(1/a+1/b),\qquad
\operatorname{Res}_bq^2=2\kappa^2\{1/(b-a)-1/b\}.
$$

Their sum is $2\kappa^2\{1/a+1/(b-a)\}=-\kappa^2(1-i)$. The [residue theorem](../../../../residue-theorem.md) therefore yields

$$
\boxed{F_x-iF_y=\frac{\rho Q^2}{4\pi}(1-i),\qquad F_x=F_y=\frac{\rho Q^2}{4\pi}}.
$$

The force points towards the source. For the moment formula the double poles also contribute: $\operatorname{Res}_{z_0}(zq^2)=s^2+2z_0s h(z_0)$. Hence

$$
\sum\operatorname{Res}(zq^2)=\kappa^2+\kappa^2+2\kappa^2b\{1/(b-a)-1/b\}=
2\kappa^2\frac{b}{b-a}=-2\kappa^2.
$$

It follows that $\oint zq^2\,dz=-4\pi i\kappa^2$ and

$$
\boxed{M=0,\qquad N=-2\pi\rho\kappa^2=-\frac{\rho Q^2}{2\pi}}.
$$

The zero [torque](../../../../torque.md) agrees with pressure acting normally to a circle, hence radially through its centre.

## ↑ Ancestors (12)

1. [K4](../k4.md)
2. [K](../../k.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
