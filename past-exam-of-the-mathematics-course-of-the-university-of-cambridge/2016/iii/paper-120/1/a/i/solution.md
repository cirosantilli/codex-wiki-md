<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the synchronous [group multiplier automata](../../../../../../../group-multiplier-automaton.md) belonging to the [automatic structure for a group](../../../../../../../automatic-structure-for-a-group.md). Write $u\otimes v$ for the [padded convolution of words](../../../../../../../padded-convolution-of-words.md): the shorter tape is completed with a symbol $\#$ outside the [alphabet](../../../../../../../alphabet.md), and reading stops when both [words over an alphabet](../../../../../../../string.md) have ended. Our convention is

$$
M_x\text{ accepts }u\otimes v
\quad\Longleftrightarrow\quad
u,v\in L\text{ and }\overline u\,x=\overline v.
$$

Let $N\geq1$ be at least the number of states of each of these [finite-state automata](../../../../../../../finite-state-machine.md), including $M_\varepsilon$.

Choose a shortest representative $v\in L$ of $g$. In the first orientation, $M_x$ accepts $w\otimes v$; in the other orientation it accepts $v\otimes w$. If $|v|>|w|+N$, the accepting run has more than $N$ transitions after the tape containing $w$ has ended. Two states in that suffix coincide. Delete the intervening nonempty loop. Every deleted column contains $\#$ on the fixed tape and a genuine letter on the tape containing $v$, so the resulting input remains a valid [padded convolution of words](../../../../../../../padded-convolution-of-words.md). The [group multiplier automaton](../../../../../../../group-multiplier-automaton.md) still accepts, giving a shorter representative of the same $g$. This contradicts minimality. Thus **a representative can always be chosen with**

$$
\boxed{|v|\leq |w|+N.}
$$

This argument does not require a symmetric [alphabet](../../../../../../../alphabet.md): the second orientation uses the same $M_x$ with its tapes interchanged in the input, rather than a presumed $M_{x^{-1}}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 120](../../../../paper-120-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
