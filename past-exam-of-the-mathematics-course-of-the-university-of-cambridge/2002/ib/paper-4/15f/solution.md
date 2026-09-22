<h1 id="15f/solution">Solution</h1>

↑ **Parent:** [15F](../15f.md)

The [dual space](../../../../../dual-space.md) $V^*$ consists of all real [linear functionals](../../../../../linear-functional.md) on $V$. If $v_1,\ldots,v_d$ is a [basis](../../../../../basis.md), its [dual basis](../../../../../dual-basis.md) $\varepsilon^1,\ldots,\varepsilon^d$ is characterized by $\varepsilon^i(v_j)=\delta_{ij}$; explicitly $\varepsilon^i$ extracts the $i$th coordinate. The natural map $J:V\to V^{**}$ is $J(v)(\phi)=\phi(v)$. It is linear and injective, because the coordinate functionals separate nonzero vectors, and both spaces have dimension $d$. Hence it is an isomorphism. Its definition uses no choice of [basis](../../../../../basis.md), which is the meaning of “naturally” here.

Evaluation $e_x(p)=p(x)$ is linear, so belongs to $V_n^*$. For distinct nodes $x_i$, define the [Lagrange interpolation polynomials](../../../../../lagrange-polynomial.md)

$$
\ell_i(t)=\prod_{j\ne i}\frac{t-x_j}{x_i-x_j}.
$$

They lie in $V_n$ and obey $e_{x_j}(\ell_i)=\delta_{ij}$. Applying a putative relation $\sum a_ie_{x_i}=0$ to $\ell_j$ gives $a_j=0$, so the $n+1$ evaluations are independent and form a [basis](../../../../../basis.md) of $V_n^*$. The [polynomials](../../../../../polynomial-split.md) $\ell_i$ give their dual [basis](../../../../../basis.md) in $V_n$, using the canonical identification with $V_n^{**}$.

Every $p\in V_n$ has the interpolation expansion $p(t)=\sum_i p(x_i)\ell_i(t)$: the difference has $n+1$ distinct roots but degree at most $n$. Integrate to get the [numerical integration](../../../../../numerical-integration.md) weights $\lambda_i=\int_{-1}^1\ell_i(t)dt$. For the specified symmetric five nodes, symmetry gives weights $(a,b,c,b,a)$. Exactness on $1,t^2,t^4$ gives

$$
2a+2b+c=2,\qquad 2a+\frac b2=\frac23,\qquad 2a+\frac b8=\frac25.
$$

Odd moments vanish automatically. Solving yields [Boole's rule](../../../../../boole-s-rule.md)

$$
\boxed{(\lambda_1,\ldots,\lambda_5)=\frac1{45}(7,32,12,32,7).}
$$

## ↑ Ancestors (10)

1. [15F](../15f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
