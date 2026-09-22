# Canonical equality of coloured interval rows

↑ **Parent:** [Run-length encoding](run-length-encoding.md)

Represent a row by sorted disjoint [half-open intervals](half-open-interval.md), each carrying a colour. Merge touching intervals precisely when their colours agree. The resulting ordered maximal runs form a canonical representation of occupancy and colour: equality of those runs is equivalent to pointwise equality, while ignoring arbitrary subdivisions inside one colour run. For two rows containing $m$ and $n$ intervals, constructing and comparing runs takes $O(m+n)$ [time complexity](time-complexity.md), independently of coordinate magnitude or interval lengths.

## ↑ Ancestors (4)

1. [Run-length encoding](run-length-encoding.md)
2. [Data compression](data-compression-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
