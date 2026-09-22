# Adjacent-suffix characterization of longest repeats

↑ **Parent:** [Suffix array](suffix-array.md)

The length of a [longest repeated substring](longest-repeated-substring.md) equals the maximum longest-common-prefix length over adjacent suffixes in [lexicographic order](lexicographic-order.md). Suffixes beginning with a fixed [string](string.md) form a consecutive interval: a [string](string.md) outside that [string prefix](string-prefix.md) [software class](class-programming.md) differs earlier or ends sooner, putting it strictly to one side. Two occurrences of a [longest repeated substring](longest-repeated-substring.md) therefore bound an interval in which every adjacent pair shares that [string prefix](string-prefix.md). At least one adjacent pair attains its length, and no pair can exceed the global maximum. This proves the result even when occurrences overlap; a text with fewer than two suffixes needs a separate empty-result convention.

## ↑ Ancestors (4)

1. [Suffix array](suffix-array.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
