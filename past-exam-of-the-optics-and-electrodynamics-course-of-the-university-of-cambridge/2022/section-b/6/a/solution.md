<h1 id="section-b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix coordinates $x^\mu=(ct,x,y,z)$ and use the following convention for the contravariant [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md):

$$
F^{\mu\nu}=\begin{pmatrix}
0&-E_x/c&-E_y/c&-E_z/c\\
E_x/c&0&-B_z&B_y\\
E_y/c&B_z&0&-B_x\\
E_z/c&-B_y&B_x&0
\end{pmatrix}.
$$

For $O'$ moving with [velocity](../../../../../velocity.md) $+v\widehat{\mathbf x}$ relative to $O$, the [Lorentz transformation](../../../../../lorentz-transformation.md) has

$$
\Lambda=\begin{pmatrix}
\gamma&-\beta\gamma&0&0\\
-\beta\gamma&\gamma&0&0\\
0&0&1&0\\
0&0&0&1
\end{pmatrix},\qquad
\beta=\frac vc,\quad\gamma=(1-\beta^2)^{-1/2}.
$$

The rank-two [tensor](../../../../../tensor.md) transformation rule is

$$
F'^{\mu\nu}=\Lambda^\mu{}_{\alpha}\Lambda^\nu{}_{\beta}F^{\alpha\beta},\qquad
F'=\Lambda F\Lambda^{\mathsf T}.
$$

For example,

$$
F'^{02}=\gamma F^{02}-\beta\gamma F^{12}
=-\frac\gamma c(E_y-vB_z),
$$



$$
F'^{12}=-\beta\gamma F^{02}+\gamma F^{12}
=-\gamma\left(B_z-\frac v{c^2}E_y\right).
$$

Similarly, $F'^{03}=-\gamma(E_z+vB_y)/c$ and $F'^{13}=\gamma(B_y+vE_z/c^2)$. The $01$ component is unchanged because $\gamma^2(1-\beta^2)=1$, and the $23$ component is unchanged since neither index lies in the boost plane. Reading off the six field components gives

$$
\boxed{\begin{aligned}
E'_x&=E_x,& B'_x&=B_x,\\
E'_y&=\gamma(E_y-vB_z),&B'_y&=\gamma(B_y+vE_z/c^2),\\
E'_z&=\gamma(E_z+vB_y),&B'_z&=\gamma(B_z-vE_y/c^2).
\end{aligned}}
$$

An alternative overall sign convention for $F^{\mu\nu}$ gives the same physical [Lorentz transformation of electromagnetic fields](../../../../../lorentz-transformation-of-electromagnetic-fields.md) when its identifications with $\mathbf E$ and $\mathbf B$ are used consistently.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
