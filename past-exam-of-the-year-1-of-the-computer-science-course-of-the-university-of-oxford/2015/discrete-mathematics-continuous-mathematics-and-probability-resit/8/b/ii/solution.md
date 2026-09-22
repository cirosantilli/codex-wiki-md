<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $I_i$ indicate that student $i$ stays awake. These indicators have independent [Bernoulli distributions](../../../../../../bernoulli-distribution.md) with parameter $p$, and $W=\sum_{i=1}^M I_i$. The [Poisson distribution](../../../../../../poisson-distribution.md) has [probability generating function](../../../../../../probability-generating-function.md)

$$
G_M(u)=\sum_{m=0}^{\infty}e^{-\lambda}\frac{\lambda^m}{m!}u^m
=e^{\lambda(u-1)}.
$$

The [probability generating function of an independent random sum](../../../../../../probability-generating-function-of-an-independent-random-sum.md) now gives

$$
G_W(s)=G_M(1-p+ps)=e^{\lambda p(s-1)}.
$$

Recognizing the [Poisson distribution](../../../../../../poisson-distribution.md),

$$
\boxed{W\sim\operatorname{Poisson}(\lambda p),\qquad
\mathbb P(W=w)=e^{-\lambda p}\frac{(\lambda p)^w}{w!},\quad w\geq0.}
$$

This is [Poisson thinning](../../../../../../poisson-thinning.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
