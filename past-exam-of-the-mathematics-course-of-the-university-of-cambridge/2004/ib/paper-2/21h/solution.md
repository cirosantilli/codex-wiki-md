<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

A [simple hypothesis](../../../../../simple-hypothesis.md) specifies one probability distribution. Let the [null hypothesis](../../../../../null-hypothesis.md) and alternative have [probability density functions](../../../../../probability-density-function.md) $f_0,f_1$ with respect to a common measure. A possibly randomized [statistical test](../../../../../statistical-test.md) is a measurable function $\varphi(x)\in[0,1]$, its conditional probability of rejecting the [null hypothesis](../../../../../null-hypothesis.md). Its [size of a statistical test](../../../../../size-of-a-statistical-test.md) is $\mathbb E_0\varphi$, and its [statistical power](../../../../../statistical-power.md) at the alternative is $\mathbb E_1\varphi$. A [most powerful test](../../../../../most-powerful-test.md) at level $\alpha$ maximizes power among tests with size at most $\alpha$.

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) says to choose $k\geq0$ and a test $\varphi_*$ of size $\alpha$ with $\varphi_*=1$ where $f_1>kf_0$ and $\varphi_*=0$ where $f_1<kf_0$, choosing values on the equality set to reach the specified size. Equivalently, threshold the [likelihood ratio](../../../../../likelihood-ratio.md), treating positive alternative density with zero null density as an infinite ratio. Randomization on a threshold atom ensures exact size when needed. If $k=0$, all remaining null-only mass can be used to reach size without changing power.

For any test $\varphi$ of size at most $\alpha$, the signs of the two factors give

$$
(\varphi_*-\varphi)(f_1-kf_0)\geq0
$$

pointwise. Integrating proves

$$
\mathbb E_1\varphi_*-\mathbb E_1\varphi
\geq k(\mathbb E_0\varphi_*-\mathbb E_0\varphi)\geq0.
$$

This is the required optimality proof. If $k>0$ and another test is equally powerful, both inequalities must be equalities. It must have size $\alpha$ and agree with $\varphi_*$ wherever $f_1\ne kf_0$, apart from null sets for the relevant densities. Thus freedom is confined to the equality set and sets null under both hypotheses; at $k=0$, additional size need not improve power. This also explains the nonuniqueness below.

For the unit-scale [Laplace distribution](../../../../../laplace-distribution.md), put $\delta=\theta_1-\theta_0>0$. Its [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
L(x)=\frac{f(x\mid\theta_1)}{f(x\mid\theta_0)}=
\begin{cases}
e^{-\delta},&x\leq\theta_0,\\
e^{2x-\theta_0-\theta_1},&\theta_0<x<\theta_1,\\
e^\delta,&x\geq\theta_1.
\end{cases}
$$

It is nondecreasing, so an upper-tail [critical region](../../../../../rejection-region.md) has the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) form, even if the cutoff lies inside a constant-ratio tail. Solving $\mathbb P_{\theta_0}(X>c_\alpha)=\alpha$ gives the [most powerful test for a Laplace location shift](../../../../../most-powerful-test-for-a-laplace-location-shift.md),

$$
\boxed{\text{reject }H_0\text{ when }X>c_\alpha,\qquad
c_\alpha=\begin{cases}
\theta_0-\log(2\alpha),&0<\alpha\leq1/2,\\
\theta_0+\log(2(1-\alpha)),&1/2<\alpha<1.
\end{cases}}
$$

Continuity of the distribution makes this nonrandomized test exactly size $\alpha$. It need not be the unique [most powerful test](../../../../../most-powerful-test.md): within a flat extreme [likelihood ratio](../../../../../likelihood-ratio.md) region, other selections having the same null probability are equally good.

Its [statistical power](../../../../../statistical-power.md) is

$$
\beta(\theta_1)=\begin{cases}
\frac12e^{\theta_1-c_\alpha},&c_\alpha\geq\theta_1,\\
1-\frac12e^{c_\alpha-\theta_1},&c_\alpha<\theta_1.
\end{cases}
$$

Here $\beta$ denotes power, not the probability of a type-II error. For $\alpha=0.05$, $c_\alpha=\theta_0+\log10$. Thus the power is $0.05e^\delta$ for $\delta\leq\log10$, and $1-5e^{-\delta}$ otherwise. The first branch is at most $1/2$. On the second branch, power at least $0.95$ is equivalent to $5e^{-\delta}\leq0.05$. Therefore **the required pairs are exactly $\theta_1-\theta_0\geq\log100$**, with no restriction on the common location.

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
