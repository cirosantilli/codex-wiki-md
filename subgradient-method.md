# Subgradient method

↑ **Parent:** [Convex optimization](convex-optimization-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subgradient_method)

The subgradient method minimizes a possibly nonsmooth [convex function](convex-function.md) by choosing $g_k\in\partial f(x_k)$ and iterating

$$
x_{k+1}=x_k-t_kg_k.
$$

If the [subgradients](subgradient.md) are bounded by $G$ and a minimizer is within distance $R$ of $x_0$, a suitable constant or diminishing [step size](step-size.md) finds objective error at most $\epsilon$ in $O(R^2G^2/\epsilon^2)$ iterations.

## ↑ Ancestors (5)

1. [Convex optimization](convex-optimization-split.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/1/e/solution.md)
