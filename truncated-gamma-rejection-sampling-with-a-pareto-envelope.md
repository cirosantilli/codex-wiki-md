# Truncated gamma rejection sampling with a Pareto envelope

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

For target density proportional to $x^{\alpha-1}e^{-\beta x}$ on $x>a>0$, use the [Pareto distribution](pareto-distribution.md) proposal $g(x)=ba^bx^{-b-1}$ with $b>0$. Its density ratio is proportional to $x^{\alpha+b}e^{-\beta x}$, maximized at $(\alpha+b)/\beta$ if that point exceeds $a$. The tight envelope yields the highest acceptance probability for this fixed proposal. An inverse draw is $aU^{-1/b}$ with $U$ [uniformly distributed](continuous-uniform-distribution.md) on $(0,1)$.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/1/b/i/solution.md)
