<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For two solutions with the same initial datum, let $h=f_1-f_2$. Their uniform [compact support](../../../../../../compact-support.md) on $[0,T]$ puts $h$ and $h_t$ in one compact region of [phase space](../../../../../../phase-space.md). Smoothness there implies that $E(t)=\int |h(t,x,v)|^2\,dx\,dv$ is finite and continuously differentiable, by [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md). The [transport equation](../../../../../../transport-equation.md) and [integration by parts](../../../../../../integration-by-parts.md) in $x$ yield

$$
E'(t)=-2\int h\,a(v)\cdot\nabla_xh\,dx\,dv
=-\int a(v)\cdot\nabla_x(h^2)\,dx\,dv=0.
$$

There is no boundary contribution because of [compact support](../../../../../../compact-support.md), and $\operatorname{div}_x a(v)=0$. Since $E(0)=0$, $h=0$ almost everywhere and then everywhere by [continuity](../../../../../../continuous-function.md). **The solution is unique in $\mathcal C_T$.** The same calculation gives [Lp conservation for incompressible transport](../../../../../../lp-conservation-for-incompressible-transport.md) at $p=2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
