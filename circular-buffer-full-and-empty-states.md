# Circular buffer full and empty states

↑ **Parent:** [Circular buffer](circular-buffer.md)

With front-plus-count storage, empty means $n=0$ and full means $n=C$; every allocated slot is usable. With only the two wrapped [array indices](array-index.md) $h,w$, the equality $h=w$ describes both possibilities. Indeed $w-h\equiv n\pmod C$, and the two allowed counts $0,C$ have the same remainder. Recovering the count as $(w-h)\bmod C$ therefore loses the full state. A count, a separate full flag, or a different index representation must resolve that ambiguity.

Another convention reserves one slot: for a physical [array](array-data-structure.md) of length $C\geq2$, empty means $w=h$ and full means $(w+1)\bmod C=h$. Its usable capacity is $C-1$, and $(w-h)\bmod C$ now recovers its count because $0\leq n<C$. A five-slot [array](array-data-structure.md) then stores at most four items.

This is the convention of the kernel's documented `CIRC_*` helpers, which additionally require power-of-two [array](array-data-structure.md) lengths. It is not a universal property of [circular buffers](circular-buffer.md); our capacity-five count-based example uses all five slots and does not use those helpers.[David Howells and Paul E. McKenney, Circular Buffers, What is a circular buffer?; Measuring power-of-2 buffers: full/empty convention and helper result range](circular-buffers-by-david-howells-and-paul-e-mckenney.md)

The smallest count-based case, $C=1$, makes the issue vivid: both $h$ and $w$ are always zero, but $n$ still distinguishes one live item from none. Capacity zero is excluded from our formulas because remainder modulo zero is undefined.

## ↑ Ancestors (4)

1. [Circular buffer](circular-buffer.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
