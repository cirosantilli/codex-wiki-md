# Carry normalization of a digit array

↑ **Parent:** [Digit-array integer representation](digit-array-integer-representation.md)

Process a [digit-array integer representation](digit-array-integer-representation.md) from low to high positions. The [integer division](integer-division.md) supplies $q=\lfloor a_i/b\rfloor$ and $0\leq r<b$. Replacing the current digit by $r$ and adding $q$ to the next position preserves the represented value. Append zero storage when a positive carry leaves the allocated array. The processed prefix remains normalized and the value stays fixed.

This also works with signed temporary digits when the represented value is nonnegative. A negative carry cannot leave the final allocated position: the normalized lower digits represent a value less than that position's next radix power, which could not offset that negative carry. Positive carries eventually stop beyond the value's finite radix expansion. Thus the usual nonnegative-digit algorithm admits this useful extension without interpreting truncated division as floor division.

## ↑ Ancestors (7)

1. [Digit-array integer representation](digit-array-integer-representation.md)
2. [Arbitrary-precision arithmetic](arbitrary-precision-arithmetic.md)
3. [Integer arithmetic](integer-arithmetic.md)
4. [Arithmetic](arithmetic-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/e/solution.md)
