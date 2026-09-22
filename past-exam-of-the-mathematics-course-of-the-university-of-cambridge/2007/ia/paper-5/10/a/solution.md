<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent the two constructors of the type grammar by subclasses of `MLType`: a `TypeVar` node and an `Arrow` node containing two types. Use immutable fields so a completed type expression cannot acquire cycles through later mutation. The static factory allocates a fresh object and gives it a fresh identifier shared across the whole hierarchy:
```
import java.math.BigInteger;

public abstract class MLType {
    private MLType() { }
    private static BigInteger next = BigInteger.ONE;

    public static synchronized TypeVar createNewTypeVar() {
        TypeVar answer = new TypeVar(next);
        next = next.add(BigInteger.ONE);
        return answer;
    }
    public static final class TypeVar extends MLType {
        private final BigInteger id;
        private TypeVar(BigInteger id) { this.id = id; }
    }
    public static final class Arrow extends MLType {
        private final MLType from, to;
        public Arrow(MLType from, MLType to) {
            if (from == null || to == null)
                throw new IllegalArgumentException();
            this.from = from; this.to = to;
        }
    }
}
```
The nested classes are public for use by clients, while their fields are private; `TypeVar` can be created only through the factory. Client code uses `MLType.TypeVar` and `MLType.Arrow`. A [type variable](../../../../../../type-variable.md) is identified by its unique node, and a [function type](../../../../../../function-type.md) by its domain and codomain nodes; repeated occurrences of one logical variable share the same `TypeVar` object.

The monotonically increasing `BigInteger` identifier avoids fixed-width counter overflow, and synchronization prevents two simultaneous calls from receiving the same identifier. Actual allocation remains subject to available memory. This is an [abstract syntax tree](../../../../../../abstract-syntax-tree.md) representation, possibly sharing subexpressions. **Fresh variable nodes and recursive arrow nodes represent every type in the given grammar.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
