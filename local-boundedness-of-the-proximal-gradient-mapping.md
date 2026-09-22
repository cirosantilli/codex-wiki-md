# Local boundedness of the proximal gradient mapping

↑ **Parent:** [Proximal gradient method](proximal-gradient-method.md)

Fix $x$ with nonempty [subdifferential](subdifferential.md) $\partial h(x)$ for a [convex function](convex-function.md) $h$. If $p=x-\alpha G_\alpha(x)$ and $v=G_\alpha(x)-\nabla f(x)\in\partial h(p)$, [monotonicity of a convex subdifferential](monotonicity-of-a-convex-subdifferential.md) gives $(v-w)^T(p-x)\geq0$ for any fixed $w\in\partial h(x)$. Hence

$$
\|G_\alpha(x)\|^2\leq(\nabla f(x)+w)^TG_\alpha(x)\leq\|\nabla f(x)+w\|\,\|G_\alpha(x)\|.
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) proves the bound uniformly for $\alpha>0$. If $f$ has an $L$-[Lipschitz gradient](lipschitz-gradient.md), this makes the remainder in the [proximal gradient mapping](proximal-gradient-mapping.md) descent bound at most $L\alpha^2\|\nabla f(x)+w\|^2/2$. Thus the [big O notation](big-o-notation.md) $O(\alpha^2)$ is justified despite the dependence of the [proximal gradient mapping](proximal-gradient-mapping.md) on $\alpha$.

```
Target: convex-optimization.bigb, under Coordinate descent.
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

- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/1/d/solution.md)
