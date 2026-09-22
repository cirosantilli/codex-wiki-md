<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

In the [Erdős-Rényi model](../../../../../erdos-renyi-model.md) $G(n,p)$, the vertex set is $[n]$ and every one of the $\binom n2$ possible edges is present independently with probability $p$.

Let $X$ count [isolated vertices](../../../../../isolated-vertex.md). If $p\geq(1+\varepsilon)\log n/n$, the [union bound](../../../../../boole-s-inequality.md) gives

$$
\mathbb P(\delta(G_n)=0)
\leq n(1-p)^{n-1}
\leq n e^{-p(n-1)}
\longrightarrow0.
$$

Thus $\mathbb P(E_n)\to1$.

[Chebyshev inequality](../../../../../chebyshev-inequality.md) states that

$$
\mathbb P(|X-\mathbb EX|\geq t)
\leq\frac{\operatorname{Var}X}{t^2}.
$$

Now suppose $p\leq(1-\varepsilon)\log n/n$. Monotonicity lets us use the largest allowed $p$. With

$$
a=(1-p)^{n-1},
$$

the supplied lower exponential estimate shows

$$
\mathbb EX=na\longrightarrow\infty.
$$

For distinct vertices $i,j$,

$$
\mathbb P(i,j\text{ both isolated})
=(1-p)^{2n-3}
=\frac{a^2}{1-p}.
$$

Hence

$$
\operatorname{Var}X
=na(1-a)+n(n-1)a^2\frac p{1-p},
$$

and

$$
\frac{\operatorname{Var}X}{(\mathbb EX)^2}
\leq\frac1{na}+\frac p{1-p}
\longrightarrow0.
$$

Chebyshev with $t=\mathbb EX$ gives $\mathbb P(X=0)\to0$, so $\mathbb P(E_n)\to0$.

For connectivity, the lower-threshold result is immediate because a connected graph has no isolated vertex:

$$
F_n\subseteq E_n.
$$

For the upper threshold, if a graph is disconnected it has a component with vertex set $S$ of some size $1\leq k\leq n/2$. In particular, every one of the $k(n-k)$ edges from $S$ to its complement is absent. Therefore

$$
\mathbb P(F_n^c)
\leq
\sum_{k=1}^{\lfloor n/2\rfloor}
\binom nk(1-p)^{k(n-k)}.
$$

Choose

$$
\eta=\frac{\varepsilon}{2(1+\varepsilon)}.
$$

For $1\leq k\leq\eta n$, the standard bound $\binom nk\leq(en/k)^k$ gives

$$
\binom nk(1-p)^{k(n-k)}
\leq
\left[
\frac ek\,
n^{1-(1+\varepsilon)(1-\eta)}
\right]^k
=
\left(\frac ek n^{-\varepsilon/2}\right)^k.
$$

The sum of these terms tends to zero. For $\eta n\leq k\leq n/2$, use $\binom nk\leq2^n$ and $k(n-k)\geq\eta n^2/2$:

$$
\sum_{\eta n\leq k\leq n/2}
\binom nk(1-p)^{k(n-k)}
\leq
n\,2^n
\exp\left(-\frac{\eta}{2}pn^2\right)
\longrightarrow0.
$$

Thus $\mathbb P(F_n)\to1$ above the threshold. Together,

$$
\boxed{
p\geq(1+\varepsilon)\frac{\log n}{n}
\Longrightarrow\mathbb P(F_n)\to1,
\qquad
p\leq(1-\varepsilon)\frac{\log n}{n}
\Longrightarrow\mathbb P(F_n)\to0
}.
$$

This is the [connectivity threshold in the Erdős-Rényi model](../../../../../connectivity-threshold-in-the-erdos-renyi-model.md).

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
