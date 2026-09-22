# Spreadsheet tabular model

↑ **Parent:** [Spreadsheet](spreadsheet-split.md)

A [spreadsheet tabular model](spreadsheet-tabular-model.md) assigns a consistent meaning to each row and column. For an original example, let rows 2–4 describe three items, with quantity in column `A`, unit price in column `B`, subtotal in column `C`, and total including tax in column `D`. Put the single shared tax rate in `F1`. The chosen rate $1/5$ is an illustrative assumption. Quantities, unit prices and `F1` are [inputs](input-computer-science.md); columns `C` and `D` hold [spreadsheet formulas](spreadsheet-formula.md) and display their computed values as [outputs](output-computing.md).

Enter decimal [inputs](input-computer-science.md) `2.5`, `1.75`, `4.5` for the unit prices and `0.2` for the tax rate. The following table expresses those values as exact [fractions](fraction.md) so that the [arithmetic](arithmetic-split.md) is easy to check. It does not require typing a fraction into an input [spreadsheet cell](spreadsheet-cell.md) or assume that all [software](software.md) calculates with exact [rational numbers](rational-number.md).

| Row | Quantity (`A`) | Unit price (`B`) | Subtotal (`C`) | Total including tax (`D`) |
| --- | --- | --- | --- | --- |
| 2 | $3$ | $5/2$ | $15/2$ | $9$ |
| 3 | $4$ | $7/4$ | $7$ | $42/5$ |
| 4 | $2$ | $9/2$ | $9$ | $54/5$ |

Start with `C2` containing `=A2*B2` and `D2` containing `=C2*(1+$F$1)`. Here `*` requests [multiplication](multiplication.md), and `1+$F$1` adds the tax fraction to one. Copy these two [spreadsheet formulas](spreadsheet-formula.md) down into rows 3 and 4, a fill operation. The [relative spreadsheet references](relative-spreadsheet-reference.md) change with the destination row: `C3` becomes `=A3*B3` and `D3` becomes `=C3*(1+$F$1)`; `C4` becomes `=A4*B4` and `D4` becomes `=C4*(1+$F$1)`. The [absolute spreadsheet reference](absolute-spreadsheet-reference.md) `$F$1` continues to read the shared rate. Copying [spreadsheet formulas](spreadsheet-formula.md) adjusts relative coordinates while retaining absolute coordinates. [Addresses and References, Absolute and Relative: Relative Addressing; Absolute Addressing; When to Use Relative and Absolute References, final two paragraphs](addresses-and-references-absolute-and-relative-libreoffice-help.md)

<a id="image-original-three-row-spreadsheet-tabular-model-before-and-after-filling-two-spreadsheet-formulas-with-a-shared-absolute-spreadsheet-reference"></a>
![](spreadsheet-copy-fill-shared-rate.png)

**[Figure 1](#image-original-three-row-spreadsheet-tabular-model-before-and-after-filling-two-spreadsheet-formulas-with-a-shared-absolute-spreadsheet-reference). Original three-row spreadsheet tabular model before and after filling two spreadsheet formulas, with a shared absolute spreadsheet reference**.

The same [mathematical expression](expression-mathematics.md) applies to every item. Writing $q_i$ for quantity, $p_i$ for unit price and $t$ for the shared tax rate gives

$$
s_i=q_i p_i,\qquad d_i=s_i(1+t).
$$

For row 2, the exact [arithmetic](arithmetic-split.md) is $(3\cdot5/2)(1+1/5)=(15/2)(6/5)=9$. The subtotals add to $47/2$, so the totals add to $(47/2)(6/5)=141/5$, agreeing with $9+42/5+54/5$. The [spreadsheet formulas](spreadsheet-formula.md) encode the relationship; the displayed numbers are its results for these particular [inputs](input-computer-science.md).

This separation is useful for forecasting and [sensitivity analysis](sensitivity-analysis.md). Keeping quantities and unit prices fixed while changing only `F1` from $1/5$ to $1/4$ gives exact totals $75/8$, $35/4$, and $45/4$. More generally, a rate change $\Delta t$ changes each total by

$$
d_i(t+\Delta t)-d_i(t)=s_i\Delta t.
$$

This follows by expanding the two [mathematical expressions](expression-mathematics.md) and cancelling $s_i(1+t)$. Here $\Delta t=1/20$, so the increases are $3/8$, $7/20$, and $9/20$, adding to $47/40$. One shared [input](input-computer-science.md) makes the assumption visible and consistent across all rows. Overwriting a computed total with a number would instead remove that [spreadsheet formula](spreadsheet-formula.md); its value would cease to follow the model when the rate changes.

// Target: computer-science.bigb

## ↑ Ancestors (3)

1. [Spreadsheet](spreadsheet-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Absolute spreadsheet reference](absolute-spreadsheet-reference.md)
- [Multiplication table](multiplication-table.md)
- [Spreadsheet cell](spreadsheet-cell.md)
- [Spreadsheet tabular model](spreadsheet-tabular-model.md)
