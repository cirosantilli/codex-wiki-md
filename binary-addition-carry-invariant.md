# Binary-addition carry invariant

↑ **Parent:** [Binary number](binary-number.md)

After adding $k$ least-significant [binary digits](binary-digit.md), the numerical sum of the two processed input suffixes equals the written $k$ result digits plus $carry\,2^k$, with $carry\in\{0,1\}$. Initially both suffixes are empty. For the next column, write $(x_k+y_k+carry)\bmod2$ and pass $\lfloor(x_k+y_k+carry)/2\rfloor$ to the next column. Multiplying these column quantities by $2^k$ preserves the equation. After all columns, the remaining carry supplies the extra leading digit, proving correctness without converting either full input to a machine integer.

## ↑ Ancestors (6)

1. [Binary number](binary-number.md)
2. [Real number](real-number.md)
3. [Arithmetic](arithmetic-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Binary addition in logarithmic space](binary-addition-in-logarithmic-space.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/3/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/2/b/solution.md)
