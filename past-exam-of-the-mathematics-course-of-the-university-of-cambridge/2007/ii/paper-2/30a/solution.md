<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

The following unheaded requests concern the spherical measure, the wave solution and both uniqueness arguments. The missing part (i) above and this root Solution slot restore their coverage while retaining the existing part (ii) anchor.

For $k=|\xi|$, rotational symmetry of the spherical measure gives

$$
\widehat A_t(\xi)=2\pi t^2\int_{-1}^1e^{-itks}\,ds
=\boxed{4\pi t\frac{\sin(tk)}k},
$$

with continuous value $4\pi t^2$ at $k=0$. The spatial [Fourier transform](../../../../../fourier-transform.md) of the [wave equation](../../../../../wave-equation-split.md) gives $\widehat u_{tt}+k^2\widehat u=0$ with initial data zero and $\widehat g$. Thus $\widehat u=\sin(tk)\widehat g/k$. The [convolution theorem](../../../../../convolution-theorem.md) gives the [Kirchhoff formula](../../../../../kirchhoff-formula.md)

$$
\boxed{u(t,x)=\frac1{4\pi t}\int_{|y|=t}g(x-y)\,d\Sigma(y)
=\frac t{4\pi}\int_{S^2}g(x+t\omega)\,d\omega.}
$$

It is smooth for Schwartz data, solves the transformed equation, and has $u(0,x)=0$, $u_t(0,x)=g(x)$ by the second expression and its small-time limit.

To prove uniqueness for arbitrary $C^2$ solutions, take their difference $v$, with zero initial data, and set $e=(v_t^2+|\nabla v|^2)/2$, $p=-v_t\nabla v$. Direct differentiation gives $e_t+\nabla\cdot p=v_t(v_{tt}-\Delta v)=0$. For any centre $x_*$ and radius $R$, integrate over the shrinking ball $B(x_*,R-t)$. Differentiating the moving-domain energy gives

$$
\frac d{dt}\int_{B(x_*,R-t)}e
=\int_{\partial B(x_*,R-t)}(v_t\partial_nv-e)\le0,
$$

since $v_t\partial_nv\le(v_t^2+|\nabla v|^2)/2$. Initial energy is zero and energy is nonnegative, so it stays zero. In each such cone $v_t$ and $\nabla v$ vanish, and the initial value is zero, hence $v=0$. Choosing $R>T$ and arbitrary centre proves uniqueness at any time $T$, without imposing finite total energy or decay on the competing solution.

For the equation with the smooth positive time-independent potential $V$, use instead

$$
e_V=\frac12(v_t^2+|\nabla v|^2+Vv^2),\qquad p=-v_t\nabla v.
$$

Then $\partial_te_V+\nabla\cdot p=v_t(v_{tt}-\Delta v+Vv)=0$. The same shrinking-ball estimate is nonpositive because $Vv^2\ge0$. Zero initial data therefore give $v=0$. **The potential-wave initial-value problem has at most one $C^2$ solution**, with no global energy-growth assumption required. Time [independence](../../../../../independent-random-variables.md) of $V$ is what makes this particular local energy identity exact.

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
