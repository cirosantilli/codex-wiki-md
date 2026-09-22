<h1 id="17a/solution">Solution</h1>

↑ **Parent:** [17A](../17a.md)

For a boost of speed $v$ in the $x$ direction, with

$$
\gamma=\frac1{\sqrt{1-v^2/c^2}},
$$

the [Lorentz transformation of electromagnetic fields](../../../../../lorentz-transformation-of-electromagnetic-fields.md) is

$$
\begin{array}{lll}
E'_x=E_x,&E'_y=\gamma(E_y-vB_z),&E'_z=\gamma(E_z+vB_y),\\
B'_x=B_x,&B'_y=\gamma(B_y+vE_z/c^2),&B'_z=\gamma(B_z-vE_y/c^2).
\end{array}
$$

Expanding $E'_yB'_y+E'_zB'_z$, the mixed terms cancel and the remaining transverse terms acquire the factor $\gamma^2(1-v^2/c^2)=1$. Together with the unchanged longitudinal product, this proves the Lorentz invariant

$$
\boxed{\mathbf E'\cdot\mathbf B'=\mathbf E\cdot\mathbf B}.
$$

An independent invariant is

$$
\boxed{E^2-c^2B^2}.
$$

If only $E_y=E$ and $B_y=B$ are nonzero, then

$$
\mathbf E'=(0,\gamma E,\gamma vB),
\qquad
\mathbf B'=(0,\gamma B,-\gamma vE/c^2),
$$

and direct subtraction gives

$$
E'^2-c^2B'^2
=\gamma^2(1-v^2/c^2)(E^2-c^2B^2)
=E^2-c^2B^2.
$$

Now put $cB=\lambda E$ and $\beta=v/c$. Invariance of the dot product gives $\mathbf E'\cdot\mathbf B'=\lambda E^2/c$, while the displayed components give

$$
E'^2=\gamma^2E^2(1+\lambda^2\beta^2),
\qquad
B'^2=\frac{\gamma^2E^2}{c^2}(\lambda^2+\beta^2).
$$

Hence

$$
\boxed{\cos\theta=
\frac{\lambda(1-\beta^2)}{sqrt{(1+\lambda^2\beta^2)(\lambda^2+\beta^2)}}}.
$$

At $\beta=0$ this equals $\operatorname{sgn}\lambda$, and as $|\beta|\uparrow1$ it tends continuously to zero with the same sign. Thus boosts realize every $0\leq\theta<\pi/2$ when $\lambda>0$, and every $\pi/2<\theta\leq\pi$ when $\lambda<0$.

## ↑ Ancestors (10)

1. [17A](../17a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
