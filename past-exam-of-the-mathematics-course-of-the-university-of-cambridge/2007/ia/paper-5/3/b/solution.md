<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace type parameters by their erasures, normally `Object` or the first declared bound, and insert checked casts where an erased result is used as its former specific type. A simple [generics in Java](../../../../../../generics-in-java.md) example becomes:
```
// Generic version
Vector<String> names = new Vector<String>();
names.add("Ada");
String s = names.get(0);

// Non-generic version
Vector names = new Vector();
names.add("Ada");
String s = (String) names.get(0);
```
The two fragments are alternatives, not consecutive declarations in one scope. For a user-defined `Box<T>`, replace fields, parameters and returns of type `T` by `Object`, and cast the retrieved result. Bounded parameters instead erase to their bound. A full translation must also preserve method dispatch where erasure changes overridden signatures, using suitable forwarding methods; this is the principle of [type erasure](../../../../../../type-erasure.md), not simply deleting every pair of angle brackets.

The raw collection permits accidental insertion of an unrelated object, which may fail much later at a cast. The generic collection rejects such insertion during compilation, documents its contract at the declaration, and eliminates repetitive casts at use sites. **The generic version catches more errors earlier and expresses the programmer's intended element type directly.** Generic types are largely erased at runtime, so their advantage is static checking rather than a new runtime vector representation. The translation mechanism is specified by the [Java language specification](https://docs.oracle.com/javase/specs/jls/se8/html/jls-4.html#jls-4.6).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
