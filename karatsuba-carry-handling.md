# Karatsuba carry handling

↑ **Parent:** [Karatsuba multiplication](karatsuba-multiplication.md)

The blocks in the [Karatsuba three-product identity](karatsuba-three-product-identity.md) are [integers](integer-split.md), not single digits: $p_0$ can need $2m$ positions and $h$ can exceed $q-1$. Concatenating the displayed blocks therefore fails. Accumulate their shifted values with ordinary [addition](addition.md), normalizing each digit position by [Euclidean division](euclidean-division.md): a coefficient $v$ becomes the digit $v\bmod B$, with carry $\lfloor v/B\rfloor$ passed to the next position. [Subtraction](subtraction.md) likewise propagates borrows. Although $h\geq0$ for these nonnegative [integers](integer-split.md), intermediate digitwise [subtraction](subtraction.md) can still borrow.

In the four-digit [Karatsuba worked multiplication](karatsuba-worked-multiplication.md), grouping by base $q=100$ gives unnormalized coefficients $[672,2840,2652]$, written from high to low. Normalize from the right: $2652=26\cdot100+52$; $2840+26=2866=28\cdot100+66$; $672+28=700=7\cdot100+0$. The final groups are $[7,00,66,52]$, yielding $7{,}006{,}652$. The zero group must retain its two positions.

Since $a,b,c,d<B^m$, their sums are less than $2B^m\leq B^{m+1}$ and can need $m+1$ digits. Allocate that extra digit before the third recursive product; discarding it can change the answer. The GMP manual describes this sum growth and uses a difference-based form to avoid it.[GNU MP 6.3.0 manual, §15.1.2 Karatsuba Multiplication: sum-based middle product can exceed k limbs; absolute differences and their signs](gnu-mp-6-3-0-manual/karatsuba-multiplication.md)

## ↑ Ancestors (4)

1. [Karatsuba multiplication](karatsuba-multiplication.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Divide-and-conquer product ledger](divide-and-conquer-product-ledger.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Karatsuba three-product identity](karatsuba-three-product-identity.md)
