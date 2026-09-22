<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the lower coordinate in each direction from the smaller lower bound, and the upper coordinate from the larger upper bound. This gives an [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md), rather than the generally nonrectangular [set union](../../../../../set-union.md) of the two regions. Use [defensive copying](../../../../../defensive-copying.md) because the paper's `Point` has mutable fields.

```
final class Rect {
    private final Point lowerLeft, upperRight;

    public Rect(Point ll, Point ur) {
        if (ll == null || ur == null)
            throw new IllegalArgumentException("null corner");
        double xl = ll.getX(), yl = ll.getY();
        double xh = ur.getX(), yh = ur.getY();
        if (!Double.isFinite(xl) || !Double.isFinite(yl)
                || !Double.isFinite(xh) || !Double.isFinite(yh)
                || xl > xh || yl > yh)
            throw new IllegalArgumentException("invalid rectangle");
        lowerLeft = new Point(xl, yl);
        upperRight = new Point(xh, yh);
    }

    public Rect Union(Rect r) {
        return new Rect(
            new Point(Math.min(lowerLeft.getX(), r.lowerLeft.getX()),
                      Math.min(lowerLeft.getY(), r.lowerLeft.getY())),
            new Point(Math.max(upperRight.getX(), r.upperRight.getX()),
                      Math.max(upperRight.getY(), r.upperRight.getY())));
    }

    public Point lowerLeft() { return lowerLeft.clone(); }
    public Point upperRight() { return upperRight.clone(); }
}
```

Any containing [rectangle](../../../../../rectangle.md) must reach at least as far as each input [rectangle](../../../../../rectangle.md) in all four coordinate directions. The constructed [rectangle](../../../../../rectangle.md) reaches exactly those four limits, which proves both containment and minimality:

$$
\boxed{[\min(x_l,x'_l),\max(x_h,x'_h)]\times[\min(y_l,y'_l),\max(y_h,y'_h)].}
$$

The corner accessors return copies, so changing a constructor argument or returned `Point` cannot alter an existing `Rect`.

## ↑ Ancestors (11)

1. [A](../a.md)
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
