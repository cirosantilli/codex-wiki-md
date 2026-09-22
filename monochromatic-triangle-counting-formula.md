# Monochromatic-triangle counting formula

↑ **Parent:** [Diagonal Ramsey number](diagonal-ramsey-number.md)

In a red-blue [edge colouring](edge-coloring.md) of $K_n$, let $d_v$ be the red degree of vertex $v$ and let $M$ be the number of [monochromatic](monochromatic-set.md) triangles. Every nonmonochromatic triangle has exactly two vertices at which its two incident edges have different colors, so

$$
M=\binom n3-\frac12\sum_v d_v(n-1-d_v).
$$

Since $d_v(n-1-d_v)\leq\lfloor(n-1)^2/4\rfloor$, this identity gives a lower bound for $M$.

## ↑ Ancestors (7)

1. [Diagonal Ramsey number](diagonal-ramsey-number.md)
2. [Ramsey theorem](ramsey-theorem.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/17i/solution.md)
