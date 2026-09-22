<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

By [linearity of expectation](../../../../../../linearity-of-expectation.md) and [independence](../../../../../../independent-random-variables.md),

$$
\mathbb E W=\mu,\qquad\operatorname{Var}(W)=
\frac1{n^2}\sum_{i=1}^n\operatorname{Var}(X_i)=\frac{\sigma^2}{n}.
$$

For $\sigma>0$, apply [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) at threshold $h\sigma$ and take the complementary event:

$$
\boxed{\mathbb P(|W-\mu|\leq h\sigma)
=1-\mathbb P(|W-\mu|>h\sigma)
\geq1-\frac{1}{nh^2}.}
$$

If $\sigma=0$, every $X_i=\mu$ almost surely, so $W=\mu$ almost surely and the bound holds directly. This handles the zero-threshold case without applying [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) at an inadmissible threshold.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
