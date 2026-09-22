# Output sets of different-length linear-feedback registers

↑ **Parent:** [Linear-feedback shift register](linear-feedback-shift-register.md)

Under the convention that a register emits each shifted-out symbol, its first $d$ output symbols are exactly its initial fill. Thus a binary register of length $d$ has $2^d-1$ distinct outputs from nonzero fills. For lengths $r<s$, at least one longer-register output is absent from the shorter register, guaranteeing a pair of unequal nonzero outputs. The two sets need not be disjoint: recurrences $s_{n+1}=s_n$ and $s_{n+2}=s_n$ both generate constant ones. Nor must they intersect: the length-one recurrence and $s_{n+2}=s_{n+1}+s_n$ have no common nonzero output, since constant ones fail the second recurrence.

## ↑ Ancestors (6)

1. [Linear-feedback shift register](linear-feedback-shift-register.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/4h/iii/solution.md)
