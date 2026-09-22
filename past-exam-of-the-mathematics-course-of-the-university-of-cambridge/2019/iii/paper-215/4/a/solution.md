<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P$ be a finite reversible Markov chain with stationary distribution $\pi$, and write $Q(e)=\pi(u)P(u,v)$ for an oriented transition edge $e=(u,v)$. For every ordered pair $(x,y)$ choose a directed path $\gamma_{xy}$ from $x$ to $y$ using positive-capacity edges, and define the congestion

$$
\rho=\max_e\frac1{Q(e)}
\sum_{x,y:e\in\gamma_{xy}}
\pi(x)\pi(y)|\gamma_{xy}|.
$$

Then the [Canonical paths comparison theorem](../../../../../../canonical-paths-comparison-theorem.md) gives the [Poincaré inequality](../../../../../../poincare-inequality.md)

$$
\boxed{\operatorname{Var}_\pi(f)\leq\rho\,\mathcal E(f,f)}
$$

for every real function $f$, and hence the spectral gap is at least $1/\rho$.

Indeed,

$$
\operatorname{Var}_\pi(f)
=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2.
$$

Write each difference as the sum of edge differences along $\gamma_{xy}$ and apply [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md):

$$
(f(x)-f(y))^2
\leq|\gamma_{xy}|\sum_{e\in\gamma_{xy}}(\nabla_ef)^2.
$$

Interchanging the pair and edge sums, then applying the definition of $\rho$, bounds the result by

$$
\frac\rho2\sum_eQ(e)(\nabla_ef)^2
=\rho\mathcal E(f,f).
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
