<h1 id="j/j1/solution">Solution</h1>

↑ **Parent:** [J1](../j1.md)

In SI units, [Gauss's law](../../../../gauss-s-law.md) for a closed surface with outward unit [normal vector](../../../../normal-vector.md) is

$$
\oint_S\mathbf E\cdot\mathbf n\,dS=\frac1{\varepsilon_0}\int_{\operatorname{inside}(S)}\rho\,dV=Q_{\rm enclosed}/\varepsilon_0.
$$

Spherical symmetry and the absence of an imposed external field make the [electric field](../../../../electric-field-split.md) radial, $\mathbf E=E_r(r)\mathbf e_r$. For $0\leq r\leq a$ (with the physical radius $a>0$),

$$
Q(r)=4\pi K\int_0^r(a^2s^2-s^4)\,ds=4\pi K\left(\frac{a^2r^3}{3}-\frac{r^5}{5}\right).
$$

Outside the charge distribution this becomes $Q(a)=8\pi K a^5/15$. Applying [Gauss's law](../../../../gauss-s-law.md) on spheres gives

$$
\boxed{\mathbf E(\mathbf x)=\begin{cases}\displaystyle\frac K{\varepsilon_0}\left(\frac{a^2r}{3}-\frac{r^3}{5}\right)\mathbf e_r,&0<r\leq a,\\[3pt]\displaystyle\frac{2Ka^5}{15\varepsilon_0 r^2}\mathbf e_r,&r\geq a,\\0,&r=0.\end{cases}}
$$

Both formulas agree at $r=a$, and the first tends to zero at the origin. Thus **the total charge is $8\pi K a^5/15$**. Negative $K$ reverses the field direction. If the radius is zero the distribution vanishes; a negative value of $a$ gives no nonnegative-radius support under the printed piecewise inequalities and likewise gives the zero distribution.

## ↑ Ancestors (12)

1. [J1](../j1.md)
2. [J](../../j.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
