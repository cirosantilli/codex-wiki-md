<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A standard [Brownian motion](../../../../../brownian-motion-split.md) is a real [stochastic process](../../../../../stochastic-process-split.md) $(B_t)_{t\geq0}$ with $B_0=0$ [almost surely](../../../../../almost-sure-convergence.md), continuous [sample paths](../../../../../sample-path.md) [almost surely](../../../../../almost-sure-convergence.md), and independent increments such that $B_t-B_s$ has [normal distribution](../../../../../normal-distribution.md) $N(0,t-s)$ whenever $0\leq s<t$. With its completed, right-continuous [natural filtration](../../../../../natural-filtration.md) $(\mathcal F_t)$, its [Strong Markov property](../../../../../strong-markov-property.md) is the following: for every almost-surely finite [stopping time](../../../../../stopping-time.md) $T$, the process

$$
W_s=B_{T+s}-B_T,\qquad s\geq0,
$$

is a standard [Brownian motion](../../../../../brownian-motion-split.md) independent of $\mathcal F_T$. Here the [stopping-time sigma-algebra](../../../../../stopping-time-sigma-algebra.md) is

$$
\mathcal F_T=\{A\in\mathcal F:A\cap\{T\leq t\}\in\mathcal F_t\text{ for all }t\geq0\}.
$$

In particular, for every bounded $\mathcal F_T$-measurable [random variable](../../../../../random-variable-split.md) $H$ and bounded Borel functional $G$ on the continuous path space,

$$
\mathbb E\bigl[H\,G((B_{T+s}-B_T)_{s\geq0})\bigr]
=\mathbb E[H]\,\mathbb E\bigl[G((B_s)_{s\geq0})\bigr].
$$

Thus the independence is from the entire stopped past, not only from $B_T$, and is a statement about the whole future path, not just a single increment.

To prove the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) without assuming that a level is hit in finite time, fix $t>0$, $m>0$, and set $T_m=\inf\{s\geq0:B_s\geq m\}$ and $R=T_m\wedge t$. Continuity of the [sample paths](../../../../../sample-path.md) makes $T_m$ a [stopping time](../../../../../stopping-time.md) and gives $B_{T_m}=m$ whenever $T_m<\infty$. The [stopping time](../../../../../stopping-time.md) $R$ is bounded. Reflect the path after $R$:

$$
\widehat B_s=
\begin{cases}
B_s,&s\leq R,\\
2B_R-B_s,&s>R.
\end{cases}
$$

By the [Strong Markov property](../../../../../strong-markov-property.md), the future increments after $R$ are an independent [Brownian motion](../../../../../brownian-motion-split.md). Negating them preserves their [probability distribution](../../../../../probability-distribution.md), by symmetry of their joint [normal distributions](../../../../../normal-distribution.md). Hence the reflected process $\widehat B$ has the same path law as $B$.

If $T_m>t$, reflection changes nothing on $[0,t]$ and $\widehat B_t=B_t<m$. If $T_m\leq t$, both paths first hit $m$ at the same time and $\widehat B_t=2m-B_t$. Therefore, for $x\leq m$, the following [events](../../../../../event.md) agree path by path:

$$
\{M_t\geq m,\ B_t\leq x\}
=\{\widehat B_t\geq2m-x\}.
$$

Indeed, the right-hand endpoint is at least $m$, so the reflected path must have hit $m$ before or at $t$; this also forces the original path to have done so. The reflection relation then makes the endpoint inequality equivalent to $B_t\leq x$. Equality cases at $T_m=t$ satisfy the same relation. Since $\widehat B_t$ and $B_t$ have the same [probability distribution](../../../../../probability-distribution.md),

$$
\boxed{\mathbb P(M_t\geq m,\ B_t\leq x)
=\mathbb P(B_t\geq2m-x)\qquad(m>0,\ x\leq m).}
$$

For $t=0$, both sides are zero, because $B_0=M_0=0$ and $2m-x\geq m>0$.

For $t>0$, set $x=m$ in this identity. Continuity implies $\{B_t>m\}\subseteq\{M_t\geq m\}$, and the [normal distribution](../../../../../normal-distribution.md) of $B_t$ has no atom at $m$. Splitting according to whether $B_t\leq m$ gives

$$
\mathbb P(M_t\geq m)=\mathbb P(B_t\geq m)+\mathbb P(B_t>m)
=2\mathbb P(B_t\geq m)=\mathbb P(|B_t|\geq m).
$$

Both [random variables](../../../../../random-variable-split.md) are nonnegative. Their tails agree for all $m>0$, which determines their [probability distributions](../../../../../probability-distribution.md), including the mass at zero. Thus the [Brownian running maximum](../../../../../brownian-running-maximum.md) satisfies

$$
\boxed{M_t\overset d=|B_t|\quad(t\geq0).}
$$

For $x>0$ and $t>0$, continuity again gives $\{T_x\leq t\}=\{M_t\geq x\}$. Since $B_t/\sqrt t$ is a [standard normal random variable](../../../../../standard-normal-random-variable.md), the [distribution function](../../../../../cumulative-distribution-function.md) of the [Brownian first-passage time](../../../../../brownian-first-passage-time.md) is

$$
F_{T_x}(t)=2\left[1-\Phi\!\left(\frac{x}{\sqrt t}\right)\right].
$$

It tends to one as $t\to\infty$ and to zero as $t\downarrow0$, proving almost-sure finiteness and absence of an atom at zero. For the [standard normal random variable](../../../../../standard-normal-random-variable.md) $B_1$,

$$
\mathbb P\!\left(\left(\frac{x}{B_1}\right)^2\leq t\right)
=\mathbb P\!\left(|B_1|\geq\frac{x}{\sqrt t}\right)
=2\left[1-\Phi\!\left(\frac{x}{\sqrt t}\right)\right].
$$

The value of this ratio on the zero-probability [event](../../../../../event.md) $\{B_1=0\}$ may be defined arbitrarily. Matching the [distribution functions](../../../../../cumulative-distribution-function.md) proves

$$
\boxed{T_x\overset d=\left(\frac{x}{B_1}\right)^2.}
$$

Finally, differentiate the [distribution function](../../../../../cumulative-distribution-function.md) on $t>0$, using $\Phi'=\phi$ and $\frac{d}{dt}(x/\sqrt t)=-x/(2t^{3/2})$. The [first-passage-time density](../../../../../first-passage-time-density.md) is

$$
\boxed{f_{T_x}(t)=\frac{x}{\sqrt{2\pi}\,t^{3/2}}\exp\!\left(-\frac{x^2}{2t}\right)\quad(t>0),}
$$

and is zero for $t\leq0$. Its integral is one by the endpoint limits of $F_{T_x}$, so no missing mass at an infinite [hitting time](../../../../../first-passage-time.md) is present.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
