<h1 id="a/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $u=\psi_Y$, $V=-\psi_x$, and put $\eta=Y/x^\gamma$, $\psi=x^\beta f(\eta)$. Then

$$
u=x^{\beta-\gamma}f',\qquad V=-x^{\beta-1}(\beta f-\gamma\eta f').
$$

Matching $u\sim x^m$ requires $\beta-\gamma=m$. Equating the powers in streamwise [inertia](../../../../../inertia.md) $x^{2m-1}$ and transverse diffusion $x^{m-2\gamma}$ gives

$$
\boxed{\gamma=\frac{1-m}{2},\qquad\beta=\frac{1+m}{2}.}
$$

The two convective terms combine to $x^{2m-1}[m(f')^2-\beta f f'']$, while $UU'=mx^{2m-1}$. Hence the [Falkner-Skan equation](../../../../../falkner-skan-equation.md) in this scaling is

$$
\boxed{f^{(3)}+\beta f f''+m[1-(f')^2]=0,\quad f(0)=f'(0)=0,\quad f'(\infty)=1.}
$$

The additive stream-function constant is fixed by $f(0)=0$; when $\beta\ne0$ this also encodes [no penetration](../../../../../no-penetration-boundary-condition.md). For $\beta=0$ it is a harmless choice of additive constant choice. Existence of an attached physical branch for a given $m$ is a separate issue from deriving the similarity reduction.

On an attached branch with $w=f'>0$ away from the wall, use $f$ itself as the independent variable. The [chain rule](../../../../../chain-rule.md) gives $f''=w w_f$ and $f^{(3)}=w(w_f^2+w w_{ff})$. Therefore

$$
\boxed{w^2w_{ff}+w(w_f)^2+\beta f w w_f+m(1-w^2)=0,\qquad w(0)=0,\quad w(f)\to1\text{ as }f\to\infty.}
$$

If the [wall shear](../../../../../wall-shear-stress.md) $s=f''(0)>0$, then $f\sim s\eta^2/2$, so $w(f)\sim\sqrt{2sf}$. Thus $w_f$ is singular at zero while $w w_f\to s$ is finite. Imposing a finite arbitrary $w_f(0)$ would remove the usual attached branch. This is the [velocity as dependent variable in the Falkner-Skan equation](../../../../../velocity-as-dependent-variable-in-the-falkner-skan-equation.md) reduction.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
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
