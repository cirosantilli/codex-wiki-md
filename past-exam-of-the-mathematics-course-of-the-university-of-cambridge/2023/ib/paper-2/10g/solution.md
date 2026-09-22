<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

A [sequence](../../../../../sequence.md) $f_n:S\to\mathbb R$ converges uniformly to $f$ if, for every $\varepsilon>0$, there is $N$ such that

$$
|f_n(x)-f(x)|<\varepsilon
$$

for every $x\in S$ and every $n\geq N$. A map $h:M\to N$ is uniformly continuous if, for every $\varepsilon>0$, there is $\delta>0$ such that

$$
d_M(x,y)<\delta\quad\Longrightarrow\quad d_N(h(x),h(y))<\varepsilon
$$

for all $x,y\in M$.

If $f\in C_0(\mathbb R^d)$, choose a ball outside which $|f|<1$. On the closed ball, continuity gives boundedness, so $f$ is bounded everywhere.

Now let $(f_n)$ be Cauchy in the uniform metric. For each $x$, $(f_n(x))$ is Cauchy in $\mathbb R$; let its [limit](../../../../../limit-of-a-function.md) be $f(x)$. Passing to the pointwise [limit](../../../../../limit-of-a-function.md) in the uniform Cauchy estimate shows that $f_n\to f$ uniformly. Hence $f$ is continuous. Given $\varepsilon>0$, choose $n$ with $\|f-f_n\|_\infty<\varepsilon/2$, and then choose $K$ so that $|f_n(x)|<\varepsilon/2$ for $\|x\|>K$. It follows that $f$ also vanishes at infinity. Thus $C_0(\mathbb R^d)$ is complete, as in [completeness of continuous functions vanishing at infinity](../../../../../completeness-of-continuous-functions-vanishing-at-infinity.md).

Every $f\in C_0(\mathbb R^d)$ is uniformly continuous. Given $\varepsilon>0$, choose $R$ so that $|f(x)|<\varepsilon/2$ outside the ball of radius $R$. On the compact ball of radius $R+1$, $f$ is uniformly continuous; choose the corresponding $\delta\leq1$. If two points at distance below $\delta$ are not both in that ball, then both lie outside the ball of radius $R$, and their [function](../../../../../function-split.md) values differ by less than $\varepsilon$.

For the final [sequence](../../../../../sequence.md), continuity of $\varepsilon$ at zero gives, for each fixed $x$,

$$
f_n(x)=\sqrt{x^2+\varepsilon(x/n)}\longrightarrow|x|.
$$

Thus [pointwise convergence](../../../../../pointwise-convergence.md) is compulsory. [Uniform convergence](../../../../../uniform-convergence.md) need not hold: with $\varepsilon(t)=t^2$,

$$
f_n(x)-|x|
=|x|\left(\sqrt{1+n^{-2}}-1\right),
$$

which is unbounded as a [function](../../../../../function-split.md) of $x$ for every fixed $n$.

Under the additional bound $\varepsilon(t)\leq M|t|$, however,

$$
0\leq f_n(x)-|x|
=\frac{\varepsilon(x/n)}{\sqrt{x^2+\varepsilon(x/n)}+|x|}
\leq\frac Mn
$$

for $x\ne0$, and the difference is zero at $x=0$. Hence convergence is uniform, by the [uniform square-root perturbation under linear growth](../../../../../uniform-square-root-perturbation-under-linear-growth.md) estimate. The pointwise answer remains yes.

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
