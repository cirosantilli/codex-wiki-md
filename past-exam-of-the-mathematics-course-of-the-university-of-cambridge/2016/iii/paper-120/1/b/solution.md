<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the first tape of the [group multiplier automaton](../../../../../../group-multiplier-automaton.md) $M_x$ to be $u=a_1\cdots a_m$. Construct its possible runs by [dynamic programming](../../../../../../dynamic-programming.md), one column at a time. A record consists of a state and a flag indicating whether the output tape has ended. At column $i\leq m$, the first symbol is $a_i$ and the second symbol may be any letter of the [alphabet](../../../../../../alphabet.md), or $\#$; after the second tape first uses $\#$ it must continue to use $\#$. At later columns the first symbol is $\#$, and an additional column must have a genuine letter on the second tape. Never add a $(\#,\#)$ column.

Keep one predecessor record and its output symbol for each reachable state-and-flag pair in each layer. Two runs reaching the same record have exactly the same possible future completions, so this merging loses no accepting output. The merged [dead state of a finite automaton](../../../../../../dead-state-of-a-finite-automaton.md) can be discarded. At each layer $i\geq m$, test whether a reached state is accepting; the initial layer is included when $m=0$. Upon success, follow predecessor records backwards and omit padding symbols to recover $v$.

The [automatic structure for a group](../../../../../../automatic-structure-for-a-group.md) supplies a representative in $L$ of $\overline u x$, so an accepted [padded convolution of words](../../../../../../padded-convolution-of-words.md) exists and this search terminates. **The output is the required representative**:

$$
\boxed{v\in L,\qquad \overline v=\overline u x.}
$$

The search uses only the finite transition table; it does not presuppose a solution to the [word problem for a group](../../../../../../word-problem-for-groups.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
