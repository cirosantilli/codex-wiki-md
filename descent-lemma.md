# Descent lemma

↑ **Parent:** [Lipschitz gradient](lipschitz-gradient.md)

Suppose $f$ is a [differentiable function](differentiable-function.md) on an open [convex set](convex-set-split.md) $D\subseteq\mathbb R^n$ and has an $L$-[Lipschitz gradient](lipschitz-gradient.md) there, in the [Euclidean norm](euclidean-norm.md). For $u,v\in D$, the [descent lemma](descent-lemma.md) states

$$
f(v)\leq f(u)+\langle\nabla f(u),v-u\rangle+\frac L2\|v-u\|_2^2.
$$

A bounded continuous [Hessian matrix](hessian-matrix.md) gives one sufficient route to this estimate.[§9.1.2, p. 461, equation (9.13): Hessian upper bound and quadratic upper estimate; §9.3.1, p. 466, equation (9.17): substitution of a negative-gradient step](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

For a short proof, put $d=v-u$. The [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) along the [line segment](line-segment.md) gives

$$
f(v)-f(u)-\langle\nabla f(u),d\rangle
=\int_0^1\langle\nabla f(u+td)-\nabla f(u),d\rangle\,dt.
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) and the [Lipschitz gradient](lipschitz-gradient.md) bound make the [integrand](integrand.md) at most $Lt\|d\|_2^2$; its [integral](integral-split.md) is $L\|d\|_2^2/2$. This proof needs no assumption that $f$ is a [convex function](convex-function.md).

For the [gradient descent](gradient-descent-split.md) update $v=u-\eta\nabla f(u)$, provided $v\in D$, substitution yields

$$
f(v)\leq f(u)-\eta\left(1-\frac{L\eta}{2}\right)\|\nabla f(u)\|_2^2.
$$

For $L>0$ and $0<\eta<2/L$, this ensures strict decrease whenever the [gradient](gradient.md) is nonzero. At $\eta=2/L$ it guarantees only nonincrease; the quadratic example has a nonshrinking alternating component at this endpoint. At $\eta=1/L$ the guaranteed decrease is $\|\nabla f(u)\|_2^2/(2L)$. A bound valid only on $D$ cannot justify a step leaving $D$.

If a fixed admissible [step size](step-size.md) is used forever, every iterate stays in $D$, and $f(x_k)$ has a finite lower bound, summing this inequality shows $\sum_k\|\nabla f(x_k)\|_2^2<\infty$, hence $\nabla f(x_k)\to0$. That conclusion alone gives neither convergence of the iterates nor a [global minimum](global-minimum.md). For example, the smooth [polynomial](polynomial-split.md) $f(x)=x^4-x^2$ has $f'(0)=0$ and $f''(0)=-2$: [gradient descent](gradient-descent-split.md) started at zero never moves, although $f(1/\sqrt2)=-1/4<0$. On $D=(-1,1)$, $|f''(x)|\leq10$, so the [Lipschitz gradient](lipschitz-gradient.md) hypothesis holds on this domain. [Convex functions](convex-function.md) and [strongly convex functions](strongly-convex-function.md) provide additional structure; the exact quadratic convergence result above uses a [positive-definite matrix](positive-definite-matrix.md).

## ↑ Ancestors (7)

1. [Lipschitz gradient](lipschitz-gradient.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Baillon–Haddad theorem](baillon-haddad-theorem.md)
- [Descent lemma](descent-lemma.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/2/iv/solution.md)
