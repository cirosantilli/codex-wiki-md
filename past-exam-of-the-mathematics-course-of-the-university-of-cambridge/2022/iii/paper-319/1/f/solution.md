<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

A [solution operator for a nonautonomous evolution equation](../../../../../../evolution-family.md) is an [evolution family](../../../../../../evolution-family.md) $U(t,s)$ satisfying

$$
U(s,s)=I,
\qquad
U(t,r)U(r,s)=U(t,s),
$$

and, on a suitable common domain $\mathcal D$,

$$
\partial_tU(t,s)u=A(t)U(t,s)u,
\qquad
\partial_sU(t,s)u=-U(t,s)A(s)u.
$$

One applicable nonautonomous generation theorem is the following. Suppose $\mathcal D$ is a dense linear subspace of $H$, each $A(t)$ has domain $\mathcal D$, the family is a [stable family of semigroup generators](../../../../../../stable-family-of-semigroup-generators.md) with constants $M,0$, and $t\mapsto A(t)$ is continuously differentiable as a map from $[0,T]$ to $\mathcal B(\mathcal D,H)$, where $\mathcal D$ carries one of the uniformly equivalent [graph norms](../../../../../../graph-norm.md). Then there is a unique [evolution family](../../../../../../evolution-family.md) such that:

- $(t,s)\mapsto U(t,s)u$ is continuous for every $u\in H$ and $\|U(t,s)\|\leq M$;
- $U(t,s)\mathcal D\subseteq\mathcal D$, with a uniform bound on $U(t,s)$ as an operator on $\mathcal D$;
- for $u\in\mathcal D$, both displayed differential equations hold in $H$.

For the uniform partition $t_j=s+j(t-s)/N$, the [frozen-generator product approximation](../../../../../../frozen-generator-product-approximation.md) is

$$
U_N(t,s)
=e^{(t_N-t_{N-1})A(t_{N-1})}
\cdots e^{(t_1-t_0)A(t_0)}.
$$

As $N\to\infty$, $U_N(t,s)u\to U(t,s)u$ in the norm of $H$ for every $u\in H$, uniformly for $(t,s)$ in the compact time triangle $0\leq s\leq t\leq T$. This is convergence in the [strong operator topology](../../../../../../strong-operator-topology.md), rather than convergence in the [operator norm](../../../../../../operator-norm.md).

It remains to verify the second differential equation. The [evolution family](../../../../../../evolution-family.md) law gives, for $h>0$,

$$
U(t,s+h)u-U(t,s)u
=U(t,s+h)\bigl[u-U(s+h,s)u\bigr].
$$

Divide by $h$. Since $u\in\mathcal D$,

$$
\frac{U(s+h,s)u-u}{h}\longrightarrow A(s)u,
$$

while [strong continuity](../../../../../../strong-continuity.md) gives $U(t,s+h)A(s)u\to U(t,s)A(s)u$. Therefore

$$
\boxed{\partial_sU(t,s)u=-U(t,s)A(s)u}.
$$

The left derivative follows in the same way, so $s\mapsto U(t,s)u$ is differentiable.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
