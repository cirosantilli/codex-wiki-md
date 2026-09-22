<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $A\in\mathrm{NP}$, accepted by a fixed [Nondeterministic Turing machine](../../../../../nondeterministic-turing-machine.md) $M$ in at most $p(n)$ steps on every computation branch, for a [polynomial](../../../../../polynomial-split.md) $p$. Since the transition relation is finite, there is a fixed constant $b\geq2$ bounding the number of choices at any step. Every branch can be specified by a [word over an alphabet](../../../../../string.md) of length $p(n)$ over a $b$-symbol choice [alphabet](../../../../../alphabet.md), padding unused choices after halting.

A deterministic [Turing machine](../../../../../turing-machine.md) enumerates all $b^{p(n)}$ such choice sequences and simulates the corresponding branches for at most $p(n)$ steps each. It accepts if some simulation accepts, and rejects after all have failed. Every possible accepting branch is included, and the time cutoff guarantees termination even on invalid choice sequences. A standard direct simulation has only [polynomial](../../../../../polynomial-split.md) overhead per branch, giving

$$
b^{p(n)}p(n)^{O(1)}
=2^{O(p(n)+\log(p(n)+1))}
\leq 2^{q(n)}
$$

for a suitable [polynomial](../../../../../polynomial-split.md) $q$. This is a deterministic [exponential time](../../../../../exponential-time.md) bound. Therefore

$$
\boxed{\mathrm{NP}\subseteq\mathrm{EXPTIME}.}
$$

Here [EXPTIME](../../../../../exptime.md) means the union of deterministic time bounds $2^{n^d}$ over fixed positive [integers](../../../../../integer-split.md) $d$, allowing the usual constant factors and finitely many small [inputs](../../../../../input-computer-science.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
