# Hard-core predicate

↑ **Parent:** [Cryptography](cryptography.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hard-core_predicate)

A [hard-core predicate](hard-core-predicate.md) is an efficiently computable bit of an input to a [one-way function](one-way-function.md) that cannot be predicted from the function output with nonnegligible advantage over random guessing. For a [one-way function](one-way-function.md) $f$, padding it to $F(x,r)=(f(x),r)$ gives the inner-product predicate $h(x,r)=\sum_jx_jr_j\bmod2$. This is the Goldreich–Levin construction. It provides a way to mask a bit using an otherwise publicly revealed [one-way function](one-way-function.md) value.

## ↑ Ancestors (3)

1. [Cryptography](cryptography.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bit commitment](bit-commitment.md)
- [Hard-core predicate](hard-core-predicate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/12g/solution.md)
