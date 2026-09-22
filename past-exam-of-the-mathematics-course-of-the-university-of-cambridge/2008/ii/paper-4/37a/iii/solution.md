<h1 id="37a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The thin-layer condition is

$$
\boxed{C=(\nu^2/F)^{1/3}\ll1,\quad\text{equivalently }F\gg\nu^2.}
$$

Integrate the differential equation once: $(f''+ff')'=0$. Since $f(0)=f''(0)=0$, its integration constant is zero. A second integration gives $f'+f^2/2=b$. The outward-jet solution with $b>0$ and $f(0)=0$ is

$$
f=2k\tanh(k\eta),\qquad f'=2k^2\operatorname{sech}^2(k\eta),\qquad b=2k^2.
$$

Using the given fourth-power integral in the normalization gives $1=4k^4[4/(3k)]=16k^3/3$, so $k=(3/16)^{1/3}$. Thus the [similarity profile of an axisymmetric radial viscous free jet](../../../../../../similarity-profile-of-an-axisymmetric-radial-viscous-free-jet.md) is

$$
\boxed{u_r(r,z)=\frac{(9F^2/(32\nu))^{1/3}}r\,
\operatorname{sech}^2\left[(3F/(16\nu^2))^{1/3}\frac zr\right].}
$$

It is symmetric, outward, decays in $z$, and has exactly the conserved flux $F$. It describes the region beyond the small injection slit where the stated boundary-layer approximation applies; its formal $r=0$ singularity is outside that approximation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [37A](../../37a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
