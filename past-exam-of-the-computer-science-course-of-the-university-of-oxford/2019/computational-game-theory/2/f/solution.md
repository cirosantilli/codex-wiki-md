<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Compute $C=\max_jc_j$ and $D=\max_jd_j$ in one pass. Scan the columns again: return the top cell of column $j$ if $c_j=C$ and $a_j\geq b_j$, or its bottom cell if $d_j=D$ and $b_j\geq a_j$. Each test is exactly mutual [best response](../../../../../best-response.md), so any returned cell is a pure [Nash equilibrium](../../../../../nash-equilibrium.md).

If none is found, part (e) supplies columns

$$
\begin{pmatrix}(1,0)\\(0,1)\end{pmatrix},\qquad\begin{pmatrix}(0,1)\\(1,0)\end{pmatrix}.
$$

Locate one of each and mix with [probability](../../../../../probability.md) $1/2$ on each of those two columns, while the row player mixes $1/2$ on each row. The two row actions then both have [expected payoff](../../../../../expected-payoff.md) $1/2$.

To check all opposing deviations, observe that no column can have $(c_j,d_j)=(1,1)$. Such a column would maximize the column player's [payoff](../../../../../payoff.md) in either row; choosing a row-player [best response](../../../../../best-response.md) within it would give a pure equilibrium, contrary to the failed scan. Therefore every column has $c_j+d_j\leq1$, and against the equal row mixture its [expected payoff](../../../../../expected-payoff.md) is at most $1/2$. The two supported columns attain that bound.

Hence **the returned half-half profile is a [Nash equilibrium](../../../../../nash-equilibrium.md) against every column, not only the two supported ones**. A constant number of scans takes **$O(n)$ [running time](../../../../../running-time.md)**, with constant auxiliary storage if the output mixture is represented by its two supported column indices and probabilities. This is the construction in [equilibrium in a two-row binary game](../../../../../equilibrium-in-a-two-row-binary-game.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
