<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

After every proposed [pixel](../../../../../pixel.md) has passed part (d), insist on exactly one call in every column of the closed endpoint interval:

```
void final()
{
    for (int x = x0; x <= x1; x++) {
        if (counter[x] != 1) reject();
    }
    accept();
}
```

Part (d) already rejected every out-of-range column and every incorrect ordinate. A zero counter now detects an omitted column; a counter greater than one detects a repeated call in that column. Because the residual interval in part (d) allows exactly one [integer](../../../../../integer-split.md) ordinate in each column, accepted calls in a repeated column must address the same [pixel](../../../../../pixel.md). Conversely, a counter of one in every column forces the complete set of nearest [pixels](../../../../../pixel.md), including both endpoints. Consecutive correct columns differ in ordinate by at most one, which proves that there are no gaps in the resulting thin [line segment](../../../../../line-segment.md).

The verifier certifies the final plotted set; it need not require calls to arrive in increasing $x$ order. Its final condition is simply

$$
\boxed{\operatorname{counter}[x]=1\quad\text{for every }x=x_0,\ldots,x_1.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
