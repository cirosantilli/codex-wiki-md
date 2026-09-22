<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N=|\mathcal X|\geq2$ and let $E=\mathbf1_{\{X\ne Y\}}$ be the error [indicator random variable](../../../../indicator-random-variable.md). Because $E$ is determined by $(X,Y)$, the [chain rule for conditional entropy](../../../../chain-rule-for-conditional-entropy.md) in its two orders gives

$$
H(X\mid Y)=H(X,E\mid Y)=H(E\mid Y)+H(X\mid E,Y).
$$

By [conditioning reduces entropy](../../../../conditioning-reduces-entropy.md), $H(E\mid Y)\leq H(E)$. On $E=0$, knowing $Y$ determines $X$, so the corresponding [conditional entropy](../../../../conditional-entropy.md) is zero. On $E=1$, at most $N-1$ symbols remain possible for $X$. The maximum [Shannon entropy](../../../../information-entropy-split.md) of a [probability distribution](../../../../probability-distribution-split.md) on at most $N-1$ symbols is $\log(N-1)$. Consequently

$$
\boxed{H(X\mid Y)\leq H(\mathbf1_{\{X\ne Y\}})+\Pr(X\ne Y)\log(N-1).}
$$

For an arbitrary [function](../../../../function-split.md) $g:\mathcal X\to\mathcal X$, repeat the argument with $E_g=\mathbf1_{\{X\ne g(Y)\}}$. This is still determined by $(X,Y)$; when it is zero, $X=g(Y)$, and when it is one, $X$ has at most $N-1$ possibilities for each $Y$. Thus [Fano's inequality](../../../../fano-s-inequality.md) gives

$$
\boxed{H(X\mid Y)\leq H(\mathbf1_{\{X\ne g(Y)\}})+\Pr(X\ne g(Y))\log(N-1).}
$$

Events of zero [probability](../../../../probability.md) contribute zero to the conditional average, covering the error [probabilities](../../../../probability.md) zero and one. If $N=1$, the left side and error [probabilities](../../../../probability.md) are zero; the trivial conclusion is handled separately instead of writing $0\log0$ as an ordinary finite product.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
