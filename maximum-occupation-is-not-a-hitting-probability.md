# Maximum occupation is not a hitting probability

↑ **Parent:** [Hitting probability](hitting-probability.md)

For $Y_t=-vt+\sqrt{2D}\,B_t$ with $v,D,\ell>0$ and standard [Brownian motion](brownian-motion-split.md), the one-time occupation probability is $\tfrac12\operatorname{erfc}[(\ell+vt)/\sqrt{4Dt}]$. It is maximized at $t=\ell/v$, giving $\tfrac12\operatorname{erfc}(\sqrt{v\ell/D})$. The actual [hitting probability](hitting-probability.md) is $e^{-v\ell/D}$. To derive it, solve $Dh''-vh'=0$ on $(-A,\ell)$ with $h(-A)=0$, $h(\ell)=1$, obtaining $h(0)=(1-e^{-vA/D})/(e^{v\ell/D}-e^{-vA/D})$, and let $A\to\infty$. A path that reached the level and returned contributes to the latter event but not to a given one-time tail.

## ↑ Ancestors (8)

1. [Hitting probability](hitting-probability.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-70/2/solution.md)
