<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

The quotient $h=f/g$ is a [holomorphic function](../../../../../holomorphic-function.md) because the denominator has no zeros, and $|h|=1$. Write $h=u+iv$. The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) say $u_y=-v_x$ and $v_y=u_x$. Differentiating $u^2+v^2=1$ in both real directions gives

$$
uu_x+vv_x=0,\qquad -uv_x+vu_x=0.
$$

The coefficient [determinant](../../../../../determinant.md) is $-(u^2+v^2)=-1$, so $u_x=v_x=0$, and the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) also give $u_y=v_y=0$. Thus $h$ is locally constant. Since a [domain](../../../../../domain-mathematical-analysis.md) is connected, it is constant throughout $\Omega$. Its constant value has modulus one and can be written $e^{i\alpha}$ with $\alpha\in\mathbb R$. Therefore **$f=e^{i\alpha}g$ throughout $\Omega$**.

This is the [constant-modulus holomorphic function](../../../../../constant-modulus-holomorphic-function.md) principle. Connectedness is essential to a single global phase: on two disjoint discs, taking $g=1$ and choosing $f=1$ on one disc and $f=-1$ on the other gives equal moduli without one common phase.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
