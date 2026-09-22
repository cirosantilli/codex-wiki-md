<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Introduce the positive outlet constant

$$
J=\lim_{\eta\downarrow0}f(\eta)f'(\eta).
$$

For a draining [similarity profile](../../../../../similarity-profile.md), $J$ is finite and positive. A regular linear profile would have $ff'\to0$ and $(ff')'\geq0$ at the origin, incompatible with the [rain-fed aquifer similarity solution](../../../../../rain-fed-aquifer-similarity-solution.md) $(ff')'(0)=-1$. Instead there is a [square-root drainage boundary](../../../../../square-root-drainage-boundary.md). At leading order, $(f^2)'=2ff'\to2J$, giving

$$
\boxed{f(\eta)\sim\sqrt{2J\eta},\qquad
f'(\eta)\sim\sqrt{\frac{J}{2\eta}}.}
$$

More explicitly, the [rain-fed aquifer similarity solution](../../../../../rain-fed-aquifer-similarity-solution.md) implies $(ff')'=-1+O(\sqrt\eta)$, hence $ff'=J-\eta+O(\eta^{3/2})$ and $f^2=2J\eta-\eta^2+O(\eta^{5/2})$. The height vanishes but its [derivative](../../../../../derivative.md) diverges; their product remains finite.

Use $t_d,x_d,h_d$ temporarily for dimensional quantities. The [nondimensionalization](../../../../../nondimensionalization.md) in part (a) gives

$$
h_d=\frac R\phi t_d f(\eta),\qquad
\eta=\frac{\phi x_d}{\sqrt{KR}\,t_d},\qquad
\partial_{x_d}h_d=\sqrt{\frac RK}f'(\eta).
$$

Taking the drainage flux to be positive out of the left-hand end, $Q_0=-q(0,t_d)$, gives

$$
\boxed{Q_0(t_d)=K\lim_{x_d\downarrow0}h_d\partial_{x_d}h_d
=\frac{\sqrt K\,R^{3/2}}\phi\,t_d
\lim_{\eta\downarrow0}f(\eta)f'(\eta)
=\frac{\sqrt K\,R^{3/2}}\phi Jt_d.}
$$

The printed expression in terms of $f(0)$ and $f'(0)$ must be understood as this limit; a literal product of their separate endpoint values is undefined. This is discharge per unit transverse width. Very close to the river, the divergent slope marks the limit of the [Dupuit approximation](../../../../../dupuit-approximation.md), while the outer solution still supplies the leading discharge.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
