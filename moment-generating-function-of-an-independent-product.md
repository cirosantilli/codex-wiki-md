# Moment-generating function of an independent product

↑ **Parent:** [Moment-generating function](moment-generating-function.md)

If $U$ and $X$ are independent real [random variables](random-variable-split.md), then the [moment-generating function](moment-generating-function.md) of their product is $M_{UX}(t)=\mathbb E_U[M_X(tU)]$ wherever the expression is finite. This follows by conditioning on $U$: the conditional law of $X$ is unchanged by [independence](independent-random-variables.md), so $\mathbb E(e^{tUX}\mid U)=M_X(tU)$. For $U$ uniform on $(0,1)$, the formula becomes $M_{UX}(t)=\int_0^1M_X(tu)du$. If $M_X$ is finite on a neighborhood of zero, this product also has a finite [moment-generating function](moment-generating-function.md) on a neighborhood of zero, because the bounded factor $U$ keeps $tu$ between zero and $t$.

## ↑ Ancestors (7)

1. [Moment-generating function](moment-generating-function.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2010/m/m1/b/iv/solution.md)
