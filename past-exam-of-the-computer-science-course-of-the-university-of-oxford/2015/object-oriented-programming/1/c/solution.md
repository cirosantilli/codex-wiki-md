<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use an [abstract class](../../../../../abstract-class.md) to share the unchangeable alignment flag and the rule that the reported length equals the rendered text's length. This small [class inheritance](../../../../../class-inheritance.md) hierarchy will also serve the numeric [software classes](../../../../../class-programming.md) in part (d). The [Java interface](../../../../../java-interface.md) explicitly declares `toString()` so that the display contract is visible even though all [Java](../../../../../java-programming-language.md) [software objects](../../../../../software-object.md) already inherit that [object method](../../../../../object-method.md).

```
interface Data {
    boolean leftJustified();
    int length();
    String toString();
}

abstract class AbstractData implements Data {
    private final boolean leftj;

    protected AbstractData(boolean leftj) { this.leftj = leftj; }

    public final boolean leftJustified() { return leftj; }
    public final int length() { return toString().length(); }
    public abstract String toString();
}

final class StringData extends AbstractData {
    private final String text;

    public StringData(String s, boolean leftj) {
        super(leftj);
        if (s == null) throw new IllegalArgumentException("null text");
        text = s;
    }

    public String toString() { return text; }
}
```

There are no setters, and the stored [String data type](../../../../../string-data-type.md) value is an [immutable object](../../../../../immutable-object.md), so `StringData` is itself an [immutable object](../../../../../immutable-object.md). Its [object constructor](../../../../../object-constructor.md) rejects a [null reference](../../../../../null-reference.md) instead of deferring failure until display. Consequently,

$$
\boxed{\texttt{length()}=\texttt{toString().length()},\qquad\text{alignment is fixed at construction}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
