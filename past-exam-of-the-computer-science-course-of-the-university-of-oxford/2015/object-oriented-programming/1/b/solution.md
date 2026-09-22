<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First determine the width of each column by finding the longest rendered [String data type](../../../../../string-data-type.md) value in it. Independently determine the number of rows as the largest column size. An empty column has width zero. Then traverse rows first and columns second: render a present entry with spaces on the appropriate side, or render an absent entry as an entire column of spaces. Put one separating space between adjacent columns and a newline after each row. In particular, an exhausted column must not shift later entries into its position.

Here is executable [Java](../../../../../java-programming-language.md) for the [algorithm](../../../../../algorithm-split.md). `Column`, defined in part (e), is an ordinary [list](../../../../../list-abstract-data-type.md) of `Data`. The [object interface](../../../../../object-interface.md) in part (c) supplies the three queries used below. Each query sees stable content during this call; concurrent changes to formatting are outside this contract.

```
static String replicate(char c, int n) {
    StringBuilder s = new StringBuilder();
    for (int i = 0; i < n; ++i) s.append(c);
    return s.toString();
}

static String printData(List<Column> columns) {
    int[] width = new int[columns.size()];
    int rows = 0;
    for (int c = 0; c < columns.size(); ++c) {
        Column column = columns.get(c);
        rows = Math.max(rows, column.size());
        for (Data d : column)
            width[c] = Math.max(width[c], d.length());
    }
    StringBuilder out = new StringBuilder();
    for (int r = 0; r < rows; ++r) {
        for (int c = 0; c < columns.size(); ++c) {
            if (c != 0) out.append(' ');
            Column column = columns.get(c);
            if (r >= column.size()) {
                out.append(replicate(' ', width[c]));
            } else {
                Data d = column.get(r);
                String text = d.toString();
                String pad = replicate(' ', width[c] - text.length());
                out.append(d.leftJustified() ? text + pad : pad + text);
            }
        }
        out.append('\n');
    }
    return out.toString();
}
```

The [algorithm](../../../../../algorithm-split.md) uses the stipulated fixed-width characters and assumes entries contain no embedded newlines. If the column widths are $w_0,\ldots,w_{k-1}$ and $k>0$, every emitted row has the same width,

$$
\boxed{\sum_{c=0}^{k-1}w_c+(k-1)\quad\text{characters before its newline}.}
$$

An empty collection, or a collection consisting entirely of empty columns, gives the empty [String data type](../../../../../string-data-type.md) value. Spaces at the end of a short last row are harmless and preserve the rectangular layout.

## ↑ Ancestors (11)

1. [B](../b.md)
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
