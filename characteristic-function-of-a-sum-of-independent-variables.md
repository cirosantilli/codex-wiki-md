# Characteristic function of a sum of independent variables

↑ **Parent:** [Characteristic function](characteristic-function-split.md)

Independence makes the characteristic function of a sum equal the product of the individual characteristic functions.

For mutually [independent random variables](independent-random-variables.md) $X_1,\ldots,X_n$, write $S_n=\sum_{j=1}^nX_j$. Then

$$
\varphi_{S_n}(t)=\mathbb E\left[\prod_{j=1}^ne^{itX_j}\right]
=\prod_{j=1}^n\mathbb E[e^{itX_j}]
=\prod_{j=1}^n\varphi_{X_j}(t).
$$

This is the [expectation of a product of independent random variables](expectation-of-a-product-of-independent-random-variables.md) applied to bounded [complex exponentials](complex-exponential-function.md); no [moment](moment.md) hypothesis is needed.[§3.3.1, Theorem 3.3.2 and proof, printed p. 126](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

Identical [probability distributions](probability-distribution-split.md) are unnecessary. When the [random variables](random-variable-split.md) are [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md), the product is $\varphi_X(t)^n$. A deterministic rescaling also follows directly from the definition: $\varphi_{aX+b}(t)=e^{itb}\varphi_X(at)$ for real $a,b$. Consequently the [sample mean](sample-mean.md) has [characteristic function](characteristic-function-split.md) $\varphi_X(t/n)^n$, and a sum divided by $\sqrt n$ has [characteristic function](characteristic-function-split.md) $\varphi_X(t/\sqrt n)^n$.

The [independence](independent-random-variables.md) assumption does real work. Let $X$ take $-1$ and $1$ with equal [probabilities](probability.md) and set $Y=X$. Both [characteristic functions](characteristic-function-split.md) are $\cos t$, but $\varphi_{X+Y}(t)=\cos(2t)$, not $\cos^2t$. At $t=\pi/2$ they give $-1$ and zero respectively. Knowing the two marginal [probability distributions](probability-distribution-split.md) does not determine the sum without their [joint probability distribution](joint-probability-distribution.md).

**Table of contents**

- [Three Bernoulli variables through characteristic functions](three-bernoulli-variables-through-characteristic-functions.md)
- [Characteristic functions of symmetric sign sums](characteristic-functions-of-symmetric-sign-sums.md)

## ↑ Ancestors (6)

1. [Characteristic function](characteristic-function-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Characteristic function](characteristic-function-split.md)
- [Dyadic cosine product](dyadic-cosine-product.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/26k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-201/5/c/solution.md)
