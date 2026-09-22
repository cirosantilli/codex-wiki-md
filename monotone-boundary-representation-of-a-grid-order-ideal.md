# Monotone boundary representation of a grid order ideal

↑ **Parent:** [Order ideal](order-ideal.md)

For an [order ideal](order-ideal.md) in a finite rectangular grid with coordinatewise [partial order](partially-ordered-set.md), occupied cells in each row form a left prefix. Their lengths form a nonincreasing [sequence](sequence.md) $r_y$. Conversely, any nonincreasing sequence of valid row lengths specifies exactly one such [order ideal](order-ideal.md), giving an [abstraction function](abstraction-function.md) with no redundant per-cell information.

Removing all occupied cells with $x\geq a$ and $y\geq b$ replaces $r_y$ by $\min(r_y,a)$ for $y\geq b$ and leaves earlier rows unchanged. The new lengths remain nonincreasing: affected rows preserve their mutual order, and the first affected row only decreases. For a legal removal, the boundary immediately below it was already at least $a$. A cached [sum](sum.md) of row lengths can be updated by subtracting the decreases. This yields constant-time membership and count queries, linear storage, and an update linear in the number of affected rows.

## ↑ Ancestors (8)

1. [Order ideal](order-ideal.md)
2. [Partially ordered set](partially-ordered-set.md)
3. [Set](set-split.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Chomp](chomp.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/5/a/i/solution.md)
