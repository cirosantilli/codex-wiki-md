<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Retain `Data`, `AbstractData` and `StringData` from part (c). The following are the additional [software classes](../../../../../../class-programming.md). `Formatting` denotes the supplied formatting facility with its two static `format` overloads; its implementation is expressly not required. These calls preserve the distinction between a minimum width and a maximum width: no stored value is truncated.

```
abstract class NumericData extends AbstractData {
    private int minDigits = 0;

    protected NumericData(boolean leftj) { super(leftj); }

    public final void setDigits(int n) { minDigits = Math.max(0, n); }
    protected final int digits() { return minDigits; }
}

final class IntegerData extends NumericData {
    private final int value;

    public IntegerData(int n, boolean leftj) {
        super(leftj);
        value = n;
    }

    public String toString() {
        return Formatting.format(value, digits());
    }
}

final class RealData extends NumericData {
    private final double value;
    private int minPlaces = 0;

    public RealData(double d, boolean leftj) {
        super(leftj);
        value = d;
    }

    public void setPlaces(int p) { minPlaces = Math.max(0, p); }

    public String toString() {
        return Formatting.format(value, digits(), minPlaces);
    }
}
```

Zero is the default minimum, and a nonpositive setting removes that minimum. Formatting a negative value, or a value already longer than the minimum, is delegated to the stated formatter contract. The inherited `length()` calls the current `toString()`, so a change to either formatting setting immediately changes the measured column width. For example, after `setDigits(3)`, an `IntegerData` containing 42 renders `042` and has length 3; after `setPlaces(2)`, a `RealData` containing 2.7 renders `2.70` and has length at least 4.

Unlike `StringData`, these numeric [software objects](../../../../../../software-object.md) are mutable because their displayed state can change. Their numeric values and alignment remain fixed. The useful invariant is

$$
\boxed{\text{the current formatting settings determine both text and its reported length}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Object oriented programming](../../../../object-oriented-programming-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
