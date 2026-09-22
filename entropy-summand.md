# Entropy summand

↑ **Parent:** [Information entropy](information-entropy-split.md)

The contribution of a symbol with [probability](probability.md) $x$ to [Shannon entropy](information-entropy-split.md), with $f(0)=0$. It is a [concave function](concave-function.md) because $f''(x)=-1/(x\ln2)<0$ on $(0,1)$ and its endpoint extension is continuous. Its sharp bound for pairs exactly distance $v$ apart in $[0,1]$ is

$$
\max_{0\leq t\leq1-v}|f(t+v)-f(t)|=\max\{f(v),f(1-v)\}.
$$

To prove this, the increment $f(t+v)-f(t)$ decreases with $t$, from $f(v)$ to $-f(1-v)$. For $v\leq1/2$, the maximum is $f(v)$: the difference $f(v)-f(1-v)$ vanishes at zero and one half and has second [derivative](derivative.md) $(2v-1)/(v(1-v)\ln2)\leq0$ between them. Hence it is nonnegative by [concavity](concave-function.md).

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite-alphabet entropy continuity bound](finite-alphabet-entropy-continuity-bound.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/1/c/solution.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/1/d/solution.md)
