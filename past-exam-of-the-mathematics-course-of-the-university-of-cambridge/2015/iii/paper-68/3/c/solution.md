<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is a genuine conflict in the printed coefficient assumptions: [no uniformly positive coefficient in a zero-boundary Sobolev space](../../../../../../no-uniformly-positive-coefficient-in-a-zero-boundary-sobolev-space.md) exists. A function $a\in H_0^1(\Omega)$ cannot also obey $a\geq a_->0$ almost everywhere. Indeed, the Lipschitz truncation $g(s)=\min(\max(s,0),a_-)$ has $g(0)=0$, so [Lipschitz truncation preserves zero-boundary Sobolev spaces](../../../../../../lipschitz-truncation-preserves-zero-boundary-sobolev-spaces.md), giving $g(a)\in H_0^1(\Omega)$. But $g(a)$ would be the nonzero constant $a_-$. Its zero [gradient](../../../../../../gradient.md) contradicts the [Poincaré inequality](../../../../../../poincare-inequality.md) in the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md). Thus the literal coefficient class is empty.

For the meaningful uniformly elliptic problem, take $a\in L^\infty(\Omega)$ with $0<a_-\leq a\leq a_+$, and impose the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) on the unknown and test functions: $V=H_0^1((0,1)^2)$. Additional $H^1$ regularity of $a$ is harmless, but a zero trace for $a$ must be removed. The [divergence-form elliptic operator](../../../../../../divergence-form-elliptic-operator.md) is $L=-\operatorname{div}(a\nabla)$. [Integration by parts](../../../../../../integration-by-parts.md) defines the symmetric [bounded bilinear form](../../../../../../bounded-bilinear-form.md)

$$
 B(v,w)=\int_\Omega a\,\nabla v\cdot\nabla w\,dx\,dy.
$$

In particular,

$$
 B(v,v)\geq a_-\|\nabla v\|_2^2\geq 2\pi^2a_-\|v\|_2^2,
 \qquad |B(v,w)|\leq a_+\|\nabla v\|_2\|\nabla w\|_2.
$$

Here $2\pi^2$ is the first [Dirichlet Laplacian eigenvalue](../../../../../../dirichlet-laplacian-eigenvalue.md) on the unit square; the [Poincaré inequality](../../../../../../poincare-inequality.md) follows, for example, by applying the one-dimensional inequality in each coordinate and adding. Thus $B$ is coercive in the [gradient](../../../../../../gradient.md) [norm](../../../../../../norm.md) on $V$, and the Dirichlet realization of $L$ is a [positive definite symmetric operator](../../../../../../positive-definite-symmetric-operator.md). On its [operator domain](../../../../../../operator-domain.md), $\langle Lv,v\rangle=B(v,v)$.

The required functional and weak equation are

$$
\boxed{I(v)=\int_\Omega\left(a|\nabla v|^2-2fv\right)\,dx\,dy,\qquad v\in H_0^1(\Omega),}
$$



$$
\boxed{\int_\Omega a\nabla u\cdot\nabla w=\int_\Omega fw
\quad\text{for every }w\in H_0^1(\Omega).}
$$

Because $f\in L^2$, the right side is a bounded [linear functional](../../../../../../linear-functional.md) by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and [Poincaré inequality](../../../../../../poincare-inequality.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) gives a unique [weak solution](../../../../../../weak-solution.md), and part (b) proves that it uniquely minimizes $I$. These formulas prove the intended conclusion under the repaired coefficient hypothesis; under the literal hypothesis there is no coefficient to which the conclusion can be applied.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
