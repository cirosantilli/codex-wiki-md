<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $P_k$ be the initial proposer's share, measured as a fraction of the pie currently available, with $k$ rounds remaining. The last-round argument in part (e) gives $P_1=1$. Rejecting an offer leaves the responder as next proposer with a pie smaller by factor $\alpha$, so its continuation value is $\alpha P_{k-1}$. The current proposer offers exactly that amount, which is accepted by the [continuous-offer bargaining acceptance lemma](../../../../../continuous-offer-bargaining-acceptance-lemma.md). Hence

$$
P_k=1-\alpha P_{k-1},\qquad\boxed{P_k=1-\alpha+\alpha^2-\cdots+(-\alpha)^{k-1}=\frac{1-(-\alpha)^k}{1+\alpha}.}
$$

The formula follows by summing a finite [geometric series](../../../../../geometric-series.md), or by induction in the recurrence. Agreement is immediate in every subgame, so this share is player 1's actual initial payoff.

For odd $k$, $P_k=(1+\alpha^k)/(1+\alpha)$ lies above $1/(1+\alpha)$ and decreases with $k$. For even $k$, $P_k=(1-\alpha^k)/(1+\alpha)$ lies below that value and increases with $k$. Thus prefer odd to even, fewer rounds among odd choices, and more rounds among even choices. For the given $k_1<k_2$, this simplifies to **choose $k_1$ if $k_1$ is odd, and choose $k_2$ if $k_1$ is even**. All comparisons are strict because $0<\alpha<1$. This is the [finite-horizon bargaining parity effect](../../../../../finite-horizon-bargaining-parity-effect.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
