<h1 id="o/o5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a regular one-parameter model with joint density $f_\theta(x)$, write the [score function](../../../../../informant-function.md) as $U_\theta=\partial_\theta\log f_\theta(X)$ and the [Fisher information](../../../../../fisher-information-matrix.md) as $I_n(\theta)=\mathbb E_\theta[U_\theta^2]$. Assume a parameter-independent support, differentiability and sufficient domination to interchange parameter differentiation and integration, and $0<I_n(\theta)<\infty$. If $T$ has finite [variance](../../../../../variance-split.md) and is unbiased for a differentiable target $g(\theta)$, the [Cramér-Rao lower bound](../../../../../cramer-rao-bound.md) is

$$
\boxed{\operatorname{Var}_\theta(T)\geq\frac{[g'(\theta)]^2}{I_n(\theta)}}.
$$

Indeed, differentiating total mass gives $\mathbb E_\theta U_\theta=0$, and differentiating $\mathbb E_\theta T=g(\theta)$ gives $\operatorname{Cov}_\theta(T,U_\theta)=g'(\theta)$. [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) proves the bound. For $n$ independent identically distributed observations, information adds: $I_n=nI_1$. In particular for the parameter itself, $g(\theta)=\theta$, the bound is $1/I_n$. The assumptions are material: the same formula cannot simply be imposed on models with parameter-dependent support.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
