<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

As a function of the independent edge indicators, the maximum matching number is unit-Lipschitz. The event $f(G)\geq k$ is certified by exhibiting the $k$ present edges of a matching, so $f$ is $g(k)=k$ certifiable. The [Talagrand concentration inequality for certifiable functions](../../../../../../talagrand-concentration-inequality-for-certifiable-functions.md) around a median $M$ gives, for universal constants in the displayed standard version,

$$
\mathbb P(f(G)\leq M-t)\leq2e^{-t^2/(4M)},
\qquad
\mathbb P(f(G)\geq M+t)\leq2e^{-t^2/[4(M+t)]}.
$$

Here $M\asymp\sqrt n$. If $t/n^{1/4}\to\infty$, then $t^2/(M+t)\to\infty$, as does $t^2/M$ whenever the corresponding event is possible. Both tail probabilities therefore tend to zero. Thus deviations of any order larger than $n^{1/4}$ are unlikely.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
