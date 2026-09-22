<h1 id="11a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\eta=\psi-\phi$. The common [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) gives $\eta=0$ on $S$. Expanding the [energy functional](../../../../../../energy-functional.md),

$$
\begin{aligned}
E[\psi]-E[\phi]
={}&\int_V\left(|\nabla\eta|^2+m^2\eta^2\right)dV\\
&+2\int_V\left(\nabla\phi\cdot\nabla\eta
+m^2\phi\eta\right)dV.
\end{aligned}
$$

[Integration by parts](../../../../../../integration-by-parts.md) and the field equation make the cross term zero:

$$
\int_V\left(\nabla\phi\cdot\nabla\eta+m^2\phi\eta\right)dV
=\int_S\eta\frac{\partial\phi}{\partial n}\,dS
-\int_V\eta(\nabla^2\phi-m^2\phi)\,dV
=0.
$$

Consequently

$$
\boxed{
E[\psi]-E[\phi]
=\int_V\left(|\nabla\eta|^2+m^2\eta^2\right)dV\geq0}.
$$

For $m>0$, equality holds exactly when $\eta=0$. For $m=0$, equality holds exactly when $\nabla\eta=0$, so $\eta$ is constant on the connected region; its zero boundary value then again forces $\eta=0$. The minimizing property therefore proves uniqueness for the Dirichlet problem in both cases:

$$
\boxed{\psi=\phi\text{ is the equality condition for every }m\geq0}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
