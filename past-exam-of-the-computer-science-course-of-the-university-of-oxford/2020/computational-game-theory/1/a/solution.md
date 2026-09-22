<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a simultaneous two-player [normal-form game](../../../../../normal-form-game.md), with X choosing the row and Y the column. Each player's [pure strategies](../../../../../pure-strategy.md) are $b$ and $nb$; a [payoff](../../../../../payoff.md) pair lists X first. Measure every dataset size in millions and use the stated normalization $M=1$. The source's reference to a shared half as “points” is interpreted in the same million-point units as the corpus, so the shared addition is $n/2$ to each initial dataset.

The [bimatrix game](../../../../../bimatrix-game.md) has [payoffs](../../../../../payoff.md)

$$
\begin{array}{c|cc}
 &Y:b&Y:nb\\ \hline
X:b&
\left(\dfrac{n+2}{2(n+3)}-\dfrac P2,\ 
\dfrac{n+4}{2(n+3)}-\dfrac P2\right)&
\left(\dfrac{n+1}{n+3}-P,\ \dfrac2{n+3}\right)\\[6pt]
X:nb&
\left(\dfrac1{n+3},\ \dfrac{n+2}{n+3}-P\right)&
\left(\dfrac13,\ \dfrac23\right).
\end{array}
$$

For example, joint purchase gives dataset sizes $1+n/2$ and $2+n/2$, total $3+n$, and each buyer pays $P/2$. A sole buyer gets the full corpus and pays $P$. The total [payoff](../../../../../payoff.md) is $1-P$ whenever a purchase occurs and $1$ when neither buys: the [game](../../../../../game.md) is not a [zero-sum game](../../../../../zero-sum-game.md), even though gross market shares always sum to one.

For the following calculations, set

$$
t=\frac n{n+3},\qquad 0<t<1.
$$

The [payoff](../../../../../payoff.md) differences “buy minus do not buy,” with the other player's action held fixed, are

$$
\begin{array}{c|cc}
 &\text{opponent does not buy}&\text{opponent buys}\\ \hline
\Delta_X&\dfrac{2t}{3}-P&\dfrac{t-P}{2}\\[4pt]
\Delta_Y&\dfrac t3-P&\dfrac{t-P}{2}.
\end{array}
$$

These four differences give all the [best response](../../../../../best-response.md) comparisons without mixing up row and column [payoffs](../../../../../payoff.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
