<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p_0=\Pr(\theta\in\Theta_0)$ and $p_1=1-p_0$, assuming both are positive. The [prior odds](../../../../prior-odds.md) are $\alpha=p_0/p_1$. Given data $x$, the [posterior odds](../../../../posterior-odds.md) are

$$
O_{01}(x)=\frac{\Pr(H_0\mid x)}{\Pr(H_1\mid x)}.
$$

With conditional joint [likelihood](../../../../likelihood-function.md) $L(\theta;x)=\prod_i f(x_i\mid\theta)$, define the hypothesis-conditional marginal densities

$$
m_0(x)=\frac1{p_0}\int_{\Theta_0}L(\theta;x)\,\pi(d\theta),\qquad
m_1(x)=\frac1{p_1}\int_{\Theta\setminus\Theta_0}L(\theta;x)\,\pi(d\theta).
$$

The [Bayes factor](../../../../bayes-factor.md) for $H_0$ relative to $H_1$ is $B=m_0(x)/m_1(x)$. The normalizations $p_0,p_1$ matter: the [prior distribution](../../../../prior-probability.md) within each hypothesis must have total probability one. [Bayes' theorem](../../../../bayes-theorem.md) now gives

$$
O_{01}(x)=\frac{p_0m_0(x)}{p_1m_1(x)}=\alpha B.
$$

Converting [posterior odds](../../../../posterior-odds.md) to [posterior probability](../../../../posterior-probability.md) therefore gives

$$
\boxed{\Pr(H_0\mid x)=\frac{\alpha B}{1+\alpha B}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
