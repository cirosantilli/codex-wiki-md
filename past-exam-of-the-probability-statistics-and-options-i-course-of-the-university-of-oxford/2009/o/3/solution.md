<h1 id="o/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An independent sum of normal variables is normal, with the means and variances added. Therefore $\overline X\sim N(\mu,\sigma^2/n)$ and **$Z\sim N(0,1)$** exactly.

Under the null, $Z_0=\sqrt n(\overline X-\mu_0)/\sigma$ is standard normal. Reject for $Z_0>w$, where $w=\Phi^{-1}(1-\alpha)$, giving size $\alpha$. For $\alpha=0.05$, the supplied table gives **the critical region $\overline X>\mu_0+1.64\sigma/\sqrt n$**, using its rounded quantile.

The [power function](../../../../power-function-of-a-statistical-test.md) is the probability of rejection when the true parameter is $\mu$. Recenter by that true [mean](../../../../expected-value-split.md):

$$
Q(\mu)=\mathbb P_\mu\left(\frac{\sqrt n(\overline X-\mu)}\sigma>w-\frac{\sqrt n(\mu-\mu_0)}\sigma\right)
=1-\Phi\left(w-\frac{\sqrt n(\mu-\mu_0)}\sigma\right).
$$

For $n=100$, $\sigma=2$, power at least $0.70$ means $w-5(\mu-\mu_0)\leq-0.52$. Hence, with the supplied rounding,

$$
\boxed{\mu\geq\mu_0+0.432.}
$$

The exact unrounded threshold is $\mu_0+(\Phi^{-1}(0.95)-\Phi^{-1}(0.30))/5$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [O](../../o.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
