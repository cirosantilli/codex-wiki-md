<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use anti-Hermitian gauge potentials and the convention $D_i=\partial_i+A_i$ for the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md). Commuting these operators defines the [gauge field strength](../../../../../gauge-field-strength.md):

$$
\boxed{F_{xy}=\partial_xA_y-\partial_yA_x+[A_x,A_y].}
$$

It is antisymmetric in its two spacetime indices, so $F_{xx}=F_{yy}=0$ and $F_{yx}=-F_{xy}$. In two dimensions there is therefore only one independent component, although that component is itself Lie-algebra valued.

Put $B_x=(\partial_xg)g^{-1}$ and $B_y=(\partial_yg)g^{-1}$. Differentiating $g^{-1}$ gives $\partial_i g^{-1}=-g^{-1}(\partial_i g)g^{-1}$. Equality of mixed derivatives then gives the right [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md)

$$
\partial_xB_y-\partial_yB_x=B_xB_y-B_yB_x=[B_x,B_y].
$$

Consequently the [scaled right Maurer-Cartan gauge potential](../../../../../scaled-right-maurer-cartan-gauge-potential.md) has curvature

$$
\boxed{F_{xy}=\alpha(1+\alpha)[B_x,B_y]
=\alpha(1+\alpha)\bigl((\partial_xg)g^{-1}(\partial_yg)g^{-1}-(\partial_yg)g^{-1}(\partial_xg)g^{-1}\bigr).}
$$

Thus **$\alpha=0$ and $\alpha=-1$ give zero curvature for every smooth $g$**. At zero the potential is zero. At minus one it is a [pure gauge potential](../../../../../pure-gauge-potential.md): transforming the zero connection by $g$ gives $A=-dg\,g^{-1}$. If the gauge Lie algebra is abelian, the [commutator](../../../../../commutator.md) vanishes for every $\alpha$. If it contains $X,Y$ with $[X,Y]\ne0$, choose $g(x,y)=e^{xX}e^{yY}$; at the origin $B_x=X$ and $B_y=Y$. Thus in that case the two displayed values are the only choices flat for every $g$. If the potential is instead defined using $D=\partial-A$ and field components $\partial_xA_y-\partial_yA_x-[A_x,A_y]$, the same calculation reads $\alpha(1-\alpha)[B_x,B_y]$ and the nonzero pure-gauge value is $+1$. The sign convention must be specified.

For the specified [SU(2)](../../../../../su-2-group.md) exponential, let $r=\sqrt{x^2+y^2}$ and, away from the origin, $n=(x/r,y/r,0)$. The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives $(n\cdot\sigma)^2=I$, so summing the exponential series yields

$$
g=\cos(r/2)I-i\sin(r/2)(n\cdot\sigma).
$$

The continuous extension at the origin is $I$. For $r>0$, the second term is zero precisely when $\sin(r/2)=0$, and hence

$$
\boxed{g=I\text{ at }r=0,\qquad g=(-1)^kI\text{ on }r=2\pi k,\quad k=1,2,\ldots.}
$$

These are infinitely many distinct circles.

At the origin, differentiating the exponential at zero gives $B_x=t_1$ and $B_y=t_2$. Since $[t_1,t_2]=t_3=-i\sigma_3/2$, the [gauge field strength](../../../../../gauge-field-strength.md) there is

$$
\boxed{F_{xy}(0,0)=-\frac{i}{2}\alpha(1+\alpha)\sigma_3.}
$$

To evaluate it on the circles, use polar coordinates. On $r=2\pi k$ the angular derivative of $g$ vanishes, while $B_r=-i(n\cdot\sigma)/2$. Therefore $B_x=(x/r)B_r$ and $B_y=(y/r)B_r$ commute, and **$F_{xy}=0$ everywhere on every such circle, for every $\alpha$**.

One can also see these [circular curvature zeros for a planar SU2 exponential](../../../../../circular-curvature-zeros-for-a-planar-su2-exponential.md) from a formula valid away from the origin. Write $n=(\cos\vartheta,\sin\vartheta,0)$, $m=(-\sin\vartheta,\cos\vartheta,0)$, and $t_n=-i(n\cdot\sigma)/2$, $t_m=-i(m\cdot\sigma)/2$. Direct differentiation gives

$$
B_r=t_n,\qquad B_\vartheta=\sin r\,t_m+(1-\cos r)t_3,
$$

and hence

$$
[B_x,B_y]=\frac1r[B_r,B_\vartheta]=\frac{\sin r}{r}t_3-\frac{1-\cos r}{r}t_m.
$$

Both coefficients vanish at the positive circle radii, and the expression tends to $t_3$ at the origin, agreeing with the direct calculation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
