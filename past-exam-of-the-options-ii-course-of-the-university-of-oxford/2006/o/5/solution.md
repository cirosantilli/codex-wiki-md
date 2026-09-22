<h1 id="o/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A possibly [randomized statistical test](../../../../randomized-statistical-test.md) has rejection probability $\varphi(x)\in[0,1]$ after observing $x$. Its [statistical power](../../../../statistical-power.md) at parameter $\theta$ is $\mathbb E_\theta\varphi$, and its [test size](../../../../size-of-a-statistical-test.md) is the supremum of that [statistical power](../../../../statistical-power.md) over the null parameter set.

For simple hypotheses with densities $f_0,f_1$, the [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) states that a level-$\alpha$ test is most powerful if it rejects where $f_1>k f_0$, accepts where $f_1<k f_0$, and randomizes on equality to obtain null rejection probability $\alpha$. Here $k\geq0$ is chosen to reach that [test size](../../../../size-of-a-statistical-test.md). To prove optimality, let $\varphi_*$ be this test and $\varphi$ any test of level at most $\alpha$. Pointwise,

$$
(\varphi_*-\varphi)(f_1-kf_0)\geq0.
$$

Integrating and using $\int(\varphi_*-\varphi)f_0\geq0$ gives $\mathbb E_1\varphi_*-\mathbb E_1\varphi\geq0$. This proves maximal [statistical power](../../../../statistical-power.md). For $k>0$, equality also forces any equally powerful test to use all its allowed [test size](../../../../size-of-a-statistical-test.md) and agree with the indicated decisions away from the likelihood-ratio tie set, up to null sets.

For the Poisson sample, $S=\sum_iX_i\sim\operatorname{Poisson}(n\mu)$ and, for every fixed $\mu_1>\mu_0>0$, the [likelihood ratio](../../../../likelihood-ratio.md) is

$$
e^{-n(\mu_1-\mu_0)}(\mu_1/\mu_0)^S.
$$

It increases strictly with $S$. Choose an [integer](../../../../integer-split.md) $k$ so that $\mathbb P_{\mu_0}(S>k)\leq\alpha\leq\mathbb P_{\mu_0}(S\geq k)$, and reject for $S>k$, with boundary rejection probability

$$
\boxed{r=\frac{\alpha-\mathbb P_{\mu_0}(S>k)}
{\mathbb P_{\mu_0}(S=k)}\quad\text{when }S=k.}
$$

This has exact [test size](../../../../size-of-a-statistical-test.md) $\alpha$. Its rejection ordering and calibration do not depend on which $\mu_1>\mu_0$ is selected, so the lemma proves it **uniformly most powerful** for the whole one-sided alternative. Randomization is generally needed for an exact arbitrary [test size](../../../../size-of-a-statistical-test.md) in a discrete model.

For the approximate design, the [central limit theorem](../../../../central-limit-theorem.md) under $\mu_0=1$ gives critical sum $n+1.645\sqrt n$. Under $\mu_1$, the sum is approximately normal with mean $n\mu_1$ and [variance](../../../../variance-split.md) $n\mu_1$. Target [statistical power](../../../../statistical-power.md) $0.9$ therefore gives

$$
\frac{n+1.645\sqrt n-n\mu_1}{\sqrt{n\mu_1}}\approx-1.282,
$$

or $\sqrt n(\mu_1-1)\approx1.645+1.282\sqrt{\mu_1}$. Thus the requested design expression is

$$
\boxed{n\approx\left(\frac{1.645+1.282\sqrt{\mu_1}}{\mu_1-1}\right)^2.}
$$

Round upward to obtain an [integer](../../../../integer-split.md) design. This is a [normal approximation](../../../../normal-approximation.md) to the requested [statistical power](../../../../statistical-power.md), rather than an exact discrete sample-size guarantee; the exact Poisson test above provides its exact calibration.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [O](../../o.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
