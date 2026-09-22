<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [Turing machines](../../../../../turing-machine.md) with a two-way read-only [input](../../../../../input-computer-science.md) tape, bounded by endmarkers, and a fixed finite number of read-write work tapes over a fixed finite [alphabet](../../../../../alphabet.md). Work-tape cells count towards [space complexity](../../../../../space-complexity.md); the read-only [input](../../../../../input-computer-science.md) does not. For [input](../../../../../input-computer-science.md) length $n$, use $O(\log(n+2))$ to include the small-length cases.

**$\mathrm{Logspace}$, or [L](../../../../../l-complexity.md), is the class of [formal languages](../../../../../formal-language.md) decided by a deterministic such machine using at most $c\log(n+2)$ work-tape cells for some fixed constant $c$.** It must halt on every [input](../../../../../input-computer-science.md) and accept exactly the members.

**$\mathrm{NLogspace}$, or [NL](../../../../../nl-complexity.md), is the class of [formal languages](../../../../../formal-language.md) accepted by a [Nondeterministic Turing machine](../../../../../nondeterministic-turing-machine.md) with the same work-space bound on every computation branch.** An [input](../../../../../input-computer-science.md) is accepted if and only if at least one branch accepts. One may require all branches to halt: the [configuration graph](../../../../../configuration-graph.md) has only a [polynomial](../../../../../polynomial-split.md) number of [vertices](../../../../../vertex-graph-theory.md), so a [logarithmic space](../../../../../logarithmic-space.md) counter can stop any branch that has taken more steps than that bound. If an accepting computation exists, one exists with no repeated [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md), so this convention does not change the [complexity class](../../../../../complexity-class.md).

In standard [space complexity](../../../../../space-complexity.md) notation,

$$
\boxed{\mathrm L=\mathrm{DSPACE}(O(\log n)),\qquad
\mathrm{NL}=\mathrm{NSPACE}(O(\log n)).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
