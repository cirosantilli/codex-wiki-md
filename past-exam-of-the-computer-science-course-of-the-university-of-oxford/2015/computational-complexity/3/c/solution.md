<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let a deterministic [Turing machine](../../../../../turing-machine.md) $M$ decide $A$ with at most $s(n)=c\log(n+2)$ work-tape cells. Fix an [input](../../../../../input-computer-science.md) $x$ of length $n$. A [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md) is determined by the control state, the read-only [input](../../../../../input-computer-science.md)-head position, the work-tape contents, and the work-head positions. For one work tape with [alphabet](../../../../../alphabet.md) $\Gamma$, their number is bounded, up to harmless fixed factors, by

$$
|Q|(n+2)(s(n)+1)|\Gamma|^{s(n)}.
$$

The factors respectively count the state, [input](../../../../../input-computer-science.md)-head position, work-head position and work-tape contents. With a fixed number $r$ of work tapes, replace the last two factors by $(s(n)+1)^r|\Gamma|^{rs(n)}$ if each tape is allowed $s(n)$ cells; this still gives a valid [polynomial](../../../../../polynomial-split.md) upper bound. Two-way work tapes only change fixed factors in the head-position bounds.

Since

$$
|\Gamma|^{c\log_2(n+2)}
=(n+2)^{c\log_2|\Gamma|},
$$

there are at most $(n+2)^d$ [Turing machine configurations](../../../../../instantaneous-description-of-a-turing-machine.md) for some constant $d$ depending on $M$. If a deterministic computation repeats one of its [Turing machine configurations](../../../../../instantaneous-description-of-a-turing-machine.md) on the fixed [input](../../../../../input-computer-science.md), all subsequent steps repeat too, so it never halts. But $M$ is a decider. It therefore halts before any repetition and takes at most a [polynomial](../../../../../polynomial-split.md) number of steps. The same [Turing machine](../../../../../turing-machine.md) is consequently a [polynomial-time algorithm](../../../../../polynomial-time-algorithm.md), establishing

$$
\boxed{\mathrm{Logspace}\subseteq\mathrm{PTime}.}
$$

It would be incorrect to count just the work-tape contents and omit the read-only [input](../../../../../input-computer-science.md)-head position; that position is part of the [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md) even though the [input](../../../../../input-computer-science.md) itself is not charged as work space.

## ↑ Ancestors (11)

1. [C](../c.md)
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
