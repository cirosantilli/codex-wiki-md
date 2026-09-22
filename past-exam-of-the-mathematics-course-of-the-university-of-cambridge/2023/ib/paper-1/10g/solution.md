<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

A [Cauchy sequence](../../../../../cauchy-sequence.md) $(x_n)$ in a metric space $(M,d)$ satisfies: for every $\varepsilon>0$ there is $N$ such that $d(x_m,x_n)<\varepsilon$ whenever $m,n\geq N$. A [complete metric space](../../../../../complete-metric-space.md) is one in which every Cauchy [sequence](../../../../../sequence.md) converges to a point of the space.

Every Cauchy [sequence](../../../../../sequence.md) is bounded. Choose $N$ such that $d(x_n,x_N)<1$ for $n\geq N$, and put

$$
R=1+\max_{1\leq j<N}d(x_j,x_N).
$$

Then every term lies in the ball $B(x_N,R)$.

Now suppose $M$ is complete and $(F_n)$ is a decreasing [sequence](../../../../../sequence.md) of nonempty closed sets with $\operatorname{diam}F_n\to0$. Choose $x_n\in F_n$. Given $\varepsilon>0$, choose $N$ with $\operatorname{diam}F_N<\varepsilon$. For $m,n\geq N$, both points lie in $F_N$, so $d(x_m,x_n)<\varepsilon$. Completeness gives $x_n\to x\in M$. For each fixed $N$, the tail lies in the closed set $F_N$, hence $x\in F_N$. Therefore

$$
x\in\bigcap_{n=1}^{\infty}F_n.
$$

Conversely, assume the nested-set property and let $(x_n)$ be Cauchy. Define

$$
F_n=\overline{\{x_m:m\geq n\}}.
$$

These sets are nonempty, closed, and decreasing. The Cauchy property implies $\operatorname{diam}F_n\to0$; taking a closure does not change the diameter. Choose $x\in\bigcap_nF_n$. Since $x_n,x\in F_n$,

$$
d(x_n,x)\leq\operatorname{diam}F_n\longrightarrow0.
$$

Thus every Cauchy [sequence](../../../../../sequence.md) converges and $M$ is complete. This proves the [Cantor intersection theorem](../../../../../cantor-s-intersection-theorem.md) characterization.

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a contraction of a nonempty complete metric space has a unique fixed point.

For each $\lambda\in\Lambda$, the map $T_\lambda(x)=T(\lambda,x)$ is a contraction with the common constant $k$, so it has a unique fixed point $x^*(\lambda)$. This defines the required unique [function](../../../../../function-split.md). Fix $\lambda_0$. The fixed-point identities and the triangle inequality give

$$
\begin{aligned}
d(x^*(\lambda),x^*(\lambda_0))
&\leq d(T(\lambda,x^*(\lambda)),T(\lambda,x^*(\lambda_0)))\\
&\quad+d(T(\lambda,x^*(\lambda_0)),T(\lambda_0,x^*(\lambda_0)))\\
&\leq k\,d(x^*(\lambda),x^*(\lambda_0))
+d(T(\lambda,x^*(\lambda_0)),T(\lambda_0,x^*(\lambda_0))).
\end{aligned}
$$

Consequently

$$
d(x^*(\lambda),x^*(\lambda_0))
\leq\frac{d(T(\lambda,x^*(\lambda_0)),T(\lambda_0,x^*(\lambda_0)))}{1-k}.
$$

The numerator tends to zero as $\lambda\to\lambda_0$ by the assumed continuity for the fixed point $x^*(\lambda_0)$. Hence $x^*$ is continuous, an instance of [continuous dependence of the fixed point of a uniform contraction](../../../../../continuous-dependence-of-the-fixed-point-of-a-uniform-contraction.md).

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
