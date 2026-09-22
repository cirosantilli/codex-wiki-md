<h1 id="29l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [scalar](../../../../../../scalar.md) $\theta$, Taylor's theorem about the MLE, where  
$\ell_n'(\widehat\theta_n)=0$, gives some $\widetilde\theta_n$ between $\theta_0$ and $\widehat\theta_n$ such that

$$
\Lambda_n
=-\ell_n''(\widetilde\theta_n)
(\widehat\theta_n-\theta_0)^2.
$$

The Wald statistic is

$$
W_n(\theta_0)
=nI(\widehat\theta_n)(\widehat\theta_n-\theta_0)^2.
$$

Under the null, consistency gives  
$\widehat\theta_n,\widetilde\theta_n\to\theta_0$ in probability. A uniform law of large numbers for the observed information on a neighborhood of $\theta_0$ gives

$$
-\frac1n\ell_n''(\widetilde\theta_n)\xrightarrow P I(\theta_0),
\qquad
I(\widehat\theta_n)\xrightarrow P I(\theta_0)>0.
$$

Cancellation of the common squared displacement and Slutsky's theorem prove the [Wald and likelihood-ratio asymptotic equivalence](../../../../../../wald-and-likelihood-ratio-asymptotic-equivalence.md)

$$
\boxed{\frac{\Lambda_n}{W_n(\theta_0)}\xrightarrow P1}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29L](../../29l.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
