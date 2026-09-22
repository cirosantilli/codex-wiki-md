# Proximal gradient mapping

↑ **Parent:** [Proximal gradient method](proximal-gradient-method.md)

For a [convex function](convex-function.md) $h$ with a well-defined [proximal operator](proximal-operator.md), and a [differentiable function](differentiable-function.md) $f$, the proximal gradient mapping is the displacement of one [proximal gradient method](proximal-gradient-method.md) update divided by its positive [step size](step-size.md) $\alpha$. Writing $p=x-\alpha G_\alpha(x)$, the [subgradient optimality condition](subgradient-optimality-condition.md) gives $G_\alpha(x)-\nabla f(x)\in\partial h(p)$. For [convex functions](convex-function.md) $f,h$, its zeros are precisely the [global minimizers](global-minimizer.md) of $f+h$, by the [subgradient optimality condition](subgradient-optimality-condition.md) and [subdifferential sum rule](subdifferential-sum-rule.md). When $h=0$, it is the ordinary [gradient](gradient.md).

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

## ← Incoming links (5)

- [Local boundedness of the proximal gradient mapping](local-boundedness-of-the-proximal-gradient-mapping.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/1/a/solution.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/1/b/solution.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/1/c/solution.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/1/d/solution.md)
