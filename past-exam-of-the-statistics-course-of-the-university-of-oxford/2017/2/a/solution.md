<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) concerns a [simple hypothesis](../../../../simple-hypothesis.md) $H_0:\theta=\theta_0$ against another [simple hypothesis](../../../../simple-hypothesis.md) $H_1:\theta=\theta_1$. For a continuous [statistical sample](../../../../statistical-sample.md), put $f_j(x)=\prod_i f(x_i;\theta_j)$ for the joint [probability density functions](../../../../probability-density-function.md), $j=0,1$. A [randomized statistical test](../../../../randomized-statistical-test.md) is a measurable $\phi(x)\in[0,1]$, the conditional [probability](../../../../probability.md) of rejection after observing $x$. Its [test size](../../../../size-of-a-statistical-test.md) is $\mathbb E_0\phi$ and its [statistical power](../../../../statistical-power.md) is $\mathbb E_1\phi$.

Choose $k\geq0$ and boundary randomization so that

$$
\phi_*(x)=\begin{cases}
1,&f_1(x)>kf_0(x),\\
0,&f_1(x)<kf_0(x),\\
\gamma(x)\in[0,1],&f_1(x)=kf_0(x),
\end{cases}
\qquad\mathbb E_0\phi_* =\alpha.
$$

Then **$\phi_*$ is most powerful among all tests of size at most $\alpha$**. Thus one rejects for sufficiently large alternative-to-null [likelihood ratio](../../../../likelihood-ratio.md). If the equality set has zero [probability](../../../../probability.md) under $H_0$, the test needs no randomization. Continuous observations alone do not guarantee that their [likelihood ratio](../../../../likelihood-ratio.md) has a continuous [probability distribution](../../../../probability-distribution-split.md).

For the proof, let $\phi$ be any competing test with $\mathbb E_0\phi\leq\alpha$. At every $x$,

$$
(\phi_*(x)-\phi(x))(f_1(x)-kf_0(x))\geq0.
$$

Indeed, on $f_1>kf_0$ the first factor is $1-\phi\geq0$; on $f_1<kf_0$ it is $-\phi\leq0$; and on equality the product is zero. [Integration](../../../../integral-split.md) gives

$$
\mathbb E_1\phi_* -\mathbb E_1\phi
\geq k(\mathbb E_0\phi_* -\mathbb E_0\phi)\geq0,
$$

which proves the claimed optimality. Moreover, when $k>0$, equality of [statistical power](../../../../statistical-power.md) forces equality of [test size](../../../../size-of-a-statistical-test.md) and forces $\phi=\phi_*$ almost everywhere where $f_1\ne kf_0$: otherwise the nonnegative integrand would have positive [integral](../../../../integral-split.md). This proves the usual necessity assertion as well, up to equality sets and sets of zero [probability](../../../../probability.md) under both hypotheses.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
