<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Three advantages of [integer arithmetic](../../../../../integer-arithmetic.md) for [raster graphics](../../../../../raster-graphics.md) are:

- **Cheap, fast operations.** Historically, [integer](../../../../../integer-split.md) addition, subtraction and shifts needed much less hardware and execution time than [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), especially on machines without a [floating-point unit](../../../../../floating-point-unit.md). An incremental [Bresenham's line algorithm](../../../../../bresenham-s-line-algorithm.md) needs only a few additions and a decision per [pixel](../../../../../pixel.md).
- **Exact decisions.** Provided [integer overflow](../../../../../integer-overflow.md) is excluded, the scaled [midpoint line decision](../../../../../midpoint-line-decision.md) is exact. There is no accumulated [rounding error](../../../../../round-off-error.md) that can move a decision across a half-[pixel](../../../../../pixel.md) boundary; equality has a reproducible tie rule.
- **Simple storage and hardware.** [Integer](../../../../../integer-split.md) coordinates already identify [pixels](../../../../../pixel.md). An implementation can keep coordinates and decision variables in ordinary registers and use a small add/compare datapath, avoiding conversion between [floating-point numbers](../../../../../floating-point-number.md) and [integer](../../../../../integer-split.md) screen addresses.

These are historical and structural advantages, not a claim that every modern processor executes every [integer](../../../../../integer-split.md) operation faster. An [integer](../../../../../integer-split.md) implementation still needs sufficient width for its intermediate results. The compact answer is

$$
\boxed{\text{fast elementary operations; exact decisions; simple hardware and storage}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
