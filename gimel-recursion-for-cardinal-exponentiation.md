# Gimel recursion for cardinal exponentiation

↑ **Parent:** [Gimel function](gimel-function.md)

The [Gimel function](gimel-function.md) determines all infinite [cardinal](cardinal-number.md) powers. For a regular base, $2^\kappa=\gimel(\kappa)$. For a singular base, put $s=\sup_{\rho<\kappa}2^\rho$ and $\theta=\operatorname{cf}(\kappa)$; then $2^\kappa=s^\theta$, which is $s$ if attained below $\kappa$ and $\gimel(s)$ otherwise. After these powers are known, fix an infinite exponent $\lambda$ and recurse on the base. Below $\lambda$ use $2^\lambda$; at successors use the [Hausdorff formula for cardinal exponentiation](hausdorff-formula-for-cardinal-exponentiation.md). At a limit base greater than $\lambda$, put $a=\sup_{\rho<\kappa}\rho^\lambda$. The answer is $a$ if $\operatorname{cf}(\kappa)>\lambda$ or the supremum is attained, and $\gimel(a)$ otherwise. In the nonattained cases, the cofinal-index argument identifies the [cofinality](cofinality.md) of the supremum.

## ↑ Ancestors (8)

1. [Gimel function](gimel-function.md)
2. [Cardinal arithmetic](cardinal-arithmetic.md)
3. [Cardinal number](cardinal-number.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19/3/iii/solution.md)
