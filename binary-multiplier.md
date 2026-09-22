# Binary multiplier

↑ **Parent:** [Digital electronics](digital-electronics.md)

A digital circuit implementing [binary multiplication](binary-multiplication.md). A [combinational logic](combinational-logic.md) implementation forms shifted partial products with [AND gates](and-gate.md) and combines them with [adders](adder.md). A [sequential circuit](sequential-logic.md) can instead reuse one [adder](adder.md), storing a partial sum, a shifted multiplicand, and the remaining multiplier in [digital registers](digital-register.md). If those quantities are $P,M,Q$, the update $P\gets P+(Q_0?M:0)$, $M\gets2M$, $Q\gets\lfloor Q/2\rfloor$ preserves $P+MQ$. Starting with $(0,X,Y)$ and stopping when $Q=0$ therefore produces $P=XY$, provided widths prevent overflow.

## ↑ Ancestors (3)

1. [Digital electronics](digital-electronics.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Binary multiplication](binary-multiplication.md)
- [Digital register](digital-register.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/2/c/solution.md)
