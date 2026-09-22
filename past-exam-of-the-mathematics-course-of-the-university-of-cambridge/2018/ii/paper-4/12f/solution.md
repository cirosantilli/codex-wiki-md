<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The set $K$ is [compact](../../../../../compact-space.md), and its complement is connected: two disjoint closed disks do not enclose any bounded complementary component. Since $f$ is [holomorphic](../../../../../holomorphic-function.md) on the open neighbourhood $\Omega$ of $K$, the [polynomial Runge theorem](../../../../../polynomial-runge-theorem.md) gives, for each $n$, a polynomial $p_n$ such that

$$
\sup_{z\in K}|p_n(z)-f(z)|<\frac1n.
$$

Hence

$$
\boxed{p_n\longrightarrow f\text{ uniformly on }K.}
$$

Define a function on the disconnected open set $\Omega$ by

$$
f(z)=
\begin{cases}
0,&|z-2|<3/2,\\
1,&|z+2|<3/2.
\end{cases}
$$

It is holomorphic on $\Omega$. Applying the first part produces polynomials $P_n$ with

$$
\boxed{P_n\to0\text{ uniformly on }|z-2|\leq1,\qquad
P_n\to1\text{ uniformly on }|z+2|\leq1.}
$$

For an obstruction, take

$$
K_1=\{z:|z|=1\},
\qquad
K_2=\{0\}.
$$

These are disjoint nonempty bounded closed sets. If polynomials $Q_n$ converged uniformly to zero on $K_1$, the [maximum modulus principle on a bounded domain](../../../../../maximum-modulus-principle-on-a-bounded-domain.md) would give

$$
|Q_n(0)|\leq\max_{|z|=1}|Q_n(z)|\longrightarrow0.
$$

They therefore cannot also satisfy $Q_n(0)\to1$. Thus **this pair $K_1,K_2$ has the requested non-approximation property**.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
