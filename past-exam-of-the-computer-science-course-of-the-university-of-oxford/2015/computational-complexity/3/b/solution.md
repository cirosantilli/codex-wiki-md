<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [logspace transducer](../../../../../logspace-transducer.md) is a deterministic [Turing machine](../../../../../turing-machine.md) with a read-only [input](../../../../../input-computer-science.md) tape, $O(\log(n+2))$ read-write work space, and a write-only output tape. It emits symbols successively and cannot reread the output; that output is not charged as working memory. For a total function it must halt on every [input](../../../../../input-computer-science.md). A [logspace-computable function](../../../../../logspace-computable-function.md) $f$ is a total [function](../../../../../function-split.md) whose output $f(x)$ is produced by such a [logspace transducer](../../../../../logspace-transducer.md) on [input](../../../../../input-computer-science.md) $x$.

A [logspace many-one reduction](../../../../../logspace-many-one-reduction.md) $A\leq_m^{\log}B$ is a [logspace-computable function](../../../../../logspace-computable-function.md) $f$ such that

$$
\boxed{x\in A\quad\Longleftrightarrow\quad f(x)\in B}
$$

for every [string](../../../../../string.md) $x$. The [logarithmic space](../../../../../logarithmic-space.md) bound permits a [polynomial](../../../../../polynomial-split.md)-length output, even when that output does not fit in work space. Indeed, a halting [logspace transducer](../../../../../logspace-transducer.md) cannot repeat its state, [input](../../../../../input-computer-science.md)-head position and work-tape contents and head positions: the unreadable output cannot affect its subsequent behaviour. There are only a [polynomial](../../../../../polynomial-split.md) number of such internal [Turing machine configurations](../../../../../instantaneous-description-of-a-turing-machine.md), hence a [polynomial](../../../../../polynomial-split.md) bound on the number of steps and output symbols.

To prove a [formal language](../../../../../formal-language.md) $B$ is [NL-complete](../../../../../nl-complete.md), first give an [NL](../../../../../nl-complexity.md) acceptance procedure for $B$. Then show every $A\in\mathrm{NL}$ has a [logspace many-one reduction](../../../../../logspace-many-one-reduction.md) to $B$. Alternatively, reduce one already [NL-complete](../../../../../nl-complete.md) [formal language](../../../../../formal-language.md) to $B$, using transitivity of [logspace many-one reductions](../../../../../logspace-many-one-reduction.md).

Transitivity requires [logspace composition by recomputation](../../../../../logspace-composition-by-recomputation.md), rather than storing the intermediate output. To compose $g$ with $f$, simulate the [logspace transducer](../../../../../logspace-transducer.md) for $g$ with a virtual [input](../../../../../input-computer-science.md) $f(x)$. Retain its virtual [input](../../../../../input-computer-science.md)-head position in $O(\log n)$ [bits](../../../../../bit.md). Whenever it asks for a symbol, rerun the [logspace transducer](../../../../../logspace-transducer.md) for $f$ from the beginning and count its output symbols until that position is reached. Since $|f(x)|$ is [polynomial](../../../../../polynomial-split.md) in $n$, the simulated work space $O(\log|f(x)|)$ and all output-position counters are $O(\log n)$. Repeated runs reuse their storage. This proves closure under composition and explains why the hardness argument works.

## ↑ Ancestors (11)

1. [B](../b.md)
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
