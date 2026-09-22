# Newton iteration at a multiple root

↑ **Parent:** [Newton root-finding iteration](newton-root-finding-iteration.md)

If a sufficiently smooth [function](function-split.md) has the form $f(x)=(x-\alpha)^m q(x)$ with $m>1$ and $q(\alpha)\ne0$, then the [Newton root-finding iteration](newton-root-finding-iteration.md) satisfies

$$
x_{k+1}-\alpha=(x_k-\alpha)\left(1-\frac{q(x_k)}{m q(x_k)+(x_k-\alpha)q'(x_k)}\right).
$$

Thus the ratio of successive nonzero errors tends to $(m-1)/m$: the usual iteration has only [linear convergence](linear-convergence.md). Cancelling the common factor in $f/f'$ produces a continuous extension at the [multiple root](multiple-root.md), although the original quotient is undefined there. An implementation should stop upon finding an exact [zero of a function](zero-of-a-function.md).

## ↑ Ancestors (6)

1. [Newton root-finding iteration](newton-root-finding-iteration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iv/7/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/6/e/solution.md)
