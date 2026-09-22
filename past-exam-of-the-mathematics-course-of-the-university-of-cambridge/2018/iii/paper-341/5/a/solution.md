<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in the real [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md) $X=H_0^1(0,1)$, whose members have square-integrable [weak derivatives](../../../../../../weak-derivative.md) and zero endpoint trace. Define the [bounded bilinear form](../../../../../../bounded-bilinear-form.md) and [linear functional](../../../../../../linear-functional.md)

$$
a(u,v)=\int_0^1(u'v'+uv)\,dx,\qquad
\ell(v)=\int_0^1xv\,dx.
$$

The [weak formulation](../../../../../../weak-formulation.md) is to find $u\in X$ with $a(u,v)=\ell(v)$ for every $v\in X$. [Integration by parts](../../../../../../integration-by-parts.md) recovers the differential equation for a smooth solution; conversely, this identity is the definition of its [weak solution](../../../../../../weak-solution.md).

Use the full $H^1$ [norm](../../../../../../norm.md). The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|a(u,v)|\leq\|u\|_{H^1}\|v\|_{H^1}$ and $|\ell(v)|\leq\|v\|_{H^1}/\sqrt3$. Also $a(v,v)=\|v\|_{H^1}^2$, so $a$ is a [coercive bilinear form](../../../../../../coercive-bilinear-form.md) with constant one. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) states that a bounded, coercive bilinear form on a real [Hilbert space](../../../../../../hilbert-space-split.md) determines a unique weak solution for every bounded linear functional. It therefore applies here.

The equivalent minimization problem is

$$
\boxed{\min_{v\in H_0^1(0,1)}\mathcal E(v),\qquad
\mathcal E(v)=\frac12\int_0^1\bigl((v')^2+v^2\bigr)\,dx-\int_0^1xv\,dx.}
$$

If $u$ is the weak solution, symmetry and $a(u,v-u)=\ell(v-u)$ give

$$
\mathcal E(v)-\mathcal E(u)=\frac12a(v-u,v-u).
$$

This is positive unless $v=u$, proving a unique [global minimizer](../../../../../../global-minimizer.md). Conversely, differentiating $\mathcal E(u+tv)$ at $t=0$ gives the weak identity. Thus **the unique energy minimizer is exactly the unique [weak solution](../../../../../../weak-solution.md)**. As a check, the classical representative is

$$
\boxed{u(x)=x-\frac{\sinh x}{\sinh1}.}
$$

It satisfies both endpoint conditions and $-u''+u=x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
