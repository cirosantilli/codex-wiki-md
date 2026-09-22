<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

Runge's polynomial approximation theorem says that if $K\subset\mathbb C$ is compact, $\mathbb C\setminus K$ is connected, and $f$ is holomorphic on a neighborhood of $K$, then for every $\varepsilon>0$ there is a polynomial $p$ such that

$$
\sup_K|p-f|<\varepsilon.
$$

Let

$$
S=\{z:|z|=1,\ \operatorname{Re}z\leq0\}.
$$

This arc is compact, its complement is connected, and $1/z$ is holomorphic on a neighborhood of it. Applying Runge with error $1/n$ gives a polynomial $q_n$ satisfying

$$
\sup_{z\in S}|q_n(z)-z^{-1}|<\frac1n,
$$

which is the requested uniform approximation.

For the pointwise construction, for $n\geq2$ set

$$
\begin{aligned}
K_n^+&=\{z:|z|\leq1-1/n,\ \operatorname{Re}z\geq1/n\},\\
K_n^-&=\{z:|z|\leq1-1/n,\ \operatorname{Re}z\leq-1/n\},\\
K_n^0&=\{iy:|y|\leq1-1/n\},
\qquad K_n=K_n^+\cup K_n^-\cup K_n^0.
\end{aligned}
$$

The three pieces are disjoint compact sets and $\mathbb C\setminus K_n$ is connected. Define a function on a neighborhood of $K_n$ to equal $1$, $-1$, and $0$ on neighborhoods of $K_n^+$, $K_n^-$, and $K_n^0$, respectively. It is holomorphic because those neighborhoods may be chosen disjoint. Runge supplies a polynomial $P_n$ such that

$$
|P_n-1|<1/n\ \hbox{on }K_n^+,
\quad |P_n+1|<1/n\ \hbox{on }K_n^-,
\quad |P_n|<1/n\ \hbox{on }K_n^0.
$$

Every fixed point with $|z|<1$ eventually belongs to the appropriate one of these three sets, according to the sign of its real part. These inequalities therefore give precisely the asserted pointwise limits.

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
