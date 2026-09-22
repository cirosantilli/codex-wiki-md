<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply [structural recursion](../../../../../../structural-recursion.md) to the original meal, preserving its internal constructors and replacing each leaf:
```
fun gluttony (Snack _) replacement = replacement
  | gluttony (Lunch (a, b)) replacement =
      Lunch (gluttony a replacement, gluttony b replacement)
  | gluttony (Feast (a, b, c)) replacement =
      Feast (gluttony a replacement, gluttony b replacement,
             gluttony c replacement);
```
The type is `'a meal -> 'b meal -> 'b meal`: original snack labels are discarded, so the replacement can have a different label type. The constructors introduced by the replacement are not recursively processed; only snacks of the original tree are substituted. The immutable replacement can be shared among occurrences without changing the represented value. **Every original `Snack` is replaced, while the original internal meal structure is retained.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
