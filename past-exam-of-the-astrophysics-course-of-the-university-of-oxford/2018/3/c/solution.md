<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep both component masses constant during a circular, gravitational-radiation-driven inspiral. Since $J=\mu\sqrt{GMA}$, differentiation gives $\dot J/J=\dot A/(2A)$. Combining this with the supplied angular-momentum loss yields

$$
\boxed{\dot A=-\frac{64}{5}\frac{G^3\mu M^2}{c^5A^3}\equiv-\frac K{A^3}.}
$$

The expression $A/\dot A$ printed in the source is negative during inspiral. A positive characteristic shrinking timescale is

$$
\boxed{\tau_A=\frac{A}{|\dot A|}=\frac{A^4}{K}
=\frac5{64}\frac{c^5A^4}{G^3\mu M^2}\propto A^4.}
$$

The actual remaining coalescence time follows by integrating $A^3\,dA=-K\,dt$:

$$
\boxed{t_{\mathrm{coal}}=\frac{A_0^4}{4K}=\frac{\tau_A(A_0)}4.}
$$

This constant factor does not change the requested separation scaling.

For an old, approximately coeval population, let $dN/dA_0=C$ over the relevant separation interval, and write the positive delay as $t_m=BA_0^4$. Conservation of event counts under this change of variable gives

$$
\nu_m(t_m)=\frac{dN}{dA_0}\left|\frac{dA_0}{dt_m}\right|
=\frac{C}{4B^{1/4}}t_m^{-3/4}.
$$

Therefore

$$
\boxed{\nu_m\propto t_m^{-3/4}.}
$$

The scaling applies between the minimum and maximum delays of the assumed separation distribution. It is a rate per delay interval, not the number per logarithmic delay interval.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
