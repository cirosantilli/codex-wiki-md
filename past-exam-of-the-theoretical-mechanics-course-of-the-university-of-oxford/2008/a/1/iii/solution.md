<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $\mathbf u=(u(y),0)$ and no imposed streamwise [pressure gradient](../../../../../pressure-gradient.md). The normal [momentum balance](../../../../../momentum-balance-for-a-material-fluid-element.md) gives $p=p_* -\rho gy\cos\alpha$. The streamwise equation is $\mu u''+\rho g\sin\alpha=0$, since the convective acceleration vanishes. With [no slip](../../../../../no-slip-boundary-condition.md) at the lower wall and signed upper-wall traction $\tau$ in the positive $x$ direction, the conditions are

$$
u(0)=0,\qquad\mu u'(h)=\tau.
$$

Integration gives

$$
\boxed{u(y)=\frac{\rho g\sin\alpha}{2\mu}y(2h-y)+\frac\tau\mu y,\quad\beta=\frac\rho{2\mu},\quad\gamma=2h+\frac{2\tau}{\rho g\sin\alpha}.}
$$

The required upper-wall [velocity](../../../../../velocity.md) is its endpoint value $u(h)=\rho gh^2\sin\alpha/(2\mu)+\tau h/\mu$. The unfactored formula remains meaningful when $\sin\alpha=0$.

The fluid exerts shear $\boxed{\mu u'(0)=\rho gh\sin\alpha+\tau}$ per unit length on the lower plane in the positive $x$ direction. The [force](../../../../../force-split.md) of that plane on the fluid has the opposite sign. The total wall [force](../../../../../force-split.md) on the fluid balances its downslope weight, providing an independent sign check.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
