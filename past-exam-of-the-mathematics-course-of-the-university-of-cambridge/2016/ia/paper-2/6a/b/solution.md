<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For real parameters, work on $x>0$ so arbitrary real powers are unambiguous. Taking [derivatives](../../../../../../derivative.md) gives

$$
y_1'=-\gamma x^{\gamma-1}\sin(x^\gamma),\qquad y_1''=-\gamma(\gamma-1)x^{\gamma-2}\sin(x^\gamma)-\gamma^2x^{2\gamma-2}\cos(x^\gamma).
$$

The residual after substitution is

$$
\bigl(1-a\gamma^2x^{\alpha+2\gamma-2}\bigr)\cos(x^\gamma)-\gamma\bigl(a(\gamma-1)+b\bigr)x^{\alpha+\gamma-2}\sin(x^\gamma).
$$

When $\gamma\ne0$, $x^\gamma$ ranges over $(0,\infty)$. Evaluating at the zeros of the cosine first forces the sine coefficient to vanish; then the cosine coefficient vanishes identically. If $\gamma=0$, the nonzero constant $\cos1$ cannot satisfy the equation. Thus the necessary and sufficient conditions are

$$
\boxed{\gamma\ne0,\qquad \alpha=2-2\gamma,\qquad a=\gamma^{-2},\qquad b=(1-\gamma)\gamma^{-2}.}
$$

Under these conditions the normalized coefficient is $p=(1-\gamma)/x$. The [Abel identity](../../../../../../abel-s-identity.md) gives $W=Cx^{\gamma-1}$. Choose $C=\gamma$ and apply [reduction of order](../../../../../../reduction-of-order.md) on an interval where $\cos(x^\gamma)\ne0$:

$$
y_2=\cos(x^\gamma)\int\frac{\gamma x^{\gamma-1}}{\cos^2(x^\gamma)}\,dx=\cos(x^\gamma)\tan(x^\gamma).
$$

The substitution $u=x^\gamma$ evaluates the [integral](../../../../../../integral.md). After continuation across the cosine zeros,

$$
\boxed{y_2(x)=\sin(x^\gamma),\qquad W(y_1,y_2)=\gamma x^{\gamma-1}\ne0.}
$$

This is a [power substitution for an oscillatory second-order equation](../../../../../../power-substitution-for-an-oscillatory-second-order-equation.md): in the variable $u=x^\gamma$, the equation reduces to the [harmonic oscillator equation](../../../../../../simple-harmonic-motion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
