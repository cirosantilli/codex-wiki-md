# Randomized block coordinate descent

↑ **Parent:** [Coordinate descent](coordinate-descent.md)

A [coordinate descent](coordinate-descent.md) method that randomly selects a block and updates only its coordinates. Suppose each coordinate is selected with [probability](probability.md) $1/\ell$, every block has [Lipschitz constant](lipschitz-constant.md) at most $\beta$, and the [objective function](objective-function.md) is a [strongly convex function](strongly-convex-function.md) with modulus $\gamma>0$. The block [descent lemma](descent-lemma.md) and the [strong convexity gradient inequality](strong-convexity-gradient-inequality.md) give

$$
\mathbb E[f(X^{t+1})-f(x^*)\mid X^t]\leq\left(1-\frac\gamma{\ell\beta}\right)\big(f(X^t)-f(x^*)\big).
$$

For uniform blocks of size $m$ in $n=m\ell$ coordinates, $\ell$ updates constitute an [optimization epoch](optimization-epoch.md), and the [epoch complexity](epoch-complexity.md) is $O((\beta/\gamma)\log(\Delta_0/\varepsilon))$. Here $\Delta_0$ is the initial [objective function](objective-function.md) gap, and the target is its expected gap at most $\varepsilon$. A coordinate-based common bound is $\beta=m\max_iL_i$; actual constants can improve it.

```
Target: gradient-descent.bigb, under Gradient descent.
```

## ↑ Ancestors (6)

1. [Coordinate descent](coordinate-descent.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Epoch complexity](epoch-complexity.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/d/solution.md)
