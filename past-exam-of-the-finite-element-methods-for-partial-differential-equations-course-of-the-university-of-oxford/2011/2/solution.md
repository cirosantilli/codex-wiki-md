<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A real [bilinear form](../../../bilinear-form-split.md) is a [coercive bilinear form](../../../coercive-bilinear-form.md) on $V$ when $a(v,v)\geq\alpha\|v\|_V^2$ for all $v\in V$ and some fixed $\alpha>0$. It is a [bounded bilinear form](../../../bounded-bilinear-form.md), equivalently continuous, when $|a(v,w)|\leq M\|v\|_V\|w\|_V$ for one finite $M$. A continuous [linear functional](../../../linear-functional.md) satisfies $|\ell(v)|\leq C_\ell\|v\|_V$.

The [Galerkin method](../../../galerkin-method.md) seeks $u_h\in S$ with $a(u_h,v_h)=\ell(v_h)$ for all $v_h\in S$. Subtraction from the continuous equations gives [Galerkin orthogonality](../../../galerkin-orthogonality.md): $a(u-u_h,v_h)=0$ for every $v_h\in S$. Under the stated continuity and coercivity assumptions, [Céa's lemma](../../../cea-s-lemma.md) says

$$
\boxed{\|u-u_h\|_V\leq\frac M\alpha\inf_{v_h\in S}\|u-v_h\|_V.}
$$

Indeed, with $e=u-u_h$ and any $v_h\in S$, [Galerkin orthogonality](../../../galerkin-orthogonality.md) eliminates $v_h-u_h$:

$$
\alpha\|e\|_V^2\leq a(e,e)=a(e,u-v_h)\leq M\|e\|_V\|u-v_h\|_V.
$$

If $e=0$ the claim is immediate; otherwise cancel $\|e\|_V$ and take the [infimum](../../../infimum.md). No symmetry of $a$ was used. These statements define an approximation when it exists; a finite-dimensional $S$ gives existence and uniqueness by the [Lax-Milgram theorem](../../../lax-milgram-theorem.md), as does a closed [vector subspace](../../../vector-subspace.md).

For the interval example write $L=c-b$ and $R=\max(|b|,|c|)$. The [one-dimensional Sobolev representative](../../../one-dimensional-sobolev-representative.md) of $v\in V$ satisfies

$$
v(x)=-\int_x^cv'(t)\,dt,\qquad |v(x)|^2\leq(c-x)\int_x^c|v'(t)|^2\,dt\leq(c-x)\|v'\|_2^2
$$

by the [Cauchy-Schwarz inequality](../../../cauchy-schwarz-inequality.md). The representation follows by taking the [absolutely continuous function](../../../absolutely-continuous-function.md) primitive of the [weak derivative](../../../weak-derivative.md); its difference from $v$ has zero [weak derivative](../../../weak-derivative.md), hence is constant, and $v(c)=0$ fixes that constant. Integrating the estimate gives the [Endpoint Poincaré inequality](../../../endpoint-poincare-inequality.md)

$$
\|v\|_2^2\leq\frac{L^2}{2}\|v'\|_2^2,\qquad
\|v\|_V^2\leq\left(1+\frac{L^2}{2}\right)\|v'\|_2^2.
$$

Thus the nonnegative potential $x^2$ gives

$$
\boxed{a(v,v)\geq\|v'\|_2^2\geq\frac1{1+L^2/2}\|v\|_V^2.}
$$

For continuity, $|x|\leq R$, the [Cauchy-Schwarz inequality](../../../cauchy-schwarz-inequality.md) for the two integrals, and then its two-dimensional version give

$$
|a(u,v)|\leq R^2\|u\|_2\|v\|_2+\|u'\|_2\|v'\|_2\leq\boxed{\max(1,R^2)\|u\|_V\|v\|_V}.
$$

Similarly $\boxed{|\ell(v)|\leq\|f\|_2\|v\|_2\leq\|f\|_2\|v\|_V}$, proving continuity of the [linear functional](../../../linear-functional.md).

For the last displayed integral take $\Omega=(-1,1)$ and retain the endpoint condition $v(1)=0$, the domain-consistent interpretation of the changed formula. **The changed form is still coercive.** A negative potential on part of the interval does not by itself destroy coercivity. The sharper pointwise estimate above gives

$$
\int_{-1}^0(-x)v(x)^2\,dx\leq\left[\int_{-1}^0(-x)(1-x)\,dx\right]\|v'\|_2^2=\frac56\|v'\|_2^2.
$$

Discarding only the positive part of the potential yields

$$
a(v,v)=\int_{-1}^1(v'^2+xv^2)\,dx\geq\frac16\|v'\|_2^2.
$$

The proved [Endpoint Poincaré inequality](../../../endpoint-poincare-inequality.md) with $L=2$ gives $\|v\|_V^2\leq3\|v'\|_2^2$, and therefore

$$
\boxed{a(v,v)\geq\frac1{18}\|v\|_V^2.}
$$

This is a concrete application of [negative-potential domination by endpoint control](../../../negative-potential-domination-by-endpoint-control.md). The constant is sufficient, without claiming to be optimal.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2011](../../2011-split.md)
3. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../split.md)
4. [Finite element methods for partial differential equations course of the University of Oxford](../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
