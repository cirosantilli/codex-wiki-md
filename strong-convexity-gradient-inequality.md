# Strong convexity gradient inequality

↑ **Parent:** [Strongly convex function](strongly-convex-function.md)

For a [differentiable](differentiable-function.md) [strongly convex function](strongly-convex-function.md) with modulus $\gamma>0$ and [global minimizer](global-minimizer.md) $x^*$, the supporting inequality gives

$$
f(x^*)\geq f(x)+\nabla f(x)^T(x^*-x)+\frac\gamma2\|x^*-x\|^2.
$$

Completing the square shows that the last two terms are at least $-\|\nabla f(x)\|^2/(2\gamma)$, which proves the result. Combining this with the [descent lemma](descent-lemma.md) converts squared [gradient](gradient.md) decrease into a contraction of the [objective function](objective-function.md) gap.

```
Target: mathematical-optimization.bigb, under Line search.
```

## ↑ Ancestors (7)

1. [Strongly convex function](strongly-convex-function.md)
2. [Convex function](convex-function.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/d/solution.md)
- [Randomized block coordinate descent](randomized-block-coordinate-descent.md)
