# Fisher information in an exponential survival snapshot

↑ **Parent:** [Fisher information matrix](fisher-information-matrix.md)

For $n$ [independent](independent-random-variables.md) [exponential](exponential-distribution.md) lifetimes with rate $\lambda$, recording all lifetimes gives [Fisher information](fisher-information-matrix.md) $n/\lambda^2$. Recording only the count alive at a fixed time $T>0$ gives a [binomial distribution](binomial-distribution.md) with success probability $s=e^{-\lambda T}$. Its information in $s$ is $n/[s(1-s)]$, and the change of parameter $ds/d\lambda=-Ts$ gives the displayed information.

The retained fraction is $R(z)=z^2/(e^z-1)$, $z=\lambda T$. It is strictly below one, so every single snapshot loses information. The inequality follows, for instance, from $h(z)=e^z-1-z^2$: its [derivative](derivative.md) is $e^z-2z>0$ for positive $z$, because that [derivative](derivative.md) has its [minimum](local-minimum.md) at $z=\log2$ with value $2-2\log2>0$. Also $R(z)$ tends to zero as $z\downarrow0$ and as $z\to\infty$.

Differentiating $R$ shows that the best snapshot time solves $2(1-e^{-z})=z$. The difference of the two sides is strictly concave, starts at zero with positive [derivative](derivative.md), and eventually becomes negative, so it has exactly one positive root, approximately $1.59362$. The largest retained fraction is about $0.64761$. Thus even an optimally timed snapshot keeps less than two thirds of the full lifetime information. This is a local design result: choosing that time requires a nominal rate or a preceding estimate.

## ↑ Ancestors (8)

1. [Fisher information matrix](fisher-information-matrix.md)
2. [Informant function](informant-function.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2008/o/4/solution.md)
