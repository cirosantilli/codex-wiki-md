<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an increasing sequence $(n_k)$ of nonnegative integers, [full-density sequence](../../../../../full-density-sequence.md) means that its range $S$ has [natural density](../../../../../natural-density.md) one:

$$
\frac{|S\cap\{0,\ldots,N-1\}|}{N}\longrightarrow1.
$$

For a sequence $(z_n)$ in a metric space, [convergence in density of a sequence](../../../../../convergence-in-density-of-a-sequence.md) to $z$ means that, for every $\varepsilon>0$,

$$
\frac1N\bigl|\{0\leq n<N:d(z_n,z)\geq\varepsilon\}\bigr|\longrightarrow0.
$$

In particular, a bounded nonnegative scalar sequence converging to zero in density has averages tending to zero: the average is at most $\varepsilon$ plus its bound times the proportion of indices above $\varepsilon$.

Here is a [Hilbert space](../../../../../hilbert-space-split.md) form of the [Van der Corput lemma](../../../../../van-der-corput-lemma-hilbert-space-sequences.md), including the density version. Suppose $\|u_n\|\leq M$, and put

$$
c_h=\limsup_{N\to\infty}\left|\frac1N\sum_{n=0}^{N-h-1}\langle u_{n+h},u_n\rangle\right|\qquad(h\geq1).
$$

Then

$$
\boxed{\frac1H\sum_{h=1}^Hc_h\longrightarrow0
\quad\Longrightarrow\quad
\left\|\frac1N\sum_{n=0}^{N-1}u_n\right\|\longrightarrow0.}
$$

Since $0\leq c_h\leq M^2$, it suffices for $(c_h)$ to converge to zero in density. A frequently used special case is that the correlation average tends to zero for every fixed $h\geq1$.

To prove the lemma, extend the finite list $u_0,\ldots,u_{N-1}$ by zero outside this range, and write $S_N=\sum_{n=0}^{N-1}u_n$. For $1\leq H\leq N$,

$$
HS_N=\sum_{n=-H+1}^{N-1}\sum_{r=0}^{H-1}u_{n+r}.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) for this sum, followed by expansion of the squared [Hilbert space](../../../../../hilbert-space-split.md) norm, gives

$$
H^2\|S_N\|^2
\leq(N+H-1)\left[
H\sum_{n=0}^{N-1}\|u_n\|^2
+2\sum_{h=1}^{H-1}(H-h)\operatorname{Re}\sum_{n=0}^{N-h-1}\langle u_{n+h},u_n\rangle
\right].
$$

The coefficient $H-h$ counts the pairs of shifts separated by $h$. Dividing by $H^2N^2$, bounding real parts by absolute values, and first taking the limit superior in $N$ for fixed $H$ yields

$$
\limsup_{N\to\infty}\left\|\frac{S_N}{N}\right\|^2
\leq\frac{M^2}{H}
+\frac2H\sum_{h=1}^{H-1}\left(1-\frac hH\right)c_h.
$$

The right side tends to zero as $H\to\infty$ under the stated hypothesis. This proves both the lemma and its density consequence.

For the polynomial application, fix a nonzero integer $m$ and let $u_n=e^{2\pi imP(n)}\in\mathbb C$. For each fixed $h\geq1$, the correlation phase is linear:

$$
P(n+h)-P(n)=2ahn+ah^2+bh.
$$

Thus, with $q_h=e^{2\pi i(2mah)}$,

$$
\frac1N\sum_{n=0}^{N-h-1}u_{n+h}\overline{u_n}
=e^{2\pi im(ah^2+bh)}\frac{1-q_h^{N-h}}{N(1-q_h)}.
$$

The coefficient $2mah$ is irrational, so $q_h\ne1$. This [geometric series](../../../../../geometric-series.md) is bounded in modulus by $2/(N|1-q_h|)$ and tends to zero. All $c_h$ vanish, so the [Van der Corput lemma](../../../../../van-der-corput-lemma-hilbert-space-sequences.md) gives

$$
\boxed{\frac1N\sum_{n=0}^{N-1}e^{2\pi im(an^2+bn+c)}\longrightarrow0\qquad(m\in\mathbb Z\setminus\{0\}).}
$$

The [Weyl criterion](../../../../../weyl-criterion.md) now shows that the fractional parts form an [equidistributed sequence](../../../../../equidistributed-sequence.md). For completeness, its sufficiency here follows directly: the displayed limits give the correct average for every [trigonometric polynomial](../../../../../trigonometric-polynomial.md), including the constant term. The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) extends this to every continuous function by uniform approximation. Approximating an interval's [indicator function](../../../../../indicator-function.md) above and below by continuous functions gives its length as the limiting frequency. Hence

$$
\boxed{(an^2+bn+c)\bmod1\text{ is equidistributed in }\mathbb R/\mathbb Z.}
$$

This proves the [equidistribution of a quadratic polynomial with irrational leading coefficient](../../../../../equidistribution-of-a-quadratic-polynomial-with-irrational-leading-coefficient.md) using the required correlation argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
