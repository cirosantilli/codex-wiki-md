<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a nondegenerate [distribution function](../../../../../cumulative-distribution-function.md) $G$, membership $F\in D(G)$ in its [maximum domain of attraction](../../../../../maximum-domain-of-attraction.md) means that there exist $a_n>0,b_n\in\mathbb R$ such that

$$
F(a_nx+b_n)^n=\mathbb P\!\left(\frac{X^{(n)}-b_n}{a_n}\leq x\right)\longrightarrow G(x)
$$

at every [continuity](../../../../../continuous-function.md) point of $G$. A [max-stable distribution](../../../../../max-stable-distribution.md) satisfies: for each [positive integer](../../../../../positive-integer.md) $k$, there exist $c_k>0,d_k\in\mathbb R$ such that $G(c_kx+d_k)^k=G(x)$. Thus a maximum of $k$ independent copies has the same [probability distribution](../../../../../probability-distribution.md) after a change of location and scale.

Suppose first that $F\in D(G)$. For fixed $k$, the [distribution functions](../../../../../cumulative-distribution-function.md) $H_n=F^{kn}$ have the two nondegenerate limits

$$
H_n(a_nx+b_n)\longrightarrow G(x)^k,\qquad H_n(a_{kn}x+b_{kn})\longrightarrow G(x).
$$

The given convergence-of-types result supplies constants $a>0,b$ such that $G(x)^k=G(ax+b)$. Equality extends from [continuity](../../../../../continuous-function.md) points to all points by [right continuity](../../../../../right-continuous-function.md). Substitute $x=(z-b)/a$ to obtain $G((z-b)/a)^k=G(z)$, which proves max-stability with $c_k=1/a,d_k=-b/a$. Conversely, if $G$ is max-stable, take $F=G$ and its max-stability constants for $k=n$. Then $F(c_nx+d_n)^n=G(x)$ exactly for every $n$, proving $G\in D(G)$. Therefore **the [maximum domain of attraction](../../../../../maximum-domain-of-attraction.md) is nonempty exactly when $G$ is max-stable**.

For the particular logarithmic tail, complete the [distribution function](../../../../../cumulative-distribution-function.md) by taking $F(x)=0$ for $x\leq x_0$. Let $a_n>1$ be the unique solution of $a_n\log a_n=n$, and take $b_n=0$. Equivalently $F(a_n)=1-1/n$, including $n=1$ with $a_1=x_0$. For each fixed $x>0$, eventually $a_nx>x_0$, and

$$
n\{1-F(a_nx)\}=\frac{n}{a_nx\log(a_nx)}=\frac1x\frac{\log a_n}{\log a_n+\log x}\longrightarrow\frac1x.
$$

Here $a_n\to\infty$ follows directly from its defining equation. Since $\log(1-z)=-z+O(z^2)$ as $z\to0$, it follows that $n\log F(a_nx)\to-1/x$. For $x\leq0$, the probability is zero. Consequently

$$
\boxed{F\in D(G),\qquad G(x)=\begin{cases}e^{-1/x},&x>0,\\0,&x\leq0,\end{cases}\quad a_n\log a_n=n,\quad b_n=0.}
$$

This is the shape-one [Fréchet distribution](../../../../../frechet-distribution.md), and the calculation proves the limit at every real $x$ without needing a [regular variation](../../../../../regular-variation.md) theorem.

The function $t\log t$ is strictly increasing on $t>1$. For every integer $n\geq3$, $n\log n>n=a_n\log a_n$, so $a_n<n$. The defining equation now gives $a_n=n/\log a_n>n/\log n$. Taking logarithms yields $\log a_n>\log n-\log\log n$, whose right side is positive, so

$$
\frac n{\log n}<a_n<\frac n{\log n-\log\log n}\qquad(n\geq3).
$$

Multiplying by $\log n/n$ and squeezing gives $a_n\log n/n\to1$. [Slutsky theorem](../../../../../slutsky-theorem.md) applied to the normalized [sample maximum](../../../../../sample-maximum.md) therefore gives the simpler [logarithmic-tail Fréchet normalization](../../../../../logarithmic-tail-frechet-normalization.md)

$$
\boxed{\mathbb P\!\left(\frac{X^{(n)}\log n}{n}\leq x\right)\longrightarrow G(x)\quad\text{for every }x\in\mathbb R.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
