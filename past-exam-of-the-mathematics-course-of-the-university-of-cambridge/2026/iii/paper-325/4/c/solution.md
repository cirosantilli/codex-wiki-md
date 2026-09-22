<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $z_A,z_B\in\{+1,-1\}$ denote the two $Z$ outcomes and $x_C\in\{+1,-1\}$ the $X$ outcome. Measuring $Z_A$ in the [GHZ state](../../../../../../greenberger-horne-zeilinger-state.md) projects $B$ onto the same $Z$ eigenstate, while the later $X_C$ outcome is unbiased. Hence the possible triples, in the order $(z_A,x_C,z_B)$, are

$$
\boxed{(+,+,+),\ (+,-,+),\ (-,+,-),\ (-,-,-)},
$$

each with probability $1/4$.

Choose $(z_A,x_C,z_B)=(+,+,+)$. Immediately before $t=0$, each local readout is $I/2$. The collapse at $(t,x)=(0,0)$ is immediately in $A$'s past light cone, reaches $B$ at $t=1$, and reaches $C$ at $t=2$. Thus

$$
\begin{array}{c|c}
\text{qubit}&\text{state-readout output}\\ \hline
A&I/2\text{ for }t<0,\quad |0\rangle\langle0|\text{ for }t>0,\\
B&I/2\text{ for }0<t<1,\quad |0\rangle\langle0|\text{ for }t>1,\\
C&I/2\text{ for }0<t<2,\quad |0\rangle\langle0|\text{ for }2<t<3,\quad |+\rangle\langle+|\text{ for }t>3.
\end{array}
$$

Here $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$. The $X_C$ collapse at $(3,2)$ reaches $B$ at $t=4$ and $A$ at $t=5$, but the state is already a product after the first collapse, so it does not change their local states. Likewise, the $Z_B$ collapse at $(5,1)$ reaches $A$ and $C$ at $t=6$ without changing their states. For another allowed outcome, replace $|0\rangle$ by $|1\rangle$ according to $z_A=z_B$ and replace $|+\rangle$ by $|-\rangle$ according to $x_C$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
