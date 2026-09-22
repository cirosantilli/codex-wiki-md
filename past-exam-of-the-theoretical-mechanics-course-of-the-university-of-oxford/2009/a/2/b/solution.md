<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Von Mises boundary-layer transformation](../../../../../von-mises-boundary-layer-transformation.md) uses $\Psi$ as transverse coordinate. With $u=U(x,\Psi)$ and $\Psi_x=-V$, $\Psi_Y=u=U$, the [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{u_x=U_x-VU_\Psi,\qquad u_Y=UU_\Psi,\qquad u_{YY}=U\partial_\Psi(UU_\Psi).}
$$

The streamwise advection terms reduce to $u u_x+Vu_Y=UU_x$, so, for $Y>0$ where $U>0$, division by $U$ gives

$$
\boxed{U_x=\partial_\Psi(UU_\Psi).}
$$

Continuity was already enforced by the [stream function](../../../../../stream-function.md). Substitute $U=g(\eta)$ with $\eta=\Psi/\sqrt x$. Then $U_x=-\eta g'/(2x)$ and $\partial_\Psi(UU_\Psi)=(gg')'/x$, yielding

$$
\boxed{(gg')'+\tfrac12\eta g'=0,\qquad g(0)=0,\quad g(\infty)=1.}
$$

The wall coordinate is zero because $\Psi$ was set to zero there, and the far condition matches unit external speed. This is the transformed Blasius similarity problem. One must not additionally prescribe a finite $g'(0)$: the coordinate change degenerates at the no-slip wall, and the regular physical shear corresponds to $g\propto\sqrt\eta$ near zero. This similarity reduction is obtained for the attached monotone [boundary layer](../../../../../boundary-layer.md) assumed in the question.

Existence of a positive normalized profile can also be seen directly. Put $q=gg'$ and choose $q(0)=a>0$. In $g$ coordinates the regular initial-value system is $dq/dg=-\eta/2$, $d\eta/dg=g/q$, with $\eta(0)=0$. It starts as $g\sim\sqrt{2a\eta}$. For finite positive $\eta$, $q'/q=-\eta/(2g)$ keeps $q$ positive and $q\leq a$, while $(g^2)'=2q$ gives $g\leq\sqrt{2a\eta}$. Consequently $q'/q\leq-\sqrt\eta/(2\sqrt{2a})$, so $q$ is integrable at infinity. It follows that $g$ increases to a finite positive limit $M$. The rescaled profile $\widetilde g(\eta)=M^{-1}g(\sqrt M\eta)$ satisfies the same equation and has limit one. This supplies the requested similarity solution with both boundary conditions, rather than only its formal differential equation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
