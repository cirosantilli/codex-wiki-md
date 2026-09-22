<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [character of an algebra](../../../../../../character-of-an-algebra.md) is a nonzero complex-linear multiplicative map $\varphi:A\to\mathbb C$. The [character space of an algebra](../../../../../../character-space-of-an-algebra.md) $\Phi_A$ carries the [Gelfand topology](../../../../../../gelfand-topology.md), namely pointwise convergence on $A$, equivalently the subspace weak-star topology in $A^*$.

For a unital complex [Banach algebra](../../../../../../banach-algebra-split.md), $\varphi(1)=1$: multiplicativity and nonzeroness force this. If $a-\varphi(a)1$ were invertible, applying $\varphi$ to its product with its inverse would give $0=1$. Thus $\varphi(a)\in\sigma_A(a)$. The [Neumann series](../../../../../../neumann-series.md) shows $\sigma_A(a)\subset\{|z|\le\|a\|\}$, so $|\varphi(a)|\le\|a\|$ and the [character of an algebra](../../../../../../character-of-an-algebra.md) is automatically bounded. The same conclusion for a nonunital algebra follows by extending $\varphi$ to its [unitization of an algebra](../../../../../../unitization-of-an-algebra.md) via $\widetilde\varphi(a,t)=\varphi(a)+t$ and using the standard [norm](../../../../../../norm.md) $\|(a,t)\|=\|a\|+|t|$.

In the algebra $R(K)$ let $u(z)=z$ and fix $\varphi\in\Phi_{R(K)}$. Write $\lambda=\varphi(u)$. If $\lambda\notin K$, the [rational function](../../../../../../rational-function.md) $(u-\lambda)^{-1}$ belongs to $R(K)$, which is impossible because a [character of an algebra](../../../../../../character-of-an-algebra.md) cannot vanish on an invertible element. Thus $\lambda\in K$. For a [rational function](../../../../../../rational-function.md) $r=p/q$ without poles in $K$, choose a reduced denominator having no zeros in $K$. Multiplicativity gives $\varphi(r)=p(\lambda)/q(\lambda)=r(\lambda)$. Density of these [rational functions](../../../../../../rational-function.md) and boundedness of $\varphi$ then yield $\varphi(h)=h(\lambda)$ for every $h\in R(K)$.

Conversely, evaluation at each $\lambda\in K$ is a [character of an algebra](../../../../../../character-of-an-algebra.md). The map $\lambda\mapsto\delta_\lambda$ is continuous in the Gelfand topology because every $h\in R(K)$ is continuous; its inverse is $\varphi\mapsto\varphi(u)$, also continuous. Hence the [character space of R(K)](../../../../../../character-space-of-r-k.md) is

$$
\boxed{\Phi_{R(K)}\cong K,\qquad\varphi=\delta_\lambda.}
$$

The identification includes the topology, not merely a bijection of sets.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
