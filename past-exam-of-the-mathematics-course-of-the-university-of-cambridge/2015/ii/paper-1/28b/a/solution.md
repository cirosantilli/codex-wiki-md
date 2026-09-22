<h1 id="28b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Lyapunov function](../../../../../../lyapunov-function.md) near an equilibrium is a continuously differentiable positive-definite function $V$, vanishing there, whose [derivative](../../../../../../derivative.md) along trajectories is nonpositive. The strict [Second Lyapunov theorem](../../../../../../second-lyapunov-theorem.md) says a negative-definite [derivative](../../../../../../derivative.md) implies local asymptotic stability.

For sharper bounds than the circular test $x^2+y^2$, put $z=(x,y)^T$, $r^2=z^Tz$ and

$$
A=\begin{pmatrix}-1&1\\-2&-1\end{pmatrix},\quad
P=\begin{pmatrix}4/3&-1/6\\-1/6&5/6\end{pmatrix},\quad V=z^TPz.
$$

A direct multiplication gives $A^TP+PA=-2I$. Its [eigenvalues](../../../../../../eigenvalue.md) are $\lambda_\pm=(13\pm\sqrt{13})/12>0$. Since the nonlinear vector field is $Az+r^2z$,

$$
\boxed{\dot V=2r^2(V-1)}.
$$

For $0<V<1$, the [derivative](../../../../../../derivative.md) is strictly negative. The Lyapunov theorem proves asymptotic stability. In fact $V(0)<1$ gives $V(t)\leq V(0)$ and

$$
\dot V\leq-\frac{2(1-V(0))}{\lambda_+}V,
$$

so the solution stays bounded, exists for all positive time and converges exponentially to zero.

The ellipse $V=1$ is invariant. In polar coordinates, $\dot\theta=-(2\cos^2\theta+\sin^2\theta)<0$, so it is a nonconstant periodic orbit, not part of the basin. For $V(0)>1$, use $r^2\geq V/\lambda_+$ to obtain $\dot V\geq2V(V-1)/\lambda_+$. This implies finite-time blow-up by comparison with the scalar equation. Thus the exact basin is $\{V<1\}$ and every point outside its closure escapes to unbounded norm within its maximal existence interval.

The largest open disc centred at zero lying in this exact basin has radius

$$
\boxed{r_1=\lambda_+^{-1/2}=\sqrt{\frac{12}{13+\sqrt{13}}}}.
$$

The smallest radius such that every point strictly outside its circle escapes is the largest radius on the invariant ellipse:

$$
\boxed{r_2=\lambda_-^{-1/2}=\sqrt{\frac{12}{13-\sqrt{13}}}}.
$$

These are optimal: a larger attraction disc contains a periodic-orbit point, and a smaller escape threshold leaves a periodic-orbit point in its exterior. This is an [exact quadratic basin boundary](../../../../../../exact-quadratic-basin-boundary.md).

The simpler radial [derivative](../../../../../../derivative.md) is $\tfrac12(d/dt)r^2=r^2(r^2-1)-xy$. It only certifies attraction for $r<1/\sqrt2$ and strictly increasing norm for $r>\sqrt{3/2}$. Those are optimal thresholds for a sign test on that radial [derivative](../../../../../../derivative.md), not for the actual attraction and escape regions. If “increases without bound” is read as requiring monotonic increase from the initial instant, the smallest such uniform radius is $\sqrt{3/2}$: at direction $x=y$, any smaller threshold permits an initially decreasing norm. The sharper $r_2$ above concerns eventual unbounded escape, which need not be monotone at every instant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28B](../../28b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
