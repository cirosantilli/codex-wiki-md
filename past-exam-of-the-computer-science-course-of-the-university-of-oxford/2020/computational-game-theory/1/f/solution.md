<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $P=999/1000$. If

$$
t>P\quad\Longleftrightarrow\quad
\frac n{n+3}>\frac{999}{1000}
\quad\Longleftrightarrow\quad
\boxed{n>2997},
$$

then both players prefer buying against a buyer, since $(t-P)/2>0$. Both prefer not buying against a nonbuyer: $2t/3<2/3<P$ and $t/3<1/3<P$. These strict opposite [best responses](../../../../../best-response.md) give the interior crossing of a [coordination game](../../../../../coordination-game.md).

An explicit [fully mixed Nash equilibrium](../../../../../fully-mixed-nash-equilibrium.md) follows from indifference. Let $p$ be X's [probability](../../../../../probability.md) of buying and $q$ Y's. X is indifferent when

$$
(1-q)\left(\frac{2t}{3}-P\right)+q\frac{t-P}{2}=0,
$$

and Y is indifferent when

$$
(1-p)\left(\frac t3-P\right)+p\frac{t-P}{2}=0.
$$

Solving gives

$$
\boxed{
p=\frac{2(P-t/3)}{P+t/3},\qquad
q=\frac{2(P-2t/3)}{P-t/3},\qquad t=\frac n{n+3},\ n>2997.
}
$$

Both numerators and denominators are positive. For $p<1$ the required inequality is $2P-2t/3<P+t/3$, equivalent to $P<t$; the same comparison for $q<1$ again reduces to $P<t$. Thus $p,q\in(0,1)$, and the equations make both actions [best responses](../../../../../best-response.md) for each player. By linearity of [expected payoff](../../../../../expected-payoff.md), neither player can profit by any other [mixed strategy](../../../../../mixed-strategy.md). At $n=2997$ these formulas reach $p=q=1$ and are not fully mixed; the strict threshold matters.

## ↑ Ancestors (11)

1. [F](../f.md)
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
