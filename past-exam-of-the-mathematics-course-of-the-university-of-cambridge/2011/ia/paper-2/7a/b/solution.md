<h1 id="7a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Direct calculation gives

$$
W=(1+\cos x)\cos x+\sin^2x=1+\cos x.
$$

Where $1+\cos x\ne0$, [Abel identity](../../../../../../abel-s-identity.md) gives $p=-W'/W=\sin x/(1+\cos x)$, and substitution of either solution gives $q=1/(1+\cos x)$. Thus

$$
\boxed{p(x)=\tan(x/2),\qquad q(x)=\frac1{1+\cos x},\qquad W(\pi)=0.}
$$

These coefficients have singularities at odd multiples of $\pi$. This does not contradict the [Wronskian](../../../../../../wronskian.md) criterion: its continuous-coefficient interval hypothesis fails at those points.

On $0\le x<\pi$, the initial conditions uniquely select $y=\sin x$. **The normalized differential equation is not defined on the whole interval $0\le x<\infty$**, so the usual global [uniqueness theorem for ordinary differential equations](../../../../../../uniqueness-theorem-for-ordinary-differential-equations.md) cannot give the global initial-value assertion as posed. No choice of finite coefficients at $\pi$ can repair the normalized equation while retaining both displayed solutions: at that point $1+\cos x$ and its first derivative vanish, but its second derivative equals one.

The [continuation through a zero of the leading ODE coefficient](../../../../../../continuation-through-a-zero-of-the-leading-ode-coefficient.md) is a different problem: consider the multiplied, degenerate equation

$$
(1+\cos x)y''+\sin x\,y'+y=0.
$$

For this different equation, a globally $C^2$ solution with the given initial data is uniquely $\sin x$. On each regular interval every solution is $A_j(1+\cos x)+B_j\sin x$; continuity of $y'$ and $y''$ at an odd multiple of $\pi$ forces both constants to agree across it. If only $C^1$ piecewise solutions away from the singular points are required, the $A_j$ may change and uniqueness fails. Thus the coefficient singularity and the intended solution regularity must be distinguished.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7A](../../7a.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
