<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $L=-d^2/dx^2+x$. The [Airy equation](../../../../../../airy-equation.md) is $Lu=0$. To discuss positivity of this [linear operator](../../../../../../linear-operator.md), use its homogeneous variation domain $D(L)=\{v\in H^2(0,1):v(0)=0,\ v'(1)=0\}$. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
\langle v,Lv\rangle_{L^2}=\int_0^1\bigl(|v'|^2+x|v|^2\bigr)dx>0\qquad(v\ne0).
$$

The boundary term is zero at both ends. The same calculation with two different functions proves that the associated form is a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md). Positivity here concerns the homogeneous domain; the condition $u(0)=1$ instead defines an affine set of admissible solutions.

For the [variational problem](../../../../../../variational-problem.md) define

$$
V=\{v\in H^1(0,1):v(0)=0\},\qquad a(v,w)=\int_0^1(v'w'+xvw)dx,
$$

and minimize

$$
\boxed{J[u]=\frac12\int_0^1(u'^2+xu^2)dx\quad\text{over }u\in1+V.}
$$

The [Sobolev trace](../../../../../../trace-operator.md) at zero is meaningful in $H^1$. No [derivative](../../../../../../derivative.md) boundary value is imposed on this trial space: the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) will emerge naturally. For $v\in V$, [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and integration give

$$
|v(x)|^2\le x\int_0^x|v'(s)|^2ds,\qquad
\|v\|_2^2\le\tfrac12\|v'\|_2^2,
$$

so $a(v,v)\ge\tfrac23\|v\|_{H^1}^2$. Thus $a$ is a bounded, symmetric, [coercive bilinear form](../../../../../../coercive-bilinear-form.md) on the [Hilbert space](../../../../../../hilbert-space-split.md) $V$. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) says that a bounded [coercive bilinear form](../../../../../../coercive-bilinear-form.md) and a bounded [linear functional](../../../../../../linear-functional.md) determine a unique [weak solution](../../../../../../weak-solution.md). Apply it to

$$
a(v,w)=-\int_0^1xw\,dx\qquad(w\in V),
$$

and set $u=1+v$. This is precisely the [first variation](../../../../../../first-variation.md) condition $a(u,w)=0$ for $J$.

Compactly supported [test functions](../../../../../../test-function.md) first yield $u''=xu$ in the sense of [distributional derivatives](../../../../../../distributional-derivative.md). Since $xu\in L^2$, the solution is in $H^2$. [Integration by parts](../../../../../../integration-by-parts.md) then leaves $u'(1)w(1)=0$ for every $w\in V$, hence $u'(1)=0$. The other [boundary condition](../../../../../../boundary-condition.md) is built into $1+V$. Conversely a solution of this [boundary value problem](../../../../../../boundary-value-problem.md) satisfies the [first variation](../../../../../../first-variation.md) condition. Finally,

$$
J[u+w]-J[u]=a(u,w)+\tfrac12a(w,w)=\tfrac12a(w,w)>0\qquad(0\ne w\in V).
$$

This proves existence, uniqueness and the global minimum characterization, including the natural [boundary condition](../../../../../../boundary-condition.md). It is the [mixed-boundary Airy energy principle](../../../../../../mixed-boundary-airy-energy-principle.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
