<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A standard form of [Varadhan's integral theorem](../../../../../varadhan-s-lemma.md) is as follows. Let $\mu_L$ be [probability measures](../../../../../probability-measure.md) on a [Polish space](../../../../../polish-space.md) $E$ satisfying a [large deviation principle](../../../../../large-deviation-principle.md) with speed $L\to\infty$ and [good rate function](../../../../../good-rate-function.md) $I$. If $F:E\to\mathbb R$ is [continuous](../../../../../continuous-function.md) and bounded above, then

$$
\boxed{\lim_{L\to\infty}\frac1L\log\int_Ee^{LF(x)}\,\mu_L(dx)
=\sup_{x\in E}\{F(x)-I(x)\}.}
$$

The usual bounded-[continuous](../../../../../continuous-function.md) version follows immediately. If $F$ is unbounded above, the same conclusion holds under the additional exponential tail condition

$$
\lim_{M\to\infty}\limsup_{L\to\infty}
\frac1L\log\int_{\{F>M\}}e^{LF(x)}\,\mu_L(dx)=-\infty.
$$

This is the [exponential tail extension of Varadhan's lemma](../../../../../exponential-tail-extension-of-varadhan-s-lemma.md). A convenient sufficient hypothesis is

$$
\limsup_{L\to\infty}\frac1L\log\int_Ee^{\gamma LF(x)}\,\mu_L(dx)<\infty
\quad\text{for some }\gamma>1.
$$

An integrability hypothesis is essential for general unbounded functions; the ordinary [large deviation principle](../../../../../large-deviation-principle.md) alone does not control arbitrarily large exponential weights.

For example, let $X^L=L$ with probability $e^{-L^2}$ and $X^L=0$ otherwise. It satisfies the [large deviation principle](../../../../../large-deviation-principle.md) at speed $L$ with rate zero at zero and infinite elsewhere. But for $F(x)=x^2$, $\mathbb E e^{LF(X^L)}\geq e^{L^3-L^2}$, whose logarithmic rate diverges, while $\sup(F-I)=0$. This shows why the tail hypothesis cannot simply be omitted.

For the lower bound, fix $x$ with $I(x)<\infty$ and $\varepsilon>0$. By [continuity](../../../../../continuous-function.md) choose an [open set](../../../../../open-set.md) $G$ containing $x$ on which $F(y)\geq F(x)-\varepsilon$. Then

$$
\int e^{LF}\,d\mu_L\geq
e^{L(F(x)-\varepsilon)}\mu_L(G).
$$

Apply the open-set lower bound of the [large deviation principle](../../../../../large-deviation-principle.md):

$$
\liminf_{L\to\infty}\frac1L\log\int e^{LF}\,d\mu_L
\geq F(x)-\varepsilon-\inf_GI
\geq F(x)-\varepsilon-I(x).
$$

Let $\varepsilon\downarrow0$ and take the [supremum](../../../../../supremum.md) over $x$ to obtain the required lower bound. This argument also applies when $F$ is not bounded above.

For the upper bound, suppose $F\leq M$ and set $S=\sup_E(F-I)$, which is finite. Choose a large $K$ and partition $[-K,M]$ into finitely many closed intervals $[a_j,a_j+\varepsilon]$ of length at most $\varepsilon$. The preimages

$$
C_j=\{x:a_j\leq F(x)\leq a_j+\varepsilon\}
$$

are [closed sets](../../../../../closed-set.md). The overlapping endpoints do not matter for an upper estimate. Split off the lower tail and bound each remaining exponential weight:

$$
\int e^{LF}\,d\mu_L
\leq e^{-LK}+
\sum_j e^{L(a_j+\varepsilon)}\mu_L(C_j).
$$

For a finite sum of nonnegative terms the upper logarithmic rate is at most the largest of their upper logarithmic rates. Applying the closed-set upper bound gives

$$
\limsup_{L\to\infty}\frac1L\log\int e^{LF}\,d\mu_L
\leq
\max\left\{-K,\ \max_j\left(a_j+\varepsilon-\inf_{C_j}I\right)\right\}.
$$

For $x\in C_j$, $a_j+\varepsilon\leq F(x)+\varepsilon$, hence every inner term is at most $S+\varepsilon$. Empty preimages contribute no term. Let $K\to\infty$ and then $\varepsilon\downarrow0$ to get the upper bound $S$. Together with the lower bound this proves the bounded-above theorem.

For the unbounded extension, put $F_M=\min(F,M)$. This is [continuous](../../../../../continuous-function.md) and bounded above, so the proved result applies, with

$$
S_M=\sup_x\{F_M(x)-I(x)\}\uparrow
S=\sup_x\{F(x)-I(x)\}.
$$

The full integral is at most the integral with $F_M$ plus the integral on $\{F>M\}$. The upper logarithmic rate is therefore at most the larger of $S_M$ and the tail rate. The tail hypothesis and then $M\to\infty$ give the upper bound $S$; the earlier local argument gives the lower bound. If $S=+\infty$, that lower argument already yields the asserted infinite limit.

Finally, the sufficient exponential-moment condition really implies the required tail estimate: on $F>M$,

$$
e^{LF}\leq e^{-(\gamma-1)LM}e^{\gamma LF}.
$$

After integration the upper logarithmic rate is bounded by a finite constant minus $(\gamma-1)M$, which tends to $-\infty$. This completes the statement and proof of [Varadhan's lemma](../../../../../varadhan-s-lemma.md), including the hypotheses needed for the unbounded version.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
