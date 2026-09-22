<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For each sample, include both its marker and its bar. A bar's lower vertical limit is $\min(0,y_i)$, including negative bars below the horizontal axis. Its horizontal half-width is $w_i/2$, rather than $w_i$. Its marker extends by $C$ in both directions. Therefore that sample's [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md) is

$$
\left[x_i-\max(C,w_i/2),x_i+\max(C,w_i/2)\right]
\times
\left[\min(0,y_i-C),\max(0,y_i+C)\right].
$$

Taking successive bounding unions includes every sample. Finally unite with $[-M,M]\times[-M,M]$ to include the stipulated axes. The printed upper-corner formula has one extra closing parenthesis; both the lower-corner formula and the picture confirm the coordinatewise interpretation used here.[p. 5, Question 2(f), axes formula and Figure 2](../../../../../object-oriented-programming-examination-paper-of-the-university-of-oxford-2015.md)

The following commented [Java](../../../../../java-programming-language.md) [object method](../../../../../object-method.md) may be placed in a graph-view utility [software class](../../../../../class-programming.md). It uses `Rect` from part (a) and one [iterator snapshot](../../../../../iterator-snapshot.md) from part (e).

```
static Rect barBounds(DataList data, double C, double M) {
    if (!Double.isFinite(C) || !Double.isFinite(M) || C <= 0 || M <= 0)
        throw new IllegalArgumentException("positive finite margins required");
    List<Point> p = new ArrayList<Point>();
    for (Point point : data) p.add(point);
    int n = p.size();
    if (n < 2) throw new IllegalArgumentException("at least two points required");

    // This central square supplies the required minimum axis extents.
    Rect bounds = new Rect(new Point(-M, -M), new Point(M, M));
    for (int i = 0; i < n; ++i) {
        double x = p.get(i).getX(), y = p.get(i).getY();
        double width;
        if (i == 0) {
            width = p.get(1).getX() - x;
        } else if (i == n - 1) {
            width = x - p.get(i - 1).getX();
        } else {
            width = Math.min(x - p.get(i - 1).getX(),
                             p.get(i + 1).getX() - x);
        }
        // Include whichever is wider: marker or half of the bar.
        double half = Math.max(C, width / 2.0);
        // The bar reaches the baseline; the marker reaches y +/- C.
        Rect item = new Rect(new Point(x - half, Math.min(0.0, y - C)),
                             new Point(x + half, Math.max(0.0, y + C)));
        bounds = bounds.Union(item);
    }
    return bounds;
}
```

This uses the usual assumption that coordinate differences and expanded bounds are representable as finite `double` values. `Rect` rejects overflowed bounds; numerical range extension is not part of the requested geometry. As with all [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), the calculation approximates the corresponding exact [real number](../../../../../real-number.md) formulas.

Every side produced by the coordinatewise extrema is required by some bar, marker enclosure or axis extent. The result is therefore the smallest guaranteed [rectangle](../../../../../rectangle.md) for the specified marker enclosures and axes. If $X_l,Y_l,X_h,Y_h$ denote the graph-only bounds, the final answer is

$$
\boxed{[\min(-M,X_l),\max(M,X_h)]\times[\min(-M,Y_l),\max(M,Y_h)].}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
