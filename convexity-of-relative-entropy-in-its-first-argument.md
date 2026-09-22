# Convexity of relative entropy in its first argument

↑ **Parent:** [Kullback-Leibler divergence](kullback-leibler-divergence.md)

For a fixed [probability mass function](probability-mass-function.md) $p$ on a [finite alphabet](finite-alphabet.md), [relative entropy](kullback-leibler-divergence.md) is a [convex function](convex-function.md) of its first [probability mass function](probability-mass-function.md). For $p_i>0$, the coordinate function $f_i(t)=t\log_2(t/p_i)$ has $f_i''(t)=1/(t\ln2)>0$ on $(0,\infty)$ and extends continuously with $f_i(0)=0$. Applying scalar [convexity](convex-function.md) coordinate by coordinate proves the inequality. If $p_i=0$, finite [relative entropy](kullback-leibler-divergence.md) requires $q_i=r_i=0$ for every positive-weight constituent; otherwise the right side is infinite. Thus the assertion also holds as an extended-valued [convexity](convex-function.md) statement. On the [probability simplex](probability-simplex.md) supported where $p>0$, the function is [strictly convex](strictly-convex-function.md): two distinct [probability mass functions](probability-mass-function.md) give a strict inequality for $0<\lambda<1$.

## ↑ Ancestors (6)

1. [Kullback-Leibler divergence](kullback-leibler-divergence.md)
2. [f-divergence](f-divergence-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Monotonicity of expected empirical relative entropy](monotonicity-of-expected-empirical-relative-entropy.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/1/b/iii/solution.md)
