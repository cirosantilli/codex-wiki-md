<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The stated bound is [Lipschitz continuity](../../../../../lipschitz-continuity.md) with constant $1$. For every $x$ and every $\varepsilon>0$, taking $\delta=\varepsilon$ ensures $|f(x)-f(y)|<\varepsilon$ whenever $|x-y|<\delta$. The same $\delta$ works at every point, so $f$ is both continuous and [uniformly continuous](../../../../../uniform-continuity.md).

For an integer $N\ge1$, partition $[0,1]$ into $N$ equal intervals and define a [step function](../../../../../step-function.md)

$$
g_N(x)=f(j/N)\quad\text{for }\frac jN\le x<\frac{j+1}{N},
\qquad j=0,\ldots,N-1.
$$

At the remaining endpoint set $g_N(1)=f((N-1)/N)$, so the final interval may be taken closed on the right. The [Lipschitz bound](../../../../../lipschitz-bound.md) gives

$$
|f(x)-g_N(x)|\le\frac1N
\quad\text{for all }x\in[0,1].
$$

Choosing $N\ge1/\varepsilon$ proves the requested [uniform step approximation on a compact interval](../../../../../uniform-step-approximation-on-a-compact-interval.md):

$$
\boxed{\sup_{x\in[0,1]}|f(x)-g_N(x)|\le\frac1N\le\varepsilon.}
$$

**A sufficiently fine partition gives a piecewise constant approximation uniformly over the whole interval.**

The [continuous function](../../../../../continuous-function.md) $f$ and every finite [step function](../../../../../step-function.md) $g_N$ are [Riemann integrable](../../../../../riemann-integrable-function.md). Put $c_j=f(j/N)$. Integrating each constant piece explicitly gives

$$
\int_0^1g_N(t)\cos(nt)\,dt
=\frac1n\sum_{j=0}^{N-1}c_j
\left[\sin\left(\frac{n(j+1)}N\right)
-\sin\left(\frac{nj}N\right)\right].
$$

Since the sine differences have absolute value at most $2$, the [triangle inequality](../../../../../triangle-inequality.md) and uniform approximation give

$$
\begin{aligned}
|u_n|
&\le\left|\int_0^1(f-g_N)(t)\cos(nt)\,dt\right|
+\left|\int_0^1g_N(t)\cos(nt)\,dt\right|\\
&\le\frac1N+\frac2n\sum_{j=0}^{N-1}|c_j|.
\end{aligned}
$$

To prove convergence, fix $\varepsilon>0$ and first choose $N$ with $1/N<\varepsilon/2$. With this $N$ held fixed, the finite number $\sum_j|c_j|$ is independent of $n$, so the second term is also less than $\varepsilon/2$ for sufficiently large $n$. Therefore

$$
\boxed{u_n\longrightarrow0.}
$$

**First make the approximation error small, then let the oscillation frequency grow.** This is the [step-function proof of the Riemann-Lebesgue lemma](../../../../../step-function-proof-of-the-riemann-lebesgue-lemma.md); it does not require assuming that a Lipschitz function has an everywhere-defined derivative.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
