<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Give the closed oriented genus-$g$ surface $\Sigma_g$ its usual CW structure with one vertex, $2g$ one-cells $a_1,b_1,\ldots,a_g,b_g$, and one two-cell attached along $\prod_i[a_i,b_i]$. The cellular boundary maps vanish after abelianization, so

$$
H^q(\Sigma_g;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&q=0,2,\\
\mathbb Z^{2g},&q=1,\\
0,&\text{otherwise}.
\end{cases}
$$

Choose degree-one classes $\alpha_i,\beta_i$ dual to $a_i,b_i$ and orient $\Sigma_g$ by $\omega\in H^2$. The intersection pairing, equivalently the cellular diagonal approximation, gives the [cohomology ring of a closed oriented surface](../../../../../cohomology-ring-of-a-closed-oriented-surface.md):

$$
\alpha_i\smile\beta_j=\delta_{ij}\omega,
\qquad
\beta_j\smile\alpha_i=-\delta_{ij}\omega,
$$

and all $\alpha_i\smile\alpha_j$ and $\beta_i\smile\beta_j$ vanish.

For the space $X$, use the genus-two CW structure and attach an additional two-cell $e_v^2$ along $[b_1,b_2]$. Both two-cell attaching words have zero exponent sum in every one-cell, so the cellular boundary $C_2(X)\to C_1(X)$ is zero. Hence

$$
H^0(X;\mathbb Z)=\mathbb Z,qquad
H^1(X;\mathbb Z)=\mathbb Z^4,qquad
H^2(X;\mathbb Z)=\mathbb Z^2.
$$

Let $u,v$ be the degree-two classes dual respectively to the original surface cell and the new cell. The original relator $[a_1,b_1][a_2,b_2]$ and the new relator $[b_1,b_2]$ give

$$
\alpha_1\smile\beta_1=alpha_2\smile\beta_2=u,
\qquad
\beta_1\smile\beta_2=v,
$$

together with the products forced by graded commutativity. Every other product of degree-one basis classes is zero, and every product of total degree greater than two is zero. These relations completely determine the [cohomology ring](../../../../../cohomology-ring.md) of $X$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
