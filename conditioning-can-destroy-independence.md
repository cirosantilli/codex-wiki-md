# Conditioning can destroy independence

↑ **Parent:** [Conditional independence](conditional-independence.md)

Return to [pairwise independence does not imply joint independence](pairwise-independence-does-not-imply-joint-independence.md), where $X,Y$ are [independent](independent-random-variables.md) fair [bits](bit.md) and $Z=X\mathbin\oplus Y$ is their [exclusive or](exclusive-or.md). Given $Z=0$, only $000$ and $110$ remain, each with conditional [probability](probability.md) $1/2$. Given $Z=1$, only $011$ and $101$ remain, again each with conditional [probability](probability.md) $1/2$. Consequently,

$$
J_{X,Y\mid Z=0}=\begin{pmatrix}1/2&0\\0&1/2\end{pmatrix},\qquad
J_{X,Y\mid Z=1}=\begin{pmatrix}0&1/2\\1/2&0\end{pmatrix}.
$$

The conditional [marginal distributions](marginal-distribution.md) are still fair, so their product has four entries $1/4$ in either case. The actual tables differ: $Y=X$ given $Z=0$, and $Y=1-X$ given $Z=1$. Thus unconditional [independence](independent-random-variables.md) need not survive conditioning. Observing whether two [bits](bit.md) agree restricts their possible combinations; no physical interaction between the original trials is required to produce that information constraint.

## ↑ Ancestors (8)

1. [Conditional independence](conditional-independence.md)
2. [Independent random variables](independent-random-variables.md)
3. [Random variable](random-variable-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
