<h1 id="9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The source diagram has $2R$ in series with two parallel branches: one containing $R$ then $L$, and the other containing $2R$. Let their common voltage be $u(t)$, measured from the upper node to the lower return. [Kirchhoff's current law](../../../../kirchhoff-node-law.md) and the branch laws give

$$
I_0=I_1+I_2,\qquad u=2RI_2=RI_1+L\frac{dI_1}{dt},\qquad V=2RI_0+u.
$$

Using $I_2=u/(2R)$ in the source equation yields $u=V/2-RI_1$. Substitution into the coil branch gives

$$
\boxed{L\frac{dI_1}{dt}+2RI_1=\frac V2.}
$$

The switch was open for a long time, so $I_1(0^-)=0$. [Inductor current continuity](../../../../inductor-current-continuity.md) gives $I_1(0^+)=0$ for a finite applied voltage.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [9](../../9.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
