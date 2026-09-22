<h1 id="section-b/b6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use coordinates $(ct,x,y,z)$ and put $\beta=v/c$, $\gamma=(1-\beta^2)^{-1/2}$. For an observer moving at $+v\widehat{\mathbf x}$, the coordinate [Lorentz boost](../../../../../lorentz-boost.md) is

$$
\Lambda=\begin{pmatrix}\gamma&-\beta\gamma&0&0\\-\beta\gamma&\gamma&0&0\\0&0&1&0\\0&0&0&1\end{pmatrix}.
$$

The given [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) transforms as $F'=\Lambda F\Lambda^{\mathsf T}$. For example,

$$
F'^{02}=\gamma F^{02}-\beta\gamma F^{12}=-\frac\gamma c(E_y-vB_z),\qquad
F'^{03}=\gamma F^{03}-\beta\gamma F^{13}=-\frac\gamma c(E_z+vB_y),
$$

while

$$
F'^{12}=-\beta\gamma F^{02}+\gamma F^{12}=-\gamma(B_z-vE_y/c^2),\qquad
F'^{13}=-\beta\gamma F^{03}+\gamma F^{13}=\gamma(B_y+vE_z/c^2).
$$

The $01$ component is unchanged because its boost [determinant](../../../../../determinant.md) is $\gamma^2(1-\beta^2)=1$. The $23$ component is unchanged because neither index lies in the boost plane. Reading off all six components gives

$$
\boxed{\begin{aligned}
E'_x&=E_x,&B'_x&=B_x,\\
E'_y&=\gamma(E_y-vB_z),&B'_y&=\gamma(B_y+vE_z/c^2),\\
E'_z&=\gamma(E_z+vB_y),&B'_z&=\gamma(B_z-vE_y/c^2).
\end{aligned}}
$$

The signs follow the stated positive observer [velocity](../../../../../velocity.md) and the supplied [tensor](../../../../../tensor.md) convention. In vector form for a boost in any direction, $\mathbf E'_\parallel=\mathbf E_\parallel$, $\mathbf E'_\perp=\gamma(\mathbf E_\perp+\mathbf v\times\mathbf B)$, with analogous $\mathbf B'_\perp=\gamma(\mathbf B_\perp-\mathbf v\times\mathbf E/c^2)$.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
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
