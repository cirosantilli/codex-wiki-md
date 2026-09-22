# Proximal gradient objective error bound

↑ **Parent:** [Proximal gradient method](proximal-gradient-method.md)

For $\phi=f+h$, with $f$ a [convex function](convex-function.md) having an $L$-[Lipschitz gradient](lipschitz-gradient.md) and $h$ a [proper convex function](proper-convex-function.md) with a well-defined [proximal operator](proximal-operator.md), the [proximal gradient method](proximal-gradient-method.md) with [step size](step-size.md) $1/L$ satisfies the displayed bound whenever a [global minimizer](global-minimizer.md) $x^*$ exists. The one-step [subgradient inequality](subgradient-inequality.md) and [descent lemma](descent-lemma.md) give

$$
\phi(x^{j+1})-\phi(x^*)\leq\frac L2\big(\|x^j-x^*\|^2-\|x^{j+1}-x^*\|^2\big).
$$

The [objective function](objective-function.md) values are nonincreasing. A [telescoping sum](telescoping-sum.md) over $j=0,\ldots,k-1$, followed by comparison of the last error with the [arithmetic mean](arithmetic-mean.md) of the errors, proves the result. The bound controls the last [objective function](objective-function.md) error without requiring a [strongly convex function](strongly-convex-function.md) or a unique [minimizer](global-minimizer.md).

```
Target: convex-optimization.bigb, under Proximal gradient method.
```

## ↑ Ancestors (7)

1. [Proximal gradient method](proximal-gradient-method.md)
2. [Proximal operator](proximal-operator.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/1/c/solution.md)
