<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $p<p_c=\widetilde p_c$, choose a finite set $S\ni0$ with $\phi_p(S)=\rho<1$. Let $L$ exceed the $\ell^\infty$-distance from $0$ to every endpoint of an edge in $\partial S$, and put

$$
q_n=\mathbb P_p(0\leftrightarrow\partial B(n)).
$$

On the one-arm event to distance $n>L$, take the first oriented boundary edge $(x,y)\in\partial S$ used by an open self-avoiding path. The connection $0\xleftarrow{S}x$, the open edge $(x,y)$, and the remaining connection from $y$ to $\partial B(n)$ occur disjointly. The [Van den Berg-Kesten inequality](../../../../../../van-den-berg-kesten-inequality.md) and translation invariance therefore give

$$
\begin{aligned}
q_n
&\leq p\sum_{(x,y)\in\partial S}
\mathbb P_p(0\xleftarrow{S}x)
\mathbb P_p(y\leftrightarrow\partial B(n))\\
&\leq\phi_p(S)q_{n-L}=\rho q_{n-L}.
\end{aligned}
$$

Iteration yields $q_n\leq\rho^{\lfloor n/L\rfloor}$ up to an inessential finite-scale adjustment. Since $p<1$, each of the finitely many remaining $q_n$ is strictly below one, so reducing the exponent if necessary produces a constant $c>0$ valid for every $n\geq1$:

$$
\boxed{\mathbb P_p(0\leftrightarrow\partial B(n))\leq e^{-cn}.}
$$

This is the finite-size proof of [exponential decay of subcritical percolation](../../../../../../exponential-decay-of-subcritical-percolation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
