<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Writing $\mathrm{PTime}$ as [P](../../../../../p-complexity.md) and $\mathrm{co\text{-}PTime}$ as [co-P](../../../../../co-p.md), the known relationships among the four [complexity classes](../../../../../complexity-class.md) are

$$
\boxed{\mathrm P=\mathrm{co\text{-}P},\qquad
\mathrm P\subseteq\mathrm{NP},\qquad
\mathrm P\subseteq\mathrm{co\text{-}NP}.}
$$

The equality supplies both inclusions between [P](../../../../../p-complexity.md) and [co-P](../../../../../co-p.md), and it also gives [co-P](../../../../../co-p.md) $\subseteq$ [NP](../../../../../np-complexity.md) and [co-P](../../../../../co-p.md) $\subseteq$ [co-NP](../../../../../co-np.md).

For the equality, a deterministic [polynomial-time algorithm](../../../../../polynomial-time-algorithm.md) halts on every [input](../../../../../input-computer-science.md); interchange its accepting and rejecting outcomes to decide the [complement of a set](../../../../../complement-of-a-set.md) in the same [polynomial time](../../../../../polynomial-time.md). For [P](../../../../../p-complexity.md) $\subseteq$ [NP](../../../../../np-complexity.md), a [Nondeterministic Turing machine](../../../../../nondeterministic-turing-machine.md) can simply make no choices and follow the deterministic computation. Finally, if $A\in\mathrm P$, then $\overline A\in\mathrm P\subseteq\mathrm{NP}$, whence $A\in\mathrm{co\text{-}NP}$ by the definition of [co-NP](../../../../../co-np.md).

Neither [NP](../../../../../np-complexity.md) $\subseteq$ [co-NP](../../../../../co-np.md) nor [co-NP](../../../../../co-np.md) $\subseteq$ [NP](../../../../../np-complexity.md) is known; either would imply equality by taking [complements](../../../../../complement-of-a-set.md). Nor is either inclusion of [P](../../../../../p-complexity.md) into [NP](../../../../../np-complexity.md) or [co-NP](../../../../../co-np.md) known to be strict. These unresolved relationships must not be presented as strict separations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
