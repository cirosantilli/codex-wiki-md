<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the real [Hilbert space](../../../../../../hilbert-space-split.md) $V=H_0^1(0,1)$, the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md), with [norm](../../../../../../norm.md) $\|v\|_V=\|v'\|_{L^2}$. The [Poincaré inequality](../../../../../../poincare-inequality.md) makes this equivalent to its usual [Sobolev space](../../../../../../sobolev-space-split.md) norm. Define the symmetric [bilinear form](../../../../../../bilinear-form.md) and continuous [linear functional](../../../../../../linear-functional.md)

$$
a(u,v)=\int_0^1\bigl(u'v'+xuv\bigr)\,dx,\qquad
\ell(v)=\int_0^1fv\,dx.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the sharp interval [Poincaré inequality](../../../../../../poincare-inequality.md) imply

$$
|a(u,v)|\leq(1+\pi^{-2})\|u\|_V\|v\|_V,\qquad
a(v,v)\geq\|v\|_V^2,\qquad
|\ell(v)|\leq\pi^{-1}\|f\|_{L^2}\|v\|_V.
$$

Thus $a$ is a [bounded bilinear form](../../../../../../bounded-bilinear-form.md) and a [coercive bilinear form](../../../../../../coercive-bilinear-form.md), and $\ell$ is bounded because $f$ is [square-integrable](../../../../../../square-integrable-function.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) supplies a unique [weak solution](../../../../../../weak-solution.md):

$$
\boxed{y\in H_0^1(0,1),\qquad a(y,v)=\ell(v)\quad\text{for every }v\in H_0^1(0,1)}.
$$

This is obtained from the differential equation by [integration by parts](../../../../../../integration-by-parts.md); the test functions have zero boundary trace. Conversely, the [weak solution](../../../../../../weak-solution.md) satisfies $y''=xy-f$ in the sense of [distributions](../../../../../../distribution-mathematical-analysis.md). Since $xy-f\in L^2$, it belongs to $H^2(0,1)\cap H_0^1(0,1)$ and solves the equation [almost everywhere](../../../../../../almost-everywhere.md).

Equivalently, the [Ritz method](../../../../../../rayleigh-ritz-method.md) minimizes

$$
J(v)=\frac12\int_0^1\bigl((v')^2+xv^2\bigr)\,dx-\int_0^1fv\,dx
$$

over $V$. Indeed $J(y+w)-J(y)=a(w,w)/2$, since the mixed term is $a(y,w)-\ell(w)=0$. This proves existence and uniqueness of the minimizer directly from the [weak solution](../../../../../../weak-solution.md), as well as its equivalence to the [variational problem](../../../../../../variational-problem.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
