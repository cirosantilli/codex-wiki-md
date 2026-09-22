# Indexing within a type class

↑ **Parent:** [Type class](type-class.md)

If a [decoder](channel-decoder.md) already knows the length, [alphabet](alphabet.md) and [empirical distribution](type-information-theory.md), it only needs to distinguish $|T_n(q)|$ possible strings. A fixed-length index therefore needs $\lceil\log_2|T_n(q)|\rceil$ [bits](bit.md). List the six balanced four-symbol strings in increasing lexicographic order and number them $0$ through $5$. A three-[bit](bit.md) index identifies any one of them, whereas writing the original binary string directly takes four [bits](bit.md).

Knowing the [empirical distribution](type-information-theory.md) is essential to that calculation. If it must also be sent, a simple fixed-length description of which of the five classes was used costs another $\lceil\log_2 5\rceil=3$ [bits](bit.md). That naive balanced-string message totals six [bits](bit.md) and is longer than the raw four-[bit](bit.md) string. The example demonstrates the benefit of shared constraints, rather than a free [lossless source coding](lossless-source-coding.md) scheme for every input. For long strings over a fixed [alphabet](alphabet.md), the overhead for identifying a class grows only logarithmically with length, while the [information entropy](information-entropy.md) of its frequency profile controls the leading cost within the class.

## ↑ Ancestors (7)

1. [Type class](type-class.md)
2. [Type (information theory)](type-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
