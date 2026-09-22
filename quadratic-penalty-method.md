# Quadratic penalty method

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)

For constraints $h=0$, $g\geq0$, minimize the displayed [merit function](merit-function.md) for progressively smaller $\mu>0$, where $g_i^- =\min(g_i,0)$. Increasing the quadratic penalty discourages [constraint violation](constraint-violation.md). In a violated inequality, differentiation gives the multiplier estimate $\lambda_i=-g_i/\mu$; an inactive inequality has estimate zero. Thus obtaining small violations by this method alone typically requires a very small $\mu$, which may cause a large [condition number](condition-number.md) in the inner minimization.

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Augmented Lagrangian method](augmented-lagrangian-method.md)
- [L1 exact penalty](l1-exact-penalty.md)
- [Merit function](merit-function.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/1/iv/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/5/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/5/iii/solution.md)
- [Penalty method](penalty-method.md)
