# Integer-halving recurrence with constant toll

↑ **Parent:** [Recurrence relation](recurrence-relation.md)

If $S_0=a$ and $S_n=S_{\lfloor n/2\rfloor}+m$ for positive [integers](integer-split.md) $n$, each halving removes one binary digit until zero is reached. There are $1+\lfloor\log_2n\rfloor$ such steps. The formula follows by [strong induction](strong-induction.md), using $\lfloor\log_2\lfloor n/2\rfloor\rfloor=\lfloor\log_2n\rfloor-1$ for $n\geq2$ and checking $n=1$ separately. With fixed positive $m$, this is $\Theta(\log n)$ as $n\to\infty$; the zero case retains its separately defined value.

## ↑ Ancestors (8)

1. [Recurrence relation](recurrence-relation.md)
2. [Sequence](sequence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/discrete-mathematics-continuous-mathematics-and-probability/3/d/solution.md)
