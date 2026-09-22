<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Brick boundaries are not observable in the requested row equality. Two adjacent red width-one bricks must compare equal to one red width-two brick at the same left coordinate. Comparing the underlying placement [lists](../../../../../list-abstract-data-type.md) would therefore give the wrong result.

Instead build each row's unique [sequence](../../../../../sequence.md) of maximal occupied colour runs: merge adjacent placements exactly when they touch and have equal colours. Gaps remain gaps, and touching different colours remain separate runs. This is a geometric version of [run-length encoding](../../../../../run-length-encoding.md), with explicit start and end coordinates. Insert these members inside `Row` from part (d):

```
private static final class Run {
    final long x, end;
    final Color colour;

    Run(long x, long end, Color colour) {
        this.x = x;
        this.end = end;
        this.colour = colour;
    }
}

private List<Run> runs() {
    List<Run> result = new ArrayList<Run>();
    for (Placed b : bricks) {
        int last = result.size() - 1;
        if (last >= 0) {
            Run r = result.get(last);
            if (r.end == b.x && r.colour.equals(b.colour)) {
                result.set(last, new Run(r.x, b.end, r.colour));
                continue;
            }
        }
        result.add(new Run(b.x, b.end, b.colour));
    }
    return result;
}

@Override public boolean equals(Object other) {
    if (this == other) return true;
    if (!(other instanceof Row)) return false;
    List<Run> a = runs(), b = ((Row) other).runs();
    if (a.size() != b.size()) return false;
    for (int i = 0; i < a.size(); ++i) {
        Run r = a.get(i), s = b.get(i);
        if (r.x != s.x || r.end != s.end || !r.colour.equals(s.colour))
            return false;
    }
    return true;
}

@Override public int hashCode() {
    int h = 1;
    for (Run r : runs()) {
        h = 31 * h + Long.hashCode(r.x);
        h = 31 * h + Long.hashCode(r.end);
        h = 31 * h + r.colour.hashCode();
    }
    return h;
}
```

`Color.equals` compares colour values rather than [object identity](../../../../../object-identity.md). Two row snapshots compare their local horizontal content independently of which wall height supplied them. Empty rows compare equal, even if obtained from different walls. The [hash code](../../../../../hash-code.md) uses the same canonical runs as `equals`, so alternative brick subdivisions with equal displayed content also have equal [hash codes](../../../../../hash-code.md).[hashCode(), equal objects must produce equal hash codes](../../../../../java-8-object-api-documentation.md)

To prove correctness, observe that a maximal run starts whenever occupancy begins or the colour changes, and ends exactly where that occupancy or colour ceases. Those boundaries are determined by the occupied colour at every coordinate. Thus equal occupied colours give the same runs, and equal runs give equal occupied colours. If rows contain $m$ and $n$ bricks, generating and comparing their runs has $O(m+n)$ [time complexity](../../../../../time-complexity.md) and $O(m+n)$ additional storage, independent of their widths or the magnitude of their coordinates. This meets the requirement to improve on checking every possible cell:

$$
\boxed{\text{row equality}\iff\text{equal ordered maximal occupied colour runs}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
