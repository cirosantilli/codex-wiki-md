<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $V=H_0^1(\Omega;\mathbb R^3)$. For any $v\in V$ and any real $t$, $u+tv$ is admissible. Expanding the functional gives

$$
J(u+tv)-J(u)=t\bigl(a(u,v)-\ell(v)\bigr)+\frac{t^2}2a(v,v).
$$

Since the left side is nonnegative for positive and negative $t$, its [derivative](../../../../derivative.md) at zero vanishes. Thus the [first variation](../../../../first-variation.md) gives the [weak formulation](../../../../weak-formulation.md)

$$
\boxed{u\in V,\qquad a(u,v)=\ell(v)\quad(v\in V).}
$$

To identify its differential equation, define the [stress tensor](../../../../cauchy-stress-tensor.md)

$$
\sigma(u)=2\mu\varepsilon(u)+\lambda(\operatorname{div}u)I.
$$

This is a [symmetric matrix](../../../../symmetric-matrix.md) field. The [Frobenius inner product](../../../../frobenius-inner-product.md) of a [symmetric matrix](../../../../symmetric-matrix.md) with a [skew-symmetric matrix](../../../../skew-symmetric-matrix.md) is zero, so $\sigma(u):\nabla v=\sigma(u):\varepsilon(v)$. Since $\operatorname{tr}\varepsilon(v)=\operatorname{div}v$, we obtain

$$
a(u,v)=\int_\Omega\sigma(u):\nabla v.
$$

For smooth compactly supported [test functions](../../../../test-function.md), [integration by parts](../../../../integration-by-parts.md) in each row gives

$$
\int_\Omega\sigma(u):\nabla v=-\langle\operatorname{div}\sigma(u),v\rangle.
$$

Hence $-\operatorname{div}\sigma(u)=f$ as a [distributional identity](../../../../distributional-identity.md), that is,

$$
-2\mu\operatorname{div}\varepsilon(u)-\lambda\nabla(\operatorname{div}u)=f.
$$

Membership in $V$ supplies the zero [Sobolev trace](../../../../trace-operator.md). This identifies precisely the required [weak solution](../../../../weak-solution.md) of the [linear elasticity](../../../../linear-elasticity.md) problem, with row-wise [divergence](../../../../divergence.md).

For uniqueness, use the exact form of the [Korn inequality](../../../../korn-inequality.md) supplied in the paper. Put $E=\varepsilon(v)$ and $d=\operatorname{tr}E=\operatorname{div}v$. The [deviatoric strain](../../../../deviatoric-strain.md) is $D=E-\tfrac13dI$. Because $\operatorname{tr}D=0$ and $I:I=3$, [orthogonality](../../../../orthogonal-vectors.md) for the [Frobenius inner product](../../../../frobenius-inner-product.md) gives

$$
|E|_F^2=|D|_F^2+\frac13d^2,\qquad |D|_F^2\leq|E|_F^2.
$$

If $C_K$ is the supplied [Korn inequality](../../../../korn-inequality.md) constant and $K$ the permitted [Poincaré inequality](../../../../poincare-inequality.md) constant, then

$$
\|v\|_1^2\leq(1+K)\|\nabla v\|_0^2
\leq(1+K)C_K\|D\|_0^2
\leq(1+K)C_K\|\varepsilon(v)\|_0^2.
$$

Consequently,

$$
\boxed{a(v,v)\geq\alpha\|v\|_1^2,\qquad\alpha=\frac{2\mu}{(1+K)C_K}>0.}
$$

If $u_1,u_2$ are two [weak solutions](../../../../weak-solution.md), their difference $d_u\in V$ satisfies $a(d_u,v)=0$ for every $v\in V$. Choosing $v=d_u$ and using this [coercive bilinear form](../../../../coercive-bilinear-form.md) estimate forces $d_u=0$. The minimizer therefore gives the unique [weak solution](../../../../weak-solution.md).

For later use, $|\varepsilon(v)|_F\leq|\nabla v|_F$ and $|\operatorname{div}v|\leq\sqrt3|\nabla v|_F$ also give the [bounded bilinear form](../../../../bounded-bilinear-form.md) and [linear functional](../../../../linear-functional.md) estimates

$$
|a(p,v)|\leq(2\mu+3\lambda)\|p\|_1\|v\|_1,\qquad
|\ell(v)|\leq\|f\|_0\|v\|_1.
$$

Together with the [coercive bilinear form](../../../../coercive-bilinear-form.md) estimate and the [Lax-Milgram theorem](../../../../lax-milgram-theorem.md), these would establish existence independently of the assumed minimizer.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
