<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Represent a wall by a [list](../../../../../list-abstract-data-type.md) of rows indexed by height. Within each row keep brick placements sorted by their left coordinate, with disjoint occupied [half-open intervals](../../../../../half-open-interval.md). The public `Brick` in the paper is a mutable input specification; internal placements snapshot its width and colour, so later client edits cannot invalidate an existing wall. Empty intermediate rows cannot occur in a supportive wall with occupied rows above them.

The following [Java](../../../../../java-programming-language.md) uses `import java.util.*;` and `import java.awt.Color;`. Keep the source's `Brick` input [software class](../../../../../class-programming.md). All other representation types are private nested [software classes](../../../../../class-programming.md) of `Wall`, which prevents clients from inserting directly into a row. The `row(int y)` query returns a detached row for the equality operation in part (e).

```
final class Wall {
    private static final class Placed {
        final long x, end;
        final Color colour;

        Placed(long x, int width, Color colour) {
            this.x = x;
            this.end = x + width;
            this.colour = colour;
        }
    }

    private static final class Row {
        private final List<Placed> bricks = new ArrayList<Placed>();

        boolean contains(long x) {
            for (Placed b : bricks) {
                if (x < b.x) return false;
                if (x < b.end) return true;
            }
            return false;
        }

        boolean canInsert(Placed b) {
            for (Placed old : bricks)
                if (b.x < old.end && old.x < b.end) return false;
            return true;
        }

        void insert(Placed b) {
            int i = 0;
            while (i < bricks.size() && bricks.get(i).x < b.x) ++i;
            bricks.add(i, b);
        }

        Row copy() {
            Row r = new Row();
            r.bricks.addAll(bricks);
            return r;
        }

        // Insert the equality members from part (e) here.
    }

    private final List<Row> rows = new ArrayList<Row>();

    public void addBrick(Brick b, int x, int y) throws Exception {
        if (b == null || b.col == null || b.width <= 0 || y < 0)
            throw new Exception("invalid brick or height");
        // Snapshot mutable input. Long arithmetic protects x + width.
        int width = b.width;
        Color colour = new Color(b.col.getRGB(), true);
        Placed placed = new Placed((long) x, width, colour);
        if (y > rows.size()) throw new Exception("unsupported height");

        Row target = y == rows.size() ? new Row() : rows.get(y);
        if (!target.canInsert(placed)) throw new Exception("overlap");
        if (y > 0) {
            Row below = rows.get(y - 1);
            if (!below.contains(placed.x) || !below.contains(placed.end - 1))
                throw new Exception("unsupported end");
        }
        // All checks precede the first modification of this wall.
        target.insert(placed);
        if (y == rows.size()) rows.add(target);
    }

    public boolean contains(int x, int y) {
        return y >= 0 && y < rows.size() && rows.get(y).contains((long) x);
    }

    public Object row(int y) {
        if (y < 0) throw new IllegalArgumentException("negative row");
        return y < rows.size() ? rows.get(y).copy() : new Row();
    }
}
```

Here `Placed` instances and their captured `Color` values are [immutable objects](../../../../../immutable-object.md), so copying a row's outer [list](../../../../../list-abstract-data-type.md) suffices to create a detached snapshot. Returning its static type as `Object` exposes just the equality operation needed below, without exposing a mutable row [API](../../../../../application-programming-interface.md). A fuller application could instead return an immutable row-view [object interface](../../../../../object-interface.md).

The empty [list](../../../../../list-abstract-data-type.md) represents a valid supportive wall. A rejected insertion performs no wall update. On success, the overlap test establishes validity in the target row; all other rows are unchanged. The support checks establish support for the new brick; adding material cannot remove support from old bricks. Appending a row only at the current height count keeps the row representation contiguous. [Integer overflow](../../../../../integer-overflow.md) in a right endpoint is prevented by converting the horizontal coordinate to `long` before adding the positive `int` width. For instance, a brick at `Integer.MAX_VALUE` can still have a mathematically meaningful right endpoint.

The resulting [representation invariant](../../../../../representation-invariant.md) is

$$
\boxed{\text{ordered disjoint placements within rows, with every elevated brick supported at both ends}.}
$$

This is a sequential [API](../../../../../application-programming-interface.md); concurrent mutation of an input `Brick` during the call is outside its contract. Coordinate magnitude does not determine the storage used: storage is proportional to the number of placements and occupied rows.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
