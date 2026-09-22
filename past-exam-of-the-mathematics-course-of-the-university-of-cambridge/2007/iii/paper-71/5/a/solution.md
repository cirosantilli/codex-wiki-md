<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with real functions and $f\in L^2(0,1)$. To give the variational problem a definite domain, choose the homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) used in the next part. The natural form space is the [zero-trace Sobolev space](../../../../../../zero-trace-sobolev-space.md) $H=H_0^1(0,1)$, with norm $\|v\|_H=\|v'\|_2$. The [Sobolev trace operator](../../../../../../trace-operator.md) is well defined because one-dimensional $H^1$ functions have absolutely continuous representatives. For example $v(0)=\int_0^1v(x)dx-\int_0^1(1-x)v'(x)dx$, so its endpoint trace is bounded in the $H^1$ norm; the other endpoint has the analogous estimate. The zero-trace space is closed in the Hilbert space $H^1$, and the [Poincaré inequality](../../../../../../poincare-inequality.md) $\|v\|_2\leq\pi^{-1}\|v'\|_2$ makes the chosen derivative norm equivalent to its full norm. Thus $H$ is a Hilbert space.

Differentiability of $p,q$ implies continuity on the compact interval. Hence there are finite constants $p_{\max},q_{\max}$ and a positive $p_{\min}$ with $p_{\min}\leq p\leq p_{\max}$ and $0\leq q\leq q_{\max}$. Define the symmetric [bilinear form](../../../../../../bilinear-form.md)

$$
a(u,v)=\int_0^1[p(x)u'(x)v'(x)+q(x)u(x)v(x)]dx.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and [Poincaré inequality](../../../../../../poincare-inequality.md) give all the estimates required by the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md):

$$
|a(u,v)|\leq\left(p_{\max}+\frac{q_{\max}}{\pi^2}\right)\|u\|_H\|v\|_H,\qquad a(v,v)\geq p_{\min}\|v\|_H^2,\qquad|\langle f,v\rangle|\leq\frac{\|f\|_2}{\pi}\|v\|_H.
$$

That theorem states that a continuous coercive bilinear form on a Hilbert space and a bounded linear functional determine a unique weak solution. Completeness, continuity, [coercivity](../../../../../../coercive-function.md) and boundedness have now all been verified. Therefore there is a unique $u\in H$ with $a(u,v)=\langle f,v\rangle$ for every $v\in H$.

The energy version of the given [variational problem](../../../../../../variational-problem.md) is $I(v)=a(v,v)-2\langle f,v\rangle$. Its exact variation is

$$
I(v+w)-I(v)=2a(v,w)-2\langle f,w\rangle+a(w,w).
$$

Boundedness of $a$ makes the last term quadratic in $\|w\|_H$, so the [Fréchet derivative](../../../../../../frechet-derivative.md) is $DI(v)[w]=2a(v,w)-2\langle f,w\rangle$. Its vanishing for every test function is precisely

$$
\boxed{\int_0^1[pu'v'+quv]dx=\int_0^1fv\,dx\quad\text{for every }v\in H_0^1(0,1).}
$$

Taking compactly supported smooth tests and integrating in the distributional sense shows that this is the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) $-(pu')'+qu=f$. Conversely that weak equation gives the displayed stationary condition. The stationary point is actually the unique global minimizer, because

$$
\boxed{I(v)-I(u)=a(v-u,v-u)\geq p_{\min}\|v-u\|_H^2.}
$$

Equality occurs only when $v=u$. This proves the variational equivalence, including existence and uniqueness rather than only a formal derivative calculation.

For precision about the literal [L2 inner product](../../../../../../l2-inner-product.md) $\langle Lv,v\rangle$, use the [flux-domain realization of a one-dimensional elliptic operator](../../../../../../flux-domain-realization-of-a-one-dimensional-elliptic-operator.md)

$$
D(L)=\{v\in H_0^1(0,1):pv'\in H^1(0,1)\}.
$$

For such $v$, weak [integration by parts](../../../../../../integration-by-parts.md) and its zero endpoint values give $\langle Lv,v\rangle=a(v,v)$. On the larger form space $H$, the same energy is interpreted by the weak operator pairing. The minimizer belongs to $D(L)$ automatically: its weak equation gives $(pu')'=qu-f\in L^2$, while $pu'\in L^2$. Thus its equation also holds as an equality of $L^2$ functions. This domain does not assume bounded $p'$, which mere differentiability would not supply. If $p\in C^1$ one may equivalently use $D(L)=H^2\cap H_0^1$, but that stronger coefficient assumption is not needed for the proof here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
