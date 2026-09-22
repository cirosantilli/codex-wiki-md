<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Construct $z$ as above, and run the equality [group multiplier automaton](../../../../../../group-multiplier-automaton.md) $M_\varepsilon$ on $z\otimes\gamma$. Both inputs belong to $L$, so

$$
M_\varepsilon\text{ accepts }z\otimes\gamma
\quad\Longleftrightarrow\quad
\overline z=\overline\gamma
\quad\Longleftrightarrow\quad
\overline w=1.
$$

The final [finite-state automaton](../../../../../../finite-state-machine.md) run takes $O(\max(|z|,|\gamma|)+1)=O(n+1)$ time. **The [word problem for a group](../../../../../../word-problem-for-groups.md) is therefore decidable in quadratic time**:

$$
\boxed{T_{\mathrm{word}}(w)=O(|w|^2)\quad(|w|\geq1).}
$$

The [empty word](../../../../../../empty-word.md) is accepted immediately. Comparing $z$ and $\gamma$ as literal strings would be incorrect, since an [automatic structure for a group](../../../../../../automatic-structure-for-a-group.md) need not give unique representatives.

## ↑ Ancestors (11)

1. [F](../f.md)
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
