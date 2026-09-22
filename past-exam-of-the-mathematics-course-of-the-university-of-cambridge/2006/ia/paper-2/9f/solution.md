<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Condition on the current generation size. By [independence](../../../../../independent-random-variables.md) of offspring families, $\mathbb E[s^{Z_{n+1}}\mid Z_n=k]=G(s)^k$. Taking the [expected value](../../../../../expected-value.md) gives the [probability generating function](../../../../../probability-generating-function.md) recursion

$$
G_{n+1}(s)=G_n(G(s)),\qquad G_0(s)=s.
$$

Induction therefore proves the [branching-process generating-function iteration](../../../../../branching-process-generating-function-iteration.md)

$$
\boxed{G_n(s)=G^{\circ n}(s),}
$$

where the right side means $n$-fold composition, not an ordinary power.

Let $m=G'(1)$ and $\sigma^2=G''(1)+m-m^2$ be the offspring [mean](../../../../../expected-value.md) and [variance](../../../../../variance-split.md), assuming a finite second moment. Differentiating the generating-function recursion at one gives $\mathbb EZ_n=m^n$ and, with $a_n=G_n''(1)$,

$$
a_{n+1}=m^2a_n+G''(1)m^n.
$$

Since $\operatorname{Var}(Z_n)=a_n+m^n-m^{2n}$, this implies

$$
v_{n+1}=m^2v_n+\sigma^2m^n,\qquad v_0=0.
$$

Iteration and summation of the [geometric progression](../../../../../geometric-progression.md) give the [mean and variance of a Galton-Watson generation](../../../../../mean-and-variance-of-a-galton-watson-generation.md):

$$
\boxed{\operatorname{Var}(Z_n)=\begin{cases}
\displaystyle\sigma^2m^{n-1}\frac{m^n-1}{m-1},&m>0,\ m\ne1,\ n\ge1,\\
n\sigma^2,&m=1.
\end{cases}}
$$

For $m=0$ the offspring count is identically zero, so every later generation has zero [variance](../../../../../variance-split.md). The zeroth generation always has zero [variance](../../../../../variance-split.md). Finiteness of the needed moments is an assumption for this finite-valued [variance](../../../../../variance-split.md) formula, not a consequence of merely having a [probability generating function](../../../../../probability-generating-function.md). With finite positive [mean](../../../../../expected-value.md) but infinite offspring [variance](../../../../../variance-split.md), all positive-generation variances are infinite.

For the total count, make the generation convention explicit. If the first $n$ generations include the ancestor, put $T_n=Z_0+\cdots+Z_{n-1}$ and $H_n(s)=\mathbb E[s^{T_n}]$, with $T_0=0$. Given $k$ children of the ancestor, each starts an independent depth-$n$ descendant tree with generating function $H_n$. The ancestor contributes an additional factor $s$, so

$$
\boxed{H_{n+1}(s)=sG(H_n(s)),\qquad H_0(s)=1,\quad H_1(s)=s.}
$$

This is the [finite-horizon total progeny generating function](../../../../../finite-horizon-total-progeny-generating-function.md). If instead “first $n$ generations” means descendants $Z_1+\cdots+Z_n$, excluding $Z_0$, write $\widehat H_n$ for that convention. Conditioning on the children now gives $\widehat H_{n+1}(s)=G(s\widehat H_n(s))$, with $\widehat H_0=1$ and $\widehat H_1=G$. The two conventions encode the same tree but different counts.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
