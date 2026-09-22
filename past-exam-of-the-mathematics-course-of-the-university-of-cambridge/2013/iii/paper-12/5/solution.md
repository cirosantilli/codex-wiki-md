<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Expose the independent coordinates one at a time and define the [Doob exposure martingale](../../../../../doob-exposure-martingale.md)

$$
M_i=\mathbb E[f\mid Z_1,\ldots,Z_i],\qquad M_0=\mathbb Ef,\qquad M_n=f.
$$

For a fixed exposed prefix, couple the future coordinates identically under two choices of $Z_i$. The coordinate-change hypothesis bounds the difference of the resulting conditional expectations by $c_i$. Thus the increment $D_i=M_i-M_{i-1}$ has conditional mean zero and lies in a conditional interval of length at most $c_i$. This range bound, rather than merely $|D_i|\le c_i$, gives the sharp constant in the [McDiarmid inequality](../../../../../mcdiarmid-s-inequality.md).

Here is a proof of the needed [Hoeffding lemma](../../../../../hoeffding-lemma.md). For a mean-zero random variable $X$ in an interval of length $c$, let $h(u)=\log\mathbb E e^{uX}$. Its second derivative is the variance under the exponentially tilted distribution. A random variable in $[a,b]$ has variance at most $(b-a)^2/4$: the inequality $\mathbb E[(X-a)(b-X)]\ge0$ gives $\operatorname{Var}X\le(\mathbb EX-a)(b-\mathbb EX)\le(b-a)^2/4$. Hence $h''(u)\le c^2/4$, and $h(0)=h'(0)=0$ imply $h(u)\le u^2c^2/8$, for either sign of $u$.

Apply this conditionally to each increment and iterate the [conditional expectation](../../../../../conditional-expectation.md):

$$
\mathbb E e^{u(f-\mathbb Ef)}\le\exp\left(\frac{u^2}{8}\sum_{i=1}^n c_i^2\right).
$$

For $u>0$, [Markov's inequality](../../../../../markov-inequality.md) bounds the upper tail by $\exp(-ut+u^2\sum c_i^2/8)$. Taking $u=4t/\sum c_i^2$ and then applying the same argument to $-f$ gives

$$
\boxed{\mathbb P(|f-\mathbb Ef|\ge t)\le2\exp\left(-\frac{2t^2}{\sum_i c_i^2}\right).}
$$

At $t=0$ the bound is immediate. If all $c_i$ vanish, $f$ is constant on the product support and the positive tails are zero, so that degenerate case is handled directly.

For a [binomial random graph](../../../../../binomial-random-graph.md), let coordinate $i$ be the entire vector of [edges](../../../../../edge-of-a-graph.md) from [vertex](../../../../../vertex-graph-theory.md) $i$ to [vertices](../../../../../vertex-graph-theory.md) of smaller label. The coordinates are independent finite probability spaces. Changing coordinate $i$ changes only [edges](../../../../../edge-of-a-graph.md) incident to that one [vertex](../../../../../vertex-graph-theory.md). Deleting the [vertex](../../../../../vertex-graph-theory.md) gives the same [graph](../../../../../graph-split.md) under both outcomes, and each outcome's [chromatic number](../../../../../chromatic-number.md) is either that [graph](../../../../../graph-split.md)'s chromatic number or one more. Thus the coordinate range is at most one. Taking all $c_i=1$ and $t=\lambda\sqrt n$ proves [vertex exposure for chromatic number](../../../../../vertex-exposure-for-chromatic-number.md):

$$
\boxed{\mathbb P\bigl(|\chi(G)-\mathbb E\chi(G)|\ge\lambda\sqrt n\bigr)\le2e^{-2\lambda^2}.}
$$

Using individual [edges](../../../../../edge-of-a-graph.md) as coordinates would give a weaker scale; grouping the incident [edges](../../../../../edge-of-a-graph.md) is what yields the required bound.

For the expectation asymptotic, take fixed $0<p<1$, put $b=1/(1-p)$, and write $L=\log_b n$. We outline both bounds and the step that turns probability estimates into an expectation estimate. For each fixed $\gamma>0$, the expected number of independent sets of size $k=\lceil(2+\gamma)L\rceil$ is

$$
\binom nk(1-p)^{\binom k2}.
$$

Its logarithm is $k\log n-\tfrac12k(k-1)\log b-O(k\log k)=-\Omega_\gamma((\log n)^2)$. Thus [Markov's inequality](../../../../../markov-inequality.md) gives $\alpha(G)\le(2+\gamma)L$ with probability tending to one, and $\chi(G)\ge n/\alpha(G)$ yields the corresponding lower bound on its expectation.

For the upper bound, set $m_0=\lceil n/(\log n)^2\rceil$ and $k=\lfloor(2-\gamma)L\rfloor$, with $0<\gamma<1$. The key uniform fact is that **every [vertex](../../../../../vertex-graph-theory.md) subset of size at least $m_0$ contains an independent $k$-set with probability tending to one**. For a fixed subset of size $m$, let $X$ count its independent $k$-sets and let $\mu=\binom mk b^{-\binom k2}$. The normalized dependency sum in [Janson inequality](../../../../../janson-inequality.md) is bounded by

$$
\frac{\Delta}{\mu^2}\le\sum_{j=2}^{k-1}\frac{\binom kj\binom{m-k}{k-j}}{\binom mk}\,b^{\binom j2}.
$$

The $j=2$ term is $O(k^4/m^2)$. The remaining overlap terms give the same order or less: use $\binom kj\binom{m-k}{k-j}/\binom mk\le(2k^2/m)^j$ for large $n$, and split the sum at $k/2$. For the lower half the terms beyond $j=2$ decrease at the initial endpoint and are exponentially small at the other endpoint; for the upper half, $k\le(2-\gamma/2)\log_b m$ makes every endpoint exponent negative of order $(\log n)^2$. Also $1/\mu$ is exponentially small on that scale. The exponential form of [Janson inequality](../../../../../janson-inequality.md) therefore gives, uniformly for $m\ge m_0$,

$$
\mathbb P(X=0)\le\exp(-c_\gamma m^2/k^4)
$$

for a positive constant depending only on $p,\gamma$. A union bound over at most $2^n$ subsets succeeds, because $m_0^2/k^4$ is of order $n^2/(\log n)^8\gg n$. This is [independent sets in every large subset of a dense random graph](../../../../../independent-sets-in-every-large-subset-of-a-dense-random-graph.md).

On that event, repeatedly remove an independent $k$-set and assign it one new colour until fewer than $m_0$ [vertices](../../../../../vertex-graph-theory.md) remain; colour the remainder individually. This gives $\chi(G)\le n/k+m_0$. The failure probability is exponentially small compared with $1/\log n$, and always $\chi(G)\le n$, so the failure event contributes negligibly to the expectation. Combining the upper and lower bounds and then letting $\gamma\downarrow0$ proves

$$
\boxed{\mathbb E\chi(G)=(1+o(1))\frac{n}{2\log_{1/(1-p)}n}.}
$$

This is the [chromatic number of a binomial random graph](../../../../../chromatic-number-of-a-binomial-random-graph.md) asymptotic. The slash in the printed expression must be read with $2\log_{1/(1-p)}n$ as the denominator; a multiplicative reading would eventually exceed $n$. At the endpoint probabilities $p=0$ and $p=1$, the chromatic numbers are respectively one and $n$ for $n\ge1$, so this logarithmic formula is intended for $0<p<1$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
