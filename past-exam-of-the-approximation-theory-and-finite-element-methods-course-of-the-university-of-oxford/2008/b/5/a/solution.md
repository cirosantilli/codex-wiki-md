<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Sobolev space](../../../../../sobolev-space-split.md) $H^1(0,1)$ consists of square-integrable [functions](../../../../../function-split.md) whose weak first [derivative](../../../../../derivative.md) is square-integrable, with [norm](../../../../../norm.md) $\|v\|_{H^1}^2=\int_0^1(v^2+v'^2)$. Its one-dimensional representatives have well-defined endpoint traces.

Multiplying by $v\in H^1$ and integrating by parts gives

$$
\int_0^1fv=\int_0^1(u'v'+\cos x\,uv)-u'(1)v(1)+u'(0)v(0).
$$

The two Robin conditions give $u'(0)=u(0)$ and $u'(1)=-u(1)$, so define

$$
a(u,v)=\int_0^1(u'v'+\cos x\,uv)+u(0)v(0)+u(1)v(1),\qquad
\ell(v)=\int_0^1fv.
$$

A [weak solution](../../../../../weak-solution.md) is $u\in H^1(0,1)$ satisfying $a(u,v)=\ell(v)$ for every $v\in H^1(0,1)$. The [boundary conditions](../../../../../boundary-condition.md) are natural; no endpoint [derivative](../../../../../derivative.md) is imposed in the trial space.

Since $\cos x\geq\cos1>0$ on this interval,

$$
\boxed{a(v,v)\geq\cos1\,\|v\|_{H^1}^2.}
$$

This proves [coercivity](../../../../../coercive-function.md) on the full space. Trace continuity and [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) give continuity of the form, so the [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) also ensures a unique [weak solution](../../../../../weak-solution.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
