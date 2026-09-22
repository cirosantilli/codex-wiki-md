# Signed power-of-two division by biasing

↑ **Parent:** [Integer division](integer-division.md)

For signed [two's complement](two-s-complement.md) [integers](integer-split.md), a conditional positive bias converts the rounding behaviour of an [arithmetic right shift](arithmetic-right-shift.md) into [C integer division](c-integer-division.md). It can be formed without a conditional branch by turning the sign [bit](bit.md) into either zero or a low-$k$-[bit](bit.md) [bit mask](bit-mask.md).

**Proof.** Nonnegative $a$ needs no adjustment. If $a<0$, write $-a=2^kq+r$, $0\leq r<2^k$. Then $a+(2^k-1)=-2^kq+(2^k-1-r)$, whose quotient rounded down is $-q$, exactly the quotient truncated towards zero. The bias fits safely for $1\leq k<n$ in an $n$-[bit](bit.md) signed word: it is added only to negative inputs, and the largest possible adjusted input is $2^k-2$. The corresponding remainder is $((a+b)\bmod2^k)-b$, where $b=(2^k-1)\mathbf1_{a<0}$.

## ↑ Ancestors (6)

1. [Integer division](integer-division.md)
2. [Division (mathematics)](division-mathematics.md)
3. [Arithmetic](arithmetic-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [C11 committee draft N1570](c11-committee-draft-n1570.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/1/e/solution.md)
