<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the weekday number as an [array index](../../../../../array-index.md). Before adding dates, add one empty entry to each weekday before `start`; otherwise the first date in those columns would appear a week too early. For day $d$, the slot number is $\texttt{start}+d-1$, whose remainder modulo 7 selects the column. The source's example makes clear that `start` counts empty weekday cells, rather than individual printed space characters.[p. 3, Question 1(e) and Figure 1, month(1,30)](../../../../../object-oriented-programming-examination-paper-of-the-university-of-oxford-2015.md)

With `import java.util.*;`, the remaining [Java](../../../../../java-programming-language.md) code is:

```
final class Column extends ArrayList<Data> {
    private static final long serialVersionUID = 1L;
}

static String month(int start, int numDays) {
    if (start < 0 || start >= 7 || numDays < 1 || numDays > 31)
        throw new IllegalArgumentException("invalid month parameters");
    String[] days = {"Su", "Mo", "Tu", "We", "Th", "Fr", "Sa"};
    int ncols = days.length;
    List<Column> output = new ArrayList<Column>(ncols);
    for (int c = 0; c < ncols; ++c) {
        Column column = new Column();
        column.add(new StringData(days[c], true));
        output.add(column);
    }
    for (int c = 0; c < start; ++c)
        output.get(c).add(new StringData("", true));
    for (int d = 1; d <= numDays; ++d) {
        int c = (start + d - 1) % ncols;
        output.get(c).add(new IntegerData(d, false));
    }
    return printData(output);
}
```

The two-character headers force every column to width two, and right justification aligns one-digit dates with the units digits of two-digit dates. Date $d$ appears in data row $\lfloor(\texttt{start}+d-1)/7\rfloor$, below the header. For `month(1,30)` the visible result is

```
Su Mo Tu We Th Fr Sa
    1  2  3  4  5  6
 7  8  9 10 11 12 13
14 15 16 17 18 19 20
21 22 23 24 25 26 27
28 29 30
```

The last physical line may also carry spaces for its empty trailing cells. Every physical line ends with a newline. In particular,

$$
\boxed{\text{weekday}(d)=(\texttt{start}+d-1)\bmod7.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
