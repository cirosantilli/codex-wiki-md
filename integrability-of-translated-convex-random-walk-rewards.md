# Integrability of translated convex random-walk rewards

↑ **Parent:** [Optimal stopping value function](optimal-stopping-value-function.md)

Let $Z_j$ be the sum of $j$ independent identically distributed real increments. For a finite [convex function](convex-function.md) $f$, integrability of $f(Z_j)$ and $f(Z_{j+1})$ implies integrability of $f(Z_j+x)$ for every fixed $x$. Its negative part is controlled by [negative part of a finite convex function is Lipschitz](negative-part-of-a-finite-convex-function-is-lipschitz.md). For $x>0$, if the increment law is unbounded above, take an independent increment $\eta$ with $p=\mathbb P(\eta\geq x)>0$. On this event convexity gives $f(Z_j+x)^+\leq f(Z_j)^++f(Z_j+\eta)^+$, so the expectation is bounded by $\mathbb E f(Z_j)^++p^{-1}\mathbb E f(Z_{j+1})^+$. If increments are bounded above by $M$, use $Z_j\leq jM$ and bound the positive part by $f(Z_j)^++f(jM+x)^+$. For $x<0$, use the symmetric lower-tail argument. This supplies translated integrability without assuming integrable increments or a growth bound on $f$.

## ↑ Ancestors (9)

1. [Optimal stopping value function](optimal-stopping-value-function.md)
2. [Optimal stopping](optimal-stopping.md)
3. [Snell envelope](snell-envelope.md)
4. [Martingale](martingale-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Convexity of a random-walk Snell value function](convexity-of-a-random-walk-snell-value-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/3/c/solution.md)
