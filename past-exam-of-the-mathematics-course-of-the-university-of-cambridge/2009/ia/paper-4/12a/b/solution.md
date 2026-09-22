<h1 id="12a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Place the four fixed charges at $(sa,ta)$ with $s,t\in\{-1,1\}$, and write the moving particle's position as $(x,y)$. Introduce its mass $m>0$, which is needed for an oscillation frequency but is not named in the question. Let $C=Qq/(4\pi\epsilon_0)>0$. By [Coulomb's law](../../../../../../coulomb-s-law.md) and superposition, the moving particle's [potential energy](../../../../../../potential-energy.md) is

$$
V(x,y)=C\sum_{s,t=\pm1}\left[2a^2-2a(sx+ty)+x^2+y^2\right]^{-1/2}.
$$

The [electrostatic potential](../../../../../../electric-potential.md) itself is $V/q$. Put $r^2=x^2+y^2$ and $\delta_{st}=-(sx+ty)/a+r^2/(2a^2)$. Near the centre, a [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
\left[2a^2-2a(sx+ty)+r^2\right]^{-1/2}=\frac1{\sqrt2a}\left(1-\frac12\delta_{st}+\frac38\delta_{st}^2+\cdots\right).
$$

On summing over the four corners, linear terms cancel. To quadratic order, $\sum\delta_{st}=2r^2/a^2$ and $\sum\delta_{st}^2=4r^2/a^2+O(r^4/a^4)$, since $\sum st=0$. Reflection symmetry removes all odd-degree terms. Hence

$$
V(x,y)=\frac{C}{\sqrt2a}\left(4+\frac{x^2+y^2}{2a^2}\right)+O\left(\frac{Cr^4}{a^5}\right)=V(0,0)+\frac12\kappa(x^2+y^2)+O(r^4),
$$

where

$$
\kappa=\frac{C}{\sqrt2a^3}>0.
$$

Thus the centre has zero planar force and a positive-definite planar [Hessian matrix](../../../../../../hessian-matrix.md) $\kappa I_2$. It is a strict local minimum of the constrained [potential energy](../../../../../../potential-energy.md), so it is a [stable equilibrium](../../../../../../stable-equilibrium.md). More explicitly, conservation of the total energy confines sufficiently small-energy motions within a small neighbourhood of this isolated local minimum.

Keeping only the quadratic potential, the two coordinates obey independent [small oscillations](../../../../../../small-oscillation.md):

$$
m\ddot x=-\kappa x,\qquad m\ddot y=-\kappa y.
$$

Both planar modes have the same [angular frequency](../../../../../../angular-frequency.md), and the ordinary [frequency](../../../../../../frequency.md) is

$$
\boxed{\omega=\sqrt{\frac{Qq}{4\pi\epsilon_0\sqrt2\,ma^3}},\qquad \nu=\frac{\omega}{2\pi}.}
$$

The planar constraint is essential to this [constrained electrostatic equilibrium](../../../../../../constrained-electrostatic-equilibrium.md). Along the perpendicular axis, $V(0,0,z)=4C/(2a^2+z^2)^{1/2}=V(0,0)-Cz^2/(\sqrt2a^3)+O(z^4)$, so the same stationary point is unstable to unconstrained normal displacements. That also checks the cancellation of the three-dimensional Hessian trace required by [Laplace's equation](../../../../../../laplace-equation.md) away from charges; it does not contradict the positive-definite restriction to the given plane.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12A](../../12a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
