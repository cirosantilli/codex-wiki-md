<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the completely elastic exterior, [radial elastic compatibility](../../../../radial-elastic-compatibility.md) makes $q+2t$ constant. The far-field [stress](../../../../stress.md) vanishes, so $q+2t=0$ and $t=-q/2$. Radial [force balance](../../../../force-balance.md) then gives $q'+3q/r=0$, whence $q=C/r^3$. The [pressure](../../../../pressure-split.md) [boundary condition](../../../../boundary-condition.md) is $q(a)=-P$: positive applied [pressure](../../../../pressure-split.md) is compressive. Therefore

$$
\boxed{\tau_{rr}=-P\frac{a^3}{r^3},\qquad
\tau_{\theta\theta}=\tau_{\phi\phi}=\frac P2\frac{a^3}{r^3}.}
$$

For completeness, the corresponding radial [displacement field](../../../../displacement-field-mechanics.md) is $u=Pa^3/(4\mu r^2)$, which gives these components through [Hooke's law](../../../../hooke-s-law.md) and decays at infinity.

The [Tresca yield criterion](../../../../tresca-yield-criterion.md) becomes

$$
f(r)=\frac12|q-t|=\frac{3P}{4}\frac{a^3}{r^3}.
$$

For $P\geq0$ this is largest at the cavity wall and decreases strictly with radius when $P>0$. The first [yield point](../../../../yield-point.md) is therefore at $r=a$, where $3P/4=\tau_Y$. Hence

$$
\boxed{P_c=\frac43\tau_Y,\qquad r_{\mathrm{first}}=a.}
$$

The normalization matters: $\tau_Y$ in this paper is a shear [yield stress](../../../../yield-stress.md), rather than the uniaxial [yield strength](../../../../yield-strength.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
