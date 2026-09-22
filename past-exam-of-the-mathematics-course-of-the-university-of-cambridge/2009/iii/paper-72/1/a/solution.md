<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Multiply by a [test function](../../../../../../test-function.md) vanishing at the endpoints and apply [integration by parts](../../../../../../integration-by-parts.md). The positive operator is $-u''+xu$, so the forcing changes sign. The [weak formulation](../../../../../../weak-formulation.md) of this [forced Airy boundary-value problem](../../../../../../forced-airy-boundary-value-problem.md) is: find $u\in V=H_0^1(0,1)$ such that

$$
\boxed{a(u,v)=\ell(v)\quad(v\in V),\qquad
a(u,v)=\int_0^1(u'v'+xuv)\,dx,\quad
\ell(v)=-\int_0^1v\,dx.}
$$

Here $V$ is the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md) and can be equipped with $\|v\|_V=\|v'\|_{L^2}$. The interval [Poincaré inequality](../../../../../../poincare-inequality.md) states $\|v\|_{L^2}\leq\pi^{-1}\|v'\|_{L^2}$, so this [norm](../../../../../../norm.md) makes $V$ a [Hilbert space](../../../../../../hilbert-space-split.md) and is equivalent to its usual $H^1$ [Sobolev norm](../../../../../../sobolev-norm.md). The form is symmetric and satisfies

$$
|a(u,v)|\leq(1+\pi^{-2})\|u\|_V\|v\|_V,\qquad
a(v,v)\geq\|v\|_V^2,\qquad
|\ell(v)|\leq\pi^{-1}\|v\|_V.
$$

The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) says that a bounded [coercive bilinear form](../../../../../../coercive-bilinear-form.md) on a [Hilbert space](../../../../../../hilbert-space-split.md) and a [bounded linear functional](../../../../../../continuous-linear-functional.md) determine exactly one weak solution. All its hypotheses have just been verified. Moreover, $u''=xu+1\in L^2$ gives $u\in H^2$ on the interval; the right-hand side is then continuous, so this weak solution is the classical solution with the prescribed endpoint values.

Since the form is symmetric, the equivalent [Ritz method](../../../../../../rayleigh-ritz-method.md) minimizes

$$
\boxed{J(v)=\frac12\int_0^1[(v')^2+xv^2]\,dx+\int_0^1v\,dx
\quad\text{over }H_0^1(0,1).}
$$

Indeed, stationarity gives the weak equation and

$$
J(v)-J(u)=\tfrac12a(v-u,v-u)\geq0,
$$

with equality only at $u$. This proves the minimization equivalence, including the sign of the linear term.

Restricting to a [conforming finite element space](../../../../../../conforming-finite-element-space.md) $V_h\subset V$ gives a unique discrete solution and [Galerkin orthogonality](../../../../../../galerkin-orthogonality.md), $a(u-u_h,v_h)=0$ for every $v_h\in V_h$. The [Céa lemma](../../../../../../cea-s-lemma.md) states that if the continuity and coercivity constants are $M$ and $\alpha$, then $\|u-u_h\|_V\leq(M/\alpha)\inf_{v_h\in V_h}\|u-v_h\|_V$. For this symmetric problem the exact best-approximation constant in the [energy norm](../../../../../../energy-norm.md) is one. The piecewise-linear [finite element interpolation estimate](../../../../../../finite-element-interpolation-estimate.md) $\|u-I_hu\|_{H^1}\leq Ch\|u\|_{H^2}$ on regular [finite element meshes](../../../../../../finite-element-mesh.md) therefore gives [convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) of the [Ritz method](../../../../../../rayleigh-ritz-method.md), with first-order error in the [energy norm](../../../../../../energy-norm.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
