# Milne device for forward and backward Euler

↑ **Parent:** [Linear stability domain](linear-stability-domain.md)

Starting at the same value, forward and backward Euler have opposite leading local errors. Their half-difference therefore estimates either local error:

$$
E_n=\frac12\lVert y_B-y_F\rVert.
$$

For a first-order method, a local-tolerance controller consequently scales the next step by $(\mathrm{tol}/E_n)^{1/2}$, usually with a safety factor.

## ↑ Ancestors (6)

1. [Linear stability domain](linear-stability-domain.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/17d/c/solution.md)
