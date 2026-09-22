<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a `Spreadsheet` class owning a private rectangular [Java array](../../../../../../../java-array.md) of cells. Each immutable internal `Cell` contains a private tag `Kind` with values `EMPTY`, `LABEL`, `NUMBER`, `FORMULA`, and the corresponding payload: a string, a double or a formula reference. The tag determines which payload is meaningful, and the spreadsheet's setters create valid combinations rather than letting callers change fields independently. The cell object need not be public; public methods can expose its kind and label when needed for display.

Provide public `setEmpty(r,c)`, `setLabel(r,c,text)`, `setNumber(r,c,x)` and `setFormula(r,c,f)` methods, each checking its target coordinates and invalidating cached results. A public `valueAt(r,c)` supplies the numerical value, treating out-of-grid, empty and label cells as zero, and a public `recalculate()` brings all valid formulas up to date. Keep cached numeric results and evaluation-state flags private; they are derived data rather than editable cell content.

Define a public `Formula` interface with `double evaluate(Lookup values, int row, int column)`. `Lookup` supplies only `valueAt(r,c)`, so a formula can read dependencies without needing direct access to cells or a mutation API. An immutable `AddFormula` stores four integer offsets, two row/column pairs. It evaluates the two coordinates relative to the formula's own position and returns their sum. New formula kinds implement the same interface, avoiding changes to the storage representation or a large central switch over all formula operations.

The private [spreadsheet dependency evaluation](../../../../../../../spreadsheet-dependency-evaluation.md) mechanism provides the `Lookup` implementation, checks cycles and caches evaluated cells. Formula evaluation is required to be side-effect-free with fixed dependencies during a recalculation. This separates [encapsulation in object-oriented programming](../../../../../../../encapsulation-in-object-oriented-programming.md) from extension: callers can change a cell through public setters and add new formula implementations, while internal cell invariants and cached values remain protected. **Use tagged cell contents, an extensible formula interface and spreadsheet-owned evaluation state.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
