<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Keep storage private. Find the first entry whose horizontal coordinate is not smaller than the new one. Equality there means that the coordinate is already present; otherwise insertion at that position preserves strict ordering. Reject nonfinite coordinates, since a `NaN` would make the required comparisons meaningless. This is an explicit finite-coordinate contract for a display application.[isFinite(double)](../../../../../java-8-double-api-documentation.md)

The [Observer pattern](../../../../../observer-pattern.md) uses a small callback [Java interface](../../../../../java-interface.md). With `import java.util.*;`, the full implementation is:

```
interface GraphObserver {
    void changed(DataList source);
}

final class DataList implements Iterable<Point> {
    private final List<Point> points;
    private final List<GraphObserver> observers;

    public DataList() {
        points = new ArrayList<Point>();
        observers = new ArrayList<GraphObserver>();
    }

    public void addObserver(GraphObserver observer) {
        if (observer == null)
            throw new IllegalArgumentException("null observer");
        for (GraphObserver old : observers)
            if (old == observer) return;
        observers.add(observer);
    }

    public void removeObserver(GraphObserver observer) {
        for (int i = 0; i < observers.size(); ++i) {
            if (observers.get(i) == observer) {
                observers.remove(i);
                return;
            }
        }
    }

    public void addPoint(double x, double y) throws Exception {
        if (!Double.isFinite(x) || !Double.isFinite(y))
            throw new Exception("nonfinite coordinate");
        int i = 0;
        while (i < points.size() && points.get(i).getX() < x) ++i;
        if (i < points.size() && points.get(i).getX() == x)
            throw new Exception("duplicate x coordinate");
        points.add(i, new Point(x, y));
        List<GraphObserver> current =
            new ArrayList<GraphObserver>(observers);
        for (GraphObserver observer : current) observer.changed(this);
    }

    public Iterator<Point> iterator() {
        List<Point> snapshot = new ArrayList<Point>(points.size());
        for (Point p : points) snapshot.add(p.clone());
        return Collections.unmodifiableList(snapshot).iterator();
    }
}
```

This is a sequential implementation. Callback [object methods](../../../../../object-method.md) are required to return normally and not reenter `addPoint`; they may change their registrations. Copying the registration [list](../../../../../list-abstract-data-type.md) means such changes affect future notifications, while each observer present at the start of this notification gets exactly one call. Repeated registration of the same observer is ignored by [object identity](../../../../../object-identity.md). Both signed zeros compare equal and therefore count as the same horizontal coordinate.

For correctness, all old entries before position `i` have smaller horizontal coordinates. If an entry at `i` exists after the duplicate check, it has a strictly larger coordinate. Inserting between these two groups preserves the [representation invariant](../../../../../representation-invariant.md); rejecting a duplicate has no state effect. No client receives a stored mutable `Point`. Thus

$$
\boxed{\text{sorted, duplicate-free insertion first; observer notification second}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
