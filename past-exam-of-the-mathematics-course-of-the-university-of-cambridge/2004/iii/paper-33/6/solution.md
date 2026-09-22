<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For [pure strategy](../../../../../pure-strategy.md) sets $S_1,\ldots,S_n$ and [utility functions](../../../../../utility-function-split.md) $u_i$, a [Nash equilibrium](../../../../../nash-equilibrium.md) is a strategy profile $a$ such that

$$
\boxed{u_i(a_i,a_{-i})\geq u_i(b_i,a_{-i})
\quad\text{for every player }i\text{ and every }b_i\in S_i.}
$$

For [mixed strategies](../../../../../mixed-strategy.md), replace payoffs by their expectations under independent randomization and allow each player to choose any [probability distribution](../../../../../probability-distribution.md). Since [expected utility](../../../../../expected-utility.md) is linear in a player's own distribution, checking all pure deviations suffices.

Pure equilibria need not exist. In [matching pennies](../../../../../matching-pennies.md), player 1 receives $1$ for equal choices and $-1$ for different choices, while player 2 receives the negative. At an equal pair, player 2 improves by switching; at a different pair, player 1 improves by switching. Thus no pure profile is a [Nash equilibrium](../../../../../nash-equilibrium.md).

In the [ranked university application game](../../../../../ranked-university-application-game.md), every student must be admitted at a pure equilibrium. If someone were rejected, fewer than the total 50000 seats would be filled, so another university would have a vacancy. Moving there gives positive benefit instead of zero. Consequently all 50 universities have exactly 1000 applicants and admit all of them.

Choose a university with largest [arithmetic mean](../../../../../arithmetic-mean.md) admitted rank and let $r_{\min}$ be its lowest rank. If an outside student of rank $r>r_{\min}$ moved there, that student would be admitted in place of $r_{\min}$; the new [arithmetic mean](../../../../../arithmetic-mean.md) would exceed the university's previous [arithmetic mean](../../../../../arithmetic-mean.md), which was at least the student's current payoff. This is a profitable deviation. Therefore no higher rank is outside: that university consists of the highest 1000 ranks. Remove that block and repeat with the remaining university of largest [arithmetic mean](../../../../../arithmetic-mean.md). At each step the same argument excludes omitted higher ranks from the remaining set. The admitted cohorts are necessarily the consecutive blocks

$$
\{1,\ldots,1000\},\{1001,\ldots,2000\},\ldots,
\{49001,\ldots,50000\}.
$$

Conversely, assigning these blocks to labelled universities is an equilibrium. A student moving to a higher block is rejected. A student moving to a lower block displaces its lowest rank; all the other admitted ranks there are below every rank in the student's original block. Comparing the two [arithmetic means](../../../../../arithmetic-mean.md) with that student's own rank held fixed shows a strict loss. Thus every block assignment is an equilibrium, and the preceding argument excludes all other pure ones:

$$
\boxed{\text{there are exactly }50!\text{ pure Nash equilibria}.}
$$

There is **more than one further mixed equilibrium**. We give two genuinely mixed profiles, rather than count the pure equilibria as degenerate mixed ones. First, let every student apply independently and uniformly to all 50 universities. For each fixed student the other players' distribution is invariant under every [permutation](../../../../../permutation.md) of university labels. All 50 pure applications therefore give the same [expected utility](../../../../../expected-utility.md). Uniform mixing is a [best response](../../../../../best-response.md), so this is a [Nash equilibrium](../../../../../nash-equilibrium.md).

For a distinct mixed equilibrium, assign each of the 48 highest consecutive rank blocks deterministically to a different university. Let each of the lowest 2000 students independently choose either of the two remaining universities with [probability](../../../../../probability.md) $1/2$. For a low-ranked student these two universities have identical [expected utility](../../../../../expected-utility.md) by label symmetry, and that payoff is positive: there is a positive-probability event on which the student is admitted. Applying to one of the 48 full higher-ranked blocks would guarantee rejection. Hence the specified mixture is a [best response](../../../../../best-response.md).

For a student in a deterministic higher block, moving to another deterministic block loses by the pure-equilibrium comparison above. It remains to rule out a move to a mixed university. Let the student's own block start at $L\geq2001$, and let their rank be $r\leq L+999$. Their present payoff is $L+499.5$. The number $M$ of low-ranked applicants at a specified mixed university has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $(2000,1/2)$, and the higher-ranked deviator is always admitted. If $M\geq1$, all other admitted ranks are at most 2000, so the new [arithmetic mean](../../../../../arithmetic-mean.md) is at most $(r+2000)/2$, and thus at most $(L+2999)/2$. If $M=0$, it is $r\leq50000$. Therefore the expected deviation payoff is at most

$$
\frac{L+2999}{2}+50000\,2^{-2000}
<L+499.5,
$$

because the gap without the last term is $(L-2000)/2\geq1/2$. No such deviation improves the payoff. This proves a second mixed equilibrium, with only the lowest 2000 students randomizing. It is visibly different from the fully uniform profile. In particular,

$$
\boxed{\text{the answer to the mixed-equilibrium alternative is “more than one”.}}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
