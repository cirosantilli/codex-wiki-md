# Two-phase simplex

↑ **Parent:** [Simplex method](simplex-method.md)

Phase I introduces nonnegative artificial variables to create a feasible basis and minimizes their sum, or maximizes its negative. A positive minimum proves infeasibility. At a zero minimum, remove artificial variables and use the resulting feasible original basis in Phase II with the original objective. If an artificial variable remains basic at zero, pivot it out when possible; otherwise its row is redundant. Each phase uses the [simplex ratio test](simplex-ratio-test.md) to preserve nonnegative basic values.

## ↑ Ancestors (6)

1. [Simplex method](simplex-method.md)
2. [Linear programming](linear-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/15h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/23g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/20c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-42/2/a/solution.md)
