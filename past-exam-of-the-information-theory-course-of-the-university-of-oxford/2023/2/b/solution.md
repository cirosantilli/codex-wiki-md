<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a fixed estimated [probability mass function](../../../../probability-mass-function.md) $q$, the estimated [joint probability mass function](../../../../joint-probability-mass-function.md) is $q_n(x_1,\ldots,x_n)=\prod_iq(x_i)$. If $q(x)>0$ whenever $p(x)>0$, the [strong law of large numbers](../../../../strong-law-of-large-numbers.md) gives the [mismatched asymptotic equipartition property](../../../../mismatched-asymptotic-equipartition-property.md):

$$
\boxed{\frac1n\log q_n(X_1,\ldots,X_n)\longrightarrow
\sum_{x:p(x)>0}p(x)\log q(x)
=-H(p,q)=-H(p)-D_{\mathrm{KL}}(p\Vert q)
\quad\text{almost surely}.}
$$

Here $H(p,q)$ is [cross-entropy](../../../../cross-entropy.md), and the last equality is [cross-entropy equals entropy plus relative entropy](../../../../cross-entropy-equals-entropy-plus-relative-entropy.md). The [Kullback-Leibler divergence](../../../../kullback-leibler-divergence.md) measures the extra average [logarithmic loss](../../../../logarithmic-loss.md) from the estimated law.

If $q(x)=0$ for some $x$ with $p(x)>0$, let $a=\sum_{x:q(x)=0}p(x)>0$. The [probability](../../../../probability.md) that none of the first $n$ observations belongs to this set is $(1-a)^n\to0$. Almost surely such a symbol eventually occurs, after which $q_n(X_1,\ldots,X_n)=0$ forever. Thus the limit is **$-\infty$**, consistent with infinite [cross-entropy](../../../../cross-entropy.md) and infinite [Kullback-Leibler divergence](../../../../kullback-leibler-divergence.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
