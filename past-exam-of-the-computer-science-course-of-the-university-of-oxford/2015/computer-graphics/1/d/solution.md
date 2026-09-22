<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The verifier can check the final geometric criterion directly, independently of the incremental decision variable. Set $dx=x_1-x_0$, $dy=y_1-y_0$, and define the scaled vertical residual

$$
e=2dy(x-x_0)-2dx(y-y_0).
$$

The exact [line](../../../../../straight-line.md) ordinate is $y_* = y_0+dy(x-x_0)/dx$, so $e=2dx(y_*-y)$. Nearest-[integer](../../../../../integer-split.md) selection with upward ties is precisely

$$
\boxed{x_0\leq x\leq x_1,\qquad -dx\leq e<dx.}
$$

The strictness matters: at a half-[integer](../../../../../integer-split.md) ordinate the upper [pixel](../../../../../pixel.md) has $e=-dx$ and passes, whereas the lower [pixel](../../../../../pixel.md) has $e=dx$ and fails. Each column has exactly one accepted [integer](../../../../../integer-split.md) ordinate.

With `reject()` terminating verification unsuccessfully, suitable outline code is:

```
void checkPoint(int x, int y)
{
    Wide a = Wide(x) - x0;
    if (a < 0) reject();                    // inequality 1
    Wide b = Wide(x1) - x;
    if (b < 0) reject();                    // inequality 2

    Wide dx = Wide(x1) - x0;
    Wide dy = Wide(y1) - y0;
    Wide e = 2 * dy * a - 2 * dx * (Wide(y) - y0);
    Wide lower = e + dx;
    if (lower < 0) reject();                // inequality 3
    Wide upper = dx - e;
    if (upper <= 0) reject();               // inequality 4

    counter[x]++;
}
```

`Wide` denotes a signed [integer](../../../../../integer-split.md) type large enough for the products and differences, with conversion before subtraction. These are exactly four inequalities against zero, all applied to named [integer](../../../../../integer-split.md) variables. The arithmetic restriction on the drawing loop in part (c) does not restrict multiplication in this verifier. The screen endpoints are assumed valid, with $0\leq x_0<x_1<\texttt{MAX\_SCREEN\_WIDTH}$ and valid endpoint ordinates, so indexing is safe after the first two checks. These endpoint and screen preconditions belong in initialization if they are not guaranteed by the caller.

No separate $y$-range tests are needed: for $x$ between the endpoints, $y_*$ lies in $[y_0,y_1]$, and its nearest [integer](../../../../../integer-split.md) lies in the same interval because both bounds are [integers](../../../../../integer-split.md). The counters defer detection of omissions and repetitions to part (e). As for every finite counter, use adequate capacity or a sticky failure on overflow; saturating each counter at two also suffices because only zero, one, and “more than one” matter.

## ↑ Ancestors (11)

1. [D](../d.md)
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
