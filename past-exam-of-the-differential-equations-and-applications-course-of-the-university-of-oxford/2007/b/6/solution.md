<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In vector form the system is $U_x+A(U)U_y=C(U)$, with

$$
A=\begin{pmatrix}u&2\\2v&u\end{pmatrix},\qquad
C=\binom1{\sqrt v}.
$$

For $v>0$, its two real distinct [eigenvalues](../../../../eigenvalue.md) are $\boxed{\lambda_\pm=u\pm2\sqrt v}$, with [left eigenvectors](../../../../left-eigenvector.md) $\ell_\pm^T=(1,\pm1/\sqrt v)$. Thus the system is strictly hyperbolic there; at $v=0$ the [eigenvalues](../../../../eigenvalue.md) coincide and the matrix is defective, so [strict hyperbolicity](../../../../strict-hyperbolicity.md) fails. The [characteristic directions](../../../../characteristic-direction.md) are $dy/dx=\lambda_\pm$.

If $\dot y=\lambda_\pm\dot x$, multiplication of $\dot U=U_x\dot x+U_y\dot y$ by the [left eigenvector](../../../../left-eigenvector.md) gives $\ell_\pm^T\dot U=\ell_\pm^TC\dot x$. Since $d(u\pm2\sqrt v)=du\pm dv/\sqrt v$, define

$$
R=u-2\sqrt v,\qquad S=u+2\sqrt v.
$$

Then

$$
\boxed{R_x+RR_y=0,\qquad S_x+SS_y=2.}
$$

Consequently $R$ is constant on the minus [characteristic curves](../../../../characteristic-curve.md), and $S-2x$ is constant on the plus [characteristic curves](../../../../characteristic-curve.md). One reconstructs $\boxed{u=(R+S)/2,\quad v=(S-R)^2/16}$, with the essential physical constraint $S\geq R$.

For the data on $y=0$, the nonnegative [square root](../../../../square-root.md) gives

$$
R_0(\xi)=\xi+\tfrac12-|\xi-1|,\qquad
S_0(\xi)=\xi+\tfrac12+|\xi-1|.
$$

Thus, on any regular patch, use the two footpoints determined by

$$
\boxed{y=R_0(\xi)(x-\xi),\qquad
 y=(x-\eta)^2+S_0(\eta)(x-\eta),}
$$

and put $R=R_0(\xi)$, $S=2(x-\eta)+S_0(\eta)$, selecting branches continuous from the initial point. These implicit algebraic formulas determine the local answer wherever both [characteristic curve](../../../../characteristic-curve.md) [projections](../../../../projection-linear-algebra.md) are regular and $S>R$.

For example, near an initial point with $x>1$, they give $R=3/2$, $S=2x-1/2$, so $\boxed{u=x+1/2,\quad v=(x-1)^2/4}$. On an initial interval $x<1$, define $H=\sqrt{9/4+4y}$. One instead has $S=H$ and

$$
\boxed{R=x-\tfrac14+\operatorname{sgn}(x_0-\tfrac14)\sqrt{(x-\tfrac14)^2-2y},\quad
u=\tfrac12(R+H),\quad v=(H-R)^2/16,}
$$

near the chosen initial point $x_0\ne1/4$. The radicands must be positive, the footpoints must stay in their indicated initial intervals, and $H>R$ must hold.

**There is no continuously differentiable solution realizing the first data set on the entire stated initial line.** At $(x,y)=(1/4,0)$, $u=3/4$, $\sqrt v=3/8$, $u_x=1$ and $v_x=-3/8$. The minus [left eigenvector](../../../../left-eigenvector.md) is $(1,-8/3)$ and its [eigenvalue](../../../../eigenvalue.md) is zero. The differential equation there would require $\ell_-^TU_x=\ell_-^TC$, but its two sides are respectively $2$ and $0$. This is an explicit compatibility contradiction, not merely a loss of a preferred formula. Also, the proposed simple expression independent of $y$ does not solve the equation for $x<1$, because then $v_x<0$ but $\sqrt v>0$.

For the second data set, treat $x$ as the evolution variable and let $\eta$ label the initial $y$ coordinate. Then $R_0(\eta)=4\min(\eta,0)$ and $S_0(\eta)=4\max(\eta,0)$. In the positive quadrant the minus [characteristic curves](../../../../characteristic-curve.md) give $R=0$. The plus [characteristic curves](../../../../characteristic-curve.md) satisfy $S=2x+S_0(\eta)$ and $y=\eta+x^2+xS_0(\eta)$. Therefore their continuous [characteristic curve](../../../../characteristic-curve.md) continuation is

$$
\boxed{u=\begin{cases}
x,&0<y<x^2,\\
\dfrac{x+2x^2+2y}{1+4x},&y>x^2,
\end{cases}\qquad v=\frac{u^2}{4}.}
$$

Above the parabola the footpoint is $\eta=(y-x^2)/(1+4x)>0$; below it the plus footpoint is $\eta=y-x^2<0$. Each branch directly satisfies both equations and $v>0$. They agree continuously on $y=x^2$, but their $y$ [derivatives](../../../../derivative.md) are $0$ and $2/(1+4x)$, respectively. Thus **the continuation is piecewise classical and not continuously differentiable across the parabola**. The source's globally continuously differentiable formulation needs this qualification. If only positive initial $y$ is intended, the upper rational formula is a classical continuation throughout the positive quadrant, but the region $y<x^2$ requires incoming information from $y=0$ and is not determined by that positive half of the initial line alone. This illustrates [loss of differentiability from square-root hyperbolic source data](../../../../loss-of-differentiability-from-square-root-hyperbolic-source-data.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
