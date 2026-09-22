<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use recursive dependency evaluation with [memoization](../../../../../../../memoization.md). After an edit, invalidate all cell states. To evaluate one formula, recursively obtain its dependencies before storing its own result. This is a [depth-first search](../../../../../../../depth-first-search.md) of the dependency graph; a visiting mark identifies a cycle, and a done mark avoids repeated evaluation of a shared dependency. The following single class implements the design, with public nested interfaces for formula extensions:
```
public final class Spreadsheet {
    public enum Kind { EMPTY, LABEL, NUMBER, FORMULA }

    public interface Lookup {
        double valueAt(int row, int col);
    }
    public interface Formula {
        double evaluate(Lookup values, int row, int col);
    }
    public static final class AddFormula implements Formula {
        private final int dr1, dc1, dr2, dc2;
        public AddFormula(int dr1, int dc1, int dr2, int dc2) {
            this.dr1 = dr1; this.dc1 = dc1;
            this.dr2 = dr2; this.dc2 = dc2;
        }
        public double evaluate(Lookup values, int r, int c) {
            return values.valueAt(r + dr1, c + dc1)
                 + values.valueAt(r + dr2, c + dc2);
        }
    }
    private static final class Cell {
        private final Kind kind;
        private final String label;
        private final double number;
        private final Formula formula;
        private Cell(Kind k, String s, double n, Formula f) {
            kind = k; label = s; number = n; formula = f;
        }
    }
    private static final Cell EMPTY =
        new Cell(Kind.EMPTY, null, 0.0, null);
    private final int rows, cols;
    private final Cell[][] cells;
    private final double[][] cache;
    private final byte[][] state;
    private final Lookup view = new Lookup() {
        public double valueAt(int r, int c) {
            return Spreadsheet.this.valueAt(r, c);
        }
    };

    public Spreadsheet(int rows, int cols) {
        if (rows < 0 || cols < 0) throw new IllegalArgumentException();
        this.rows = rows; this.cols = cols;
        cells = new Cell[rows][cols];
        cache = new double[rows][cols];
        state = new byte[rows][cols];
        for (int r = 0; r < rows; r++)
            for (int c = 0; c < cols; c++) cells[r][c] = EMPTY;
    }
    private boolean inside(int r, int c) {
        return r >= 0 && r < rows && c >= 0 && c < cols;
    }
    private void check(int r, int c) {
        if (!inside(r, c)) throw new IndexOutOfBoundsException();
    }
    private void invalidate() {
        for (int r = 0; r < rows; r++)
            for (int c = 0; c < cols; c++) state[r][c] = 0;
    }
    private void put(int r, int c, Cell cell) {
        check(r, c); cells[r][c] = cell; invalidate();
    }
    public void setEmpty(int r, int c) { put(r, c, EMPTY); }
    public void setLabel(int r, int c, String text) {
        if (text == null) throw new IllegalArgumentException();
        put(r, c, new Cell(Kind.LABEL, text, 0.0, null));
    }
    public void setNumber(int r, int c, double x) {
        put(r, c, new Cell(Kind.NUMBER, null, x, null));
    }
    public void setFormula(int r, int c, Formula f) {
        if (f == null) throw new IllegalArgumentException();
        put(r, c, new Cell(Kind.FORMULA, null, 0.0, f));
    }
    public Kind kindAt(int r, int c) {
        check(r, c); return cells[r][c].kind;
    }
    public String labelAt(int r, int c) {
        check(r, c); return cells[r][c].label;
    }
    public double valueAt(int r, int c) {
        if (!inside(r, c)) return 0.0;
        if (state[r][c] == 2) return cache[r][c];
        if (state[r][c] == 1)
            throw new IllegalStateException("Cyclic formula dependency");
        state[r][c] = 1;
        try {
            Cell cell = cells[r][c];
            double answer;
            switch (cell.kind) {
            case NUMBER: answer = cell.number; break;
            case FORMULA: answer = cell.formula.evaluate(view, r, c); break;
            default: answer = 0.0;
            }
            cache[r][c] = answer;
            state[r][c] = 2;
            return answer;
        } catch (RuntimeException error) {
            state[r][c] = 0;
            throw error;
        }
    }
    public void recalculate() {
        invalidate();
        for (int r = 0; r < rows; r++)
            for (int c = 0; c < cols; c++) valueAt(r, c);
    }
}
```
The outer loop's order need not be a [topological ordering](../../../../../../../topological-ordering.md), since recursion evaluates dependencies first. After an edit, callers can invoke `recalculate`; ordinary `valueAt` calls also calculate lazily from the invalidated state. Empty and label cells contribute zero without destroying their display content. Relative references are interpreted at the formula's location, and off-grid references contribute zero as required.

For an acyclic graph, [mathematical induction](../../../../../../../mathematical-induction.md) over a [topological ordering](../../../../../../../topological-ordering.md) proves that each cached value equals the evaluation of current cell contents. Each cell becomes done at most once in a pass, so the [time complexity](../../../../../../../time-complexity.md) is $O(V+E)$ for $V$ cells and $E$ dependency references, plus formula arithmetic. The stack depth is at most the longest dependency path. A more elaborate implementation can record reverse dependencies and invalidate only cells affected by an edit.

The PDF gives no policy for circular formulas. Repeated numerical sweeps are not a general solution: a cell defined as itself plus one has no finite value, while a cell defined as itself plus zero has no unique value. The implementation therefore reports a cycle instead of looping or presenting an arbitrary stale value. **An acyclic dependency graph is evaluated once per cell; circular dependencies are detected and rejected.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
